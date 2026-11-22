# Fix Guide: Insufficient Text or Interface Contrast

**Category:** Accessibility

## 1. What's wrong

Text or essential interface elements are difficult to distinguish from their background because the foreground and background colors have insufficient contrast.

## 2. Why it matters

Low contrast makes content harder to read for many users, including people with low vision or in bright environments. It can also obscure important states such as focus, selection, or errors.

## 3. How to check it yourself

1. Identify the text and interface states reported by the audit, including hover, focus, disabled, and error states where relevant.
2. Sample the actual foreground and background colors from the rendered page.
3. Check the ratio with a contrast analyzer and compare it with the applicable WCAG criterion.
4. Record the page/component, colors, measured ratio, and text size or interface use.

## 4. Step-by-step fix

1. Adjust the foreground or background color to meet the applicable contrast requirement while preserving the site's design system.
2. Check color combinations in all component states, not only the default view.
3. Keep meaning clear without relying on color alone; add labels, icons, or other visual cues where needed.
4. Update the shared token or component when multiple templates use the same problematic combination.

## 5. How to verify the fix worked

Re-measure the rendered color pair and review the component in its relevant states. Confirm that the change remains legible across responsive layouts and themes.

## 6. Tools to double-check

- WCAG contrast analyzer
- Browser developer tools
- Keyboard review for focus and state visibility
