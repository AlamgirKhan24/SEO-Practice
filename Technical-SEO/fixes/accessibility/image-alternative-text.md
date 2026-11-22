# Fix Guide: Missing or Unhelpful Image Alternative Text

**Category:** Accessibility

## 1. What's wrong

Meaningful images are missing alternative text or use text that does not communicate the image's purpose. Decorative images may be announced unnecessarily when they should have empty alternative text.

## 2. Why it matters

Alternative text gives screen-reader users a text equivalent for meaningful images and can help search engines understand image content. It should describe the image's purpose in context; adding keywords without a user benefit is not appropriate.

## 3. How to check it yourself

1. Review the affected page with images disabled or inspect image elements in the browser.
2. Check each image's `alt` attribute and surrounding text.
3. Determine whether the image conveys information, performs an action, or is purely decorative.
4. Record the affected URLs and a representative example.

## 4. Step-by-step fix

1. For an informative image, write a concise description of the information it contributes in that page context.
2. For an image link or button, describe the destination or action if adjacent text does not already provide it.
3. For decorative images that add no information, use an empty attribute: `alt=""`.
4. In a CMS, update the image field or page component that generates the affected markup. Avoid filling alt text with filenames or keyword lists.
5. If the image is a chart or diagram, provide the key information in nearby text as well as a concise alt description.

## 5. How to verify the fix worked

Inspect the rendered page and confirm each affected image has appropriate alternative text, decorative images are ignored, and the content remains understandable without the image.

## 6. Tools to double-check

- Browser developer tools
- Keyboard and screen-reader review
- Accessibility scanner as a supplementary check
