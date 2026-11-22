# GA4 Setup Guide

**Instructions only. No Analytics property, tag or measurement ID is configured for GlowCare.**

## Setup sequence
1. Create or select the organization’s Google Analytics account and create a GA4 property with the agreed reporting time zone and currency (PKR only if actual commerce uses it).
2. Create a Web data stream for the confirmed production domain. Record the Measurement ID securely in the implementation register; do not put secrets in public files.
3. Install the Google tag directly or through Google Tag Manager using one controlled deployment path. Avoid duplicate base tags. Configure consent management and data collection to meet applicable privacy requirements.
4. Configure internal/developer traffic rules and test filters before activation because excluded data may be permanently unavailable in reports. Exclude internal traffic carefully; don’t filter users based on unstable identifiers.
5. Set data retention based on business need and policy; Google’s standard properties offer 2- or 14-month user/event retention options in applicable settings. [Data retention](https://support.google.com/analytics/answer/7667196)
6. Configure cross-domain measurement only for genuine checkout domains. Review unwanted referrals only when payment/checkout referral behavior is understood.
7. Verify with Tag Assistant, GA4 Realtime and DebugView. Test consent states, page_view, ecommerce events and a controlled test order. Remove debug traffic from production reporting. [DebugView](https://support.google.com/analytics/answer/7201382)
8. Reconcile purchase count/revenue to the backend before treating GA4 ecommerce metrics as business actuals.

## Privacy and data quality
Never send names, email addresses, phone numbers, full postal addresses, order notes, payment card data, or other personal information to GA4. Use non-identifying product/SKU identifiers and transaction IDs that do not encode personal information. Document consent behavior, access roles, retention and deletion process. Implementation needs developer and privacy review.
