# Accessibility Cheatsheet

This cheatsheet provides a quick guide to common accessibility issues you might encounter in this codebase. Use it as a reference during the workshop.

## Common Accessibility Issues

### 1. Color Contrast
Text and background colours must meet contrast ratio AA WCAG standard.

**Tips**: Use tools like [Deque Contrast Checker](https://dequeuniversity.com/color-contrast) or Chrome DevTools built-in contrast checker (check color style property on text tags) to ensure compliance.

### 2. Lack of Keyboard Navigation
Interactive elements (e.g., buttons, links) must always be focusable or operable via keyboard.

**Tips**: Ensure all interactive elements are focusable and test with the `Tab` key. 

### 3. Missing Focus Indicators
Interactive elements (e.g., buttons, links) require visible focus indicators for keyboard navigation.

**Tips**: Ensure focus indicators are clearly visible and meet contrast requirements.Check for places where CSS may have been overriden using `:focus` selector.

### 4. Focus Indicators on Non-Interactive Elements
Non-interactive elements (e.g., `<div>` or `<span>`) should not have focus indicators or be operable by tabbing.

**Tips**: Keep an eye out for altered focusability of non-interactive elements using `tabindex`.

### 5. Placeholders with Low Contrast
Placeholder text is not very accessible or usable in form fields, especially if it has insufficient contrast.

**Tips**: Ensure placeholder text meets contrast requirements or provide visible labels outside the input field.

### 6. Using Only Color to Indicate Errors
Errors should not be indicated solely by colour without additional labels or text since this is inaccessible for users with colour blindness.

**Tips**: Use meaningful text error messages to provide error context alongside color.

## Tools for Testing Accessibility
- [axe DevTools](https://www.deque.com/axe/)
- [Lighthouse](https://developers.google.com/web/tools/lighthouse)
- [Deque Colour Contrast Checker](https://dequeuniversity.com/color-contrast)

## Additional Resources
- [Web Content Accessibility Guidelines (WCAG)](https://www.w3.org/WAI/standards-guidelines/wcag/)
- [Accessibility Insights](https://accessibilityinsights.io/)

Happy debugging!