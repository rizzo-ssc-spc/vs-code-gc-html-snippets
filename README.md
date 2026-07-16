# GCWeb, GCDS, and WET HTML snippets for VS Code

This folder contains an expanded VS Code snippet collection for Government of Canada web patterns. It is based on the official GCWeb and GCDS guidance and the WET working examples inventory, with separate snippet families for each library so the collection is easier to browse and reuse.

## What changed in this update

The snippet library now includes:

- WET working-example and plugin-style snippets for common patterns such as calendars, feedback forms, footnotes, overlays, lightboxes, tabs, toggles, share widgets, data-ajax, form validation, multimedia, and more
- GCDS component and style snippets for buttons, links, cards, alerts, notices, forms, tables, tags, breadcrumbs, callouts, lists, quotes, and step lists
- GCWeb component snippets for Canada.ca patterns such as skip links, breadcrumbs, page titles, containers, tables, panels, most requested links, services and information, step-by-step lists, search boxes, feedback, page details, contributors, and institutional patterns
- Accessibility-focused placeholders and labels so the generated markup is more usable for WCAG-friendly implementation work

## Source references

The snippets were shaped from the following authoritative guidance:

- GCWeb and WET: https://wet-boew.github.io/GCWeb/index-en.html
- WET working examples: https://wet-boew.github.io/v4.0-ci/demos/index-en.html
- GC Design System: https://design-system.canada.ca/en/

## Files

- gc-web-snippets.code-snippets — reusable VS Code snippets in JSON format
- README.md — installation and quick-reference documentation

## How to install in VS Code

The easiest way to use these snippets is to load them into VS Code as an HTML snippet file. This is a standard VS Code feature, and the steps below are written for someone who has not used snippets before.

### Option A: install into your VS Code user snippets folder (recommended)

1. Open the workspace that contains this folder in VS Code.
2. In the Explorer, open the file named gc-web-snippets.code-snippets.
3. Select all of the content in the file and copy it.
4. Open the Command Palette with Ctrl+Shift+P.
5. Type Preferences: Configure User Snippets and press Enter.
6. Choose html from the list. This opens your HTML snippet configuration file.
7. Replace the default content with the content you copied from gc-web-snippets.code-snippets.
8. Save the file.
9. Close and reopen VS Code, or reload the window if prompted.
10. Open any HTML or templating file such as .html, .njk, .liquid, .vue, .jsx, or .tsx.
11. Start typing a prefix such as gcweb-skip-link, gcds-header, or wet-tabs and press Tab.

### Option B: replace the default HTML snippets file directly

If you prefer a simpler path, you can copy the contents of gc-web-snippets.code-snippets into your existing HTML snippets file:

1. Open the file path below in File Explorer:
   - Windows: %APPDATA%\Code\User\snippets\html.code-snippets
2. Paste the contents of gc-web-snippets.code-snippets into that file.
3. Save the file.
4. Reload VS Code.

### How to test that the snippets are working

1. Create or open a new .html file.
2. Type one of the prefixes such as gcweb-skip-link or gcds-button.
3. Press Tab.
4. If the snippet appears, installation was successful.

### Important note for beginners

A .code-snippets file in your workspace will not automatically appear in VS Code just because it is open in the folder. It must be loaded into the VS Code snippets system using one of the steps above.

## Common snippet prefixes

### GCWeb
- gcweb-skip-link
- gcweb-breadcrumb
- gcweb-page-title
- gcweb-container
- gcweb-table
- gcweb-panel
- gcweb-most-requested
- gcweb-services-info
- gcweb-step-by-step
- gcweb-toc
- gcweb-search-box
- gcweb-feedback
- gcweb-page-details
- gcweb-contributors
- gcweb-minister

### GCDS
- gcds-header
- gcds-footer
- gcds-button
- gcds-button-secondary
- gcds-link
- gcds-card
- gcds-alert
- gcds-notice
- gcds-input
- gcds-textarea
- gcds-select
- gcds-checkbox
- gcds-radio
- gcds-table
- gcds-tag
- gcds-details
- gcds-breadcrumb
- gcds-callout
- gcds-list
- gcds-quote
- gcds-steps

### WET
- wet-add-to-calendar
- wet-alert-info
- wet-alert-success
- wet-alert-warning
- wet-badge-info
- wet-badge-success
- wet-button-primary
- wet-button-default
- wet-button-link
- wet-panel
- wet-panels
- wet-well
- wet-list-inline
- wet-list-spaced
- wet-list-group
- wet-table-basic
- wet-table-responsive
- wet-calendar
- wet-collapsible-alert
- wet-code
- wet-code-prettify
- wet-colour
- wet-datalist
- wet-datalist-polyfill
- wet-datatables
- wet-data-ajax
- wet-dismissible-content
- wet-equalize
- wet-expand-hide
- wet-feedback-form
- wet-footnote
- wet-form-validation
- wet-grid-system
- wet-headings
- wet-images
- wet-jumbotron
- wet-keyboard
- wet-labels
- wet-lightbox
- wet-margin-proximity
- wet-meter
- wet-modal-popup
- wet-multimedia-player
- wet-opacity
- wet-overlay
- wet-paginate
- wet-pills
- wet-prettify
- wet-progress
- wet-quotations
- wet-reflowing
- wet-secondary-menu
- wet-session-timeout
- wet-share
- wet-share-widget
- wet-tabbed-interface
- wet-tabs
- wet-toggle
- wet-zebra

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
- Validate the final markup against the latest GCWeb, WET, and GCDS guidance before publication.

## Accessibility notes

These snippets are designed with accessibility in mind and include patterns for:

- skip links
- ARIA labels and landmarks
- descriptive labels for forms and search
- status messaging for alerts
- keyboard-friendly disclosure and modal patterns

For production use, review the final markup against WCAG guidance and the current Canada.ca implementation standards.
