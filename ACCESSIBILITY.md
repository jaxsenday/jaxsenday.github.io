# Accessibility Checklist

This site should be maintained with WCAG 2.1 Level AA in mind.

## Before publishing any update

- Make sure every new image has meaningful alt text, or empty alt text if it is purely decorative.
- Keep headings in order and avoid skipping levels for styling.
- Use descriptive link text. Avoid labels such as `click here`, `more`, or `view`.
- Preserve sufficient color contrast when changing text, links, borders, backgrounds, or focus styles.
- Test keyboard navigation with `Tab`, `Shift+Tab`, and `Enter`.
- Check the page at 200% zoom and confirm content still reflows without overlap or clipping.
- Keep important content as real text rather than embedding it inside images.
- Treat every uploaded PDF, including a CV, as a separate accessibility task.

## This repository

- Most content updates happen in [`_data/site.yml`](/Users/jaxsen/Documents/GitHub/jaxsenrday/_data/site.yml).
- Layout and navigation behavior live in [`_layouts/default.html`](/Users/jaxsen/Documents/GitHub/jaxsenrday/_layouts/default.html).
- Visual styles and focus behavior live in [`assets/css/style.css`](/Users/jaxsen/Documents/GitHub/jaxsenrday/assets/css/style.css).

## Recommended checks after each update

- Open `https://jaxsenday.github.io/`
- Test keyboard-only navigation
- Confirm focus indicators are easy to see
- Check reading order with VoiceOver if possible
- Review the page at high zoom

## Notes

- Passing this checklist does not by itself guarantee legal compliance or formal conformance.
- Any future embedded media, forms, or third-party widgets should be reviewed separately.
