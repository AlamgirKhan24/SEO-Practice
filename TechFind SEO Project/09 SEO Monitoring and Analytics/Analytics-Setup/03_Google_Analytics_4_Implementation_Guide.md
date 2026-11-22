# Google Analytics 4 Implementation Guide

**Status:** Planned setup; no TechFind GA4 property, site code, consent configuration, tag implementation, ecommerce backend or event validation evidence was supplied.

## Setup sequence

1. Create a GA4 property under the authorized business account and set property time zone/currency deliberately to match reporting and commerce configuration.
2. Create a Web data stream for the production domain and record the Measurement ID in a secure implementation log (not public docs).
3. Install the Google tag through the chosen CMS/tag manager or engineering implementation. Follow the business's consent and privacy requirements; do not deploy tags before appropriate consent controls are configured.
4. Configure cross-domain measurement only if a real checkout/payment journey spans owned domains. Exclude internal/test traffic and document filters.
5. Enable Enhanced Measurement only for relevant interactions and verify its behavior to avoid duplicate or unwanted events.
6. Use DebugView/Tag Assistant and GA4 Realtime for QA; then reconcile purchases/revenue against the backend and test order flow before relying on reports.
7. Mark only business-approved outcomes as key events (e.g. `purchase`, qualified `generate_lead`). Do not mark every engagement event as a conversion.

## Ecommerce event specification

Use GA4 recommended ecommerce event names and an `items` array. Key parameters should be populated from actual catalog/transaction data and use consistent types/currency. Never send personally identifiable information.

| Event | Trigger | Core data to capture |
|---|---|---|
| `view_item_list` | A visible product list/category appears | `item_list_id`, `item_list_name`, `items[]` with item identifiers, name, brand, category, list position, price as appropriate |
| `select_item` | User selects an item from a list | List identifiers and selected item object |
| `view_item` | Product detail is viewed | `currency`, `value` if appropriate, `items[]` with stable `item_id`, `item_name`, brand/category, price, actual variant/configuration |
| `add_to_cart` | Item successfully added | `currency`, `value`, `items[]` with item ID, quantity, price, variant |
| `remove_from_cart` | Item removed | Same item/quantity/price context as available |
| `begin_checkout` | Checkout starts | `currency`, `value`, `items[]`; coupon/shipping/tax only if actual values known and event spec warrants |
| `purchase` | Order confirmed (not merely payment button clicked) | Unique `transaction_id`, `currency`, `value`, `tax`, `shipping`, `coupon` where actual, and purchased `items[]` |

Use stable item IDs matching product reporting; transmit actual values with currency; prevent duplicate purchase firing by transaction ID; ensure canceled/failed orders are handled consistently. Parameters should follow current GA4 schema and the business's data-minimization policy.

## Reporting and QA

- Acquisition: organic sessions by source/medium, landing page and device.
- Landing pages: engaged sessions and key events for organic landings.
- Ecommerce: item views, cart, checkout and purchase funnel, product/category, device and revenue.
- QA: event naming, required parameters, currency, numeric types, item IDs, duplicate counts, consent behavior, internal traffic and backend revenue reconciliation.

Suggested official references: [GA4 ecommerce measurement](https://developers.google.com/analytics/devguides/collection/ga4/ecommerce), [recommended events](https://developers.google.com/analytics/devguides/collection/ga4/reference/events), [create a GA4 property](https://support.google.com/analytics/answer/9304153), [DebugView](https://support.google.com/analytics/answer/7201382).

No tracking is claimed as implemented or tested. Have the authorized developer/privacy owner verify current requirements before launch.
