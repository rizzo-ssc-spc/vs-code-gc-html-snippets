# GCWeb, GCDS, and WET HTML snippets for VS Code

This folder contains a broader VS Code snippet collection for Government of Canada web patterns. It is built around the official GCWeb and GCDS guidance and the component examples documented in the WET working examples library.

## What is included

The collection now covers a wide range of reusable patterns such as:

- accessibility landmarks and skip links
- breadcrumbs, page titles, and pagination
- tables, panels, cards, accordions, and tabs
- alerts, callouts, footnotes, and dismissible content
- forms, validation, dates, ranges, and autocomplete patterns
- downloadable assets, media, lightboxes, overlays, and share widgets
- Canada.ca-style sections such as services and information and most requested links

## Source references

The snippets were shaped from the following authoritative guidance:

- GCWeb and WET: https://wet-boew.github.io/GCWeb/index-en.html
- WET working examples: https://wet-boew.github.io/v4.0-ci/demos/index-en.html
- GC Design System: https://design-system.canada.ca/en/

## Files

- gc-web-snippets.code-snippets — reusable VS Code snippets in JSON format
- README.md — installation and quick-reference documentation

## How to install in VS Code

1. Open VS Code.
2. Copy the snippet file into your user snippets folder:
   - Windows: %APPDATA%\Code\User\snippets\html.code-snippets
3. Reload VS Code or restart the editor.
4. Open any HTML or templating file such as .html, .njk, .liquid, .vue, .jsx, or .tsx.
5. Start typing a prefix such as gcweb-skip-link, gcds-header, or wet-tabs and press Tab.

## Common snippet prefixes

### GCWeb
- gcweb-skip-link
- gcweb-breadcrumb
- gcweb-page-title
- gcweb-table
- gcweb-accordion
- gcweb-modal
- gcweb-search
- gcweb-most-requested

### GCDS
- gcds-header
- gcds-footer
- gcds-button
- gcds-card
- gcds-alert
- gcds-input
- gcds-radio
- gcds-hero

### WET
- wet-download-link
- wet-image-caption
- wet-feedback-form
- wet-form-validation
- wet-alert
- wet-footnote
- wet-lightbox
- wet-overlay
- wet-tabs
- wet-toggle
- wet-progress
- wet-share
- wet-calendar

## How to use placeholders

Each snippet uses Tab-stops so you can quickly fill in content:

- ${1:placeholder} — first editable field
- ${2:placeholder} — second editable field
- $0 — final cursor position

Press Tab to move through the placeholders.

## Authoring guidance

- Replace placeholder text with real content before publishing.
- Keep link text, button text, and labels concise and useful.
- Preserve accessibility by pairing labels with inputs, using descriptive link text, and keeping interactive controls keyboard accessible.
- Prefer meaningful page headings and clear section structure.

## Accessibility notes

These snippets are designed with accessibility in mind and include patterns for:

- skip links
- ARIA labels and landmarks
- descriptive labels for forms and search
- status messaging for alerts
- keyboard-friendly disclosure and modal patterns

For production use, validate the final markup against the latest GCWeb, WET, and GCDS guidance before publication.
