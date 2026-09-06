# Design Improvement Suggestions

This document lists practical design improvements for the Hamburg Catholics website based on the current homepage and shared layouts.

## 1) Improve homepage content hierarchy

### Why
The homepage currently places long informational sections and multiple alerts close together, which can make it harder for first-time visitors to quickly find service time/location and next steps.

### Suggestions
- Convert the top alerts into a single **“Latest Updates”** section with clear date labels and a consistent card style.
- Add a short **quick-actions row** near the top (e.g., “Mass Times”, “Location”, “Newsletter”, “Sacramental Registration”).
- Introduce a compact **service summary card** with mass time and address so key details are visible without scrolling.

## 2) Replace inline image styling with reusable classes

### Why
Inline image styles are currently used in content blocks, which makes consistent spacing and responsiveness harder to maintain.

### Suggestions
- Move image sizing and float/margin settings into SCSS utility classes (e.g., `.profile-image`, `.content-image-right`).
- Add mobile breakpoints so images stack above text on smaller screens.
- Standardize image treatment (radius, spacing, optional subtle border) for a more cohesive visual identity.

## 3) Strengthen mobile readability

### Why
Several sections are text dense and can be difficult to scan on mobile.

### Suggestions
- Increase paragraph spacing and line height slightly in body content.
- Use clear section dividers or card containers for major homepage sections.
- Ensure iframes and media blocks maintain comfortable spacing and full-width behavior on small screens.

## 4) Improve navigation clarity

### Why
The current fixed navbar is simple, but can better support new visitors trying to find critical pages quickly.

### Suggestions
- Highlight one primary action in navigation (e.g., “Mass & Location” or “Contact”).
- Add active-state styling for the current page.
- Consider grouping utility links (newsletter, forms) separately from informational pages.

## 5) Use a consistent call-to-action system

### Why
Links currently appear in different contexts (alerts, paragraphs), reducing visual consistency.

### Suggestions
- Introduce primary and secondary button styles for key actions.
- Use concise CTA labels (e.g., “Register for First Communion”, “Subscribe to Newsletter”).
- Keep only 1–2 primary CTAs per section to avoid decision overload.

## 6) Polish typography and spacing scale

### Why
A consistent type and spacing system improves perceived quality and readability.

### Suggestions
- Define a spacing scale (e.g., 8/16/24/32 px) and use it consistently between sections.
- Tighten heading hierarchy so H2/H3 sections are visually distinct but balanced.
- Consider slightly darker body text color for stronger contrast and readability.

## 7) Improve accessibility and semantic structure

### Why
Accessibility improvements benefit all users and improve maintainability.

### Suggestions
- Ensure heading levels follow a strict logical order.
- Add descriptive link text (avoid generic labels like “Form” in isolation).
- Verify color contrast in alerts/buttons and include visible keyboard focus styles.

## 8) Build trust with location and contact blocks

### Why
Visitors often need immediate confirmation of where and when to attend.

### Suggestions
- Add a compact **“Visit Us”** block with mass time, church address, and transit/parking note.
- Add a **“Contact the Community”** block near the footer with email and expected response information.
- Optionally include a small FAQ link for newcomers.

## Suggested implementation order

1. Content hierarchy + quick-actions + CTA consistency
2. Reusable image/media classes and mobile spacing updates
3. Navigation polish and active-state styling
4. Accessibility pass (headings, labels, focus, contrast)

## Success criteria

- First-time visitors can identify mass time and location in under 5 seconds.
- Homepage key actions are visible without hunting through body text.
- Mobile readability and spacing feel consistent across sections.
- Core pages retain the same visual rhythm and CTA style.
