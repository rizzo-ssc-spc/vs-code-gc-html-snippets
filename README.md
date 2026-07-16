# GCWeb, GCDS, and WET HTML snippets for VS Code

This repository contains an expanded VS Code snippet collection for Government of Canada web patterns. It is based on the official GCWeb and GCDS guidance and the WET working examples inventory, with separate snippet families for each library, making it easier to browse and reuse.

## Snippet library

The snippet library includes:

- WET working-example and plugin-style snippets for common patterns such as calendars, feedback forms, footnotes, overlays, lightboxes, tabs, toggles, share widgets, data-ajax, form validation, multimedia, and more
- GCDS component and style snippets for buttons, links, cards, alerts, notices, forms, tables, tags, breadcrumbs, callouts, lists, quotes, and step lists
- GCWeb component snippets for Canada.ca patterns such as skip links, breadcrumbs, page titles, containers, tables, panels, most requested links, services and information, step-by-step lists, search boxes, feedback, page details, contributors, and institutional patterns

## Source references

The snippets were shaped from the following authoritative guidance:

- GCWeb and WET: https://wet-boew.github.io/GCWeb/index-en.html
- WET working examples: https://wet-boew.github.io/v4.0-ci/demos/index-en.html
- GC Design System: https://design-system.canada.ca/en/

## Files

- gc-web-snippets.code-snippets — reusable VS Code snippets in JSON format
- README.md — installation and quick-reference documentation

## How to install in VS Code

Code snippets is a santard VS code feature. The easiest way to use these snippets is to load them into VS Code as an HTML snippet file.

### Option A: install into your VS Code user snippets folder (recommended)

1. Select all of the content in the [gc-web-snippets.code-snippets](https://github.com/rizzo-ssc-spc/vs-code-gc-html-snippets/blob/main/gc-web-snippets.code-snippets) file and copy it
2. In VS Code, open the Command Palette with Ctrl+Shift+P
3. Type Snippets: Configure Snippets and press Enter
4. Choose from the list
   1. "New Snippets file for 'workspace' to install in your current workspace
   2. "New Global Snippets file" to install and use it in all of your workspaces
5. This opens your HTML snippet configuration file
6. Replace the default content with the content you copied from [gc-web-snippets.code-snippets](https://github.com/rizzo-ssc-spc/vs-code-gc-html-snippets/blob/main/gc-web-snippets.code-snippets)
7. Save the file
8. Close and reopen VS Code, or reload the window if prompted
9. Open any HTML or templating file such as .html
10. Start typing a prefix such as `wet-panels` or  `gcds-card` and press Tab

### Option B: replace the default HTML snippets file directly

If you prefer a simpler path, you can copy the contents of gc-web-snippets.code-snippets into your existing HTML snippets file:

1. Open the file path below in File Explorer:
   - Windows: %APPDATA%\Code\User\snippets\html.code-snippets
2. Paste the contents of gc-web-snippets.code-snippets into that file
3. Save the file
4. Reload VS Code

### How to test that the snippets are working

1. Create or open a new .html file
2. Type one of the prefixes such as wet-panel or gcds-button
3. Press Tab
4. If the snippet appears, installation was successful

### Important note

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
- gcweb-subway
- gcweb-featured-link
- gcweb-institutional-byline
- gcweb-social-media
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
- gcds-hero
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
- wet-archived
- wet-background-image
- wet-basic-html
- wet-calendar
- wet-chart
- wet-mobile-a11y
- wet-collapsible-alert
- wet-conditional-template
- wet-country-content
- wet-data-ajax
- wet-data-fusion
- wet-data-inview
- wet-data-json
- wet-data-picture
- wet-datalist
- wet-details-closed
- wet-details-polyfill
- wet-dismissible-content
- wet-do-action
- wet-equal-height
- wet-exit-script
- wet-facebook
- wet-favicon
- wet-feedback-form
- wet-feeds
- wet-fieldflow
- wet-filter
- wet-footnote
- wet-form-validation
- wet-geomap
- wet-hello-world
- wet-date-input
- wet-range-input
- wet-json-manager
- wet-lightbox
- wet-mathml
- wet-menu
- wet-merge-errors
- wet-audio
- wet-video
- wet-youtube
- wet-overlay
- wet-paginate
- wet-pii-scrub
- wet-postback
- wet-prettify
- wet-progress
- wet-randomize
- wet-session-expired
- wet-steps-form
- wet-table-filters
- wet-table-validator
- wet-tables
- wet-tag-filter
- wet-template-html5
- wet-text-highlight
- wet-toggle
- wet-transitions
- wet-twitter
- wet-url-ajax
- wet-url-table
- wet-url-json
- wet-utilities
- wet-a11y-assessment
- wet-core
- wet-zebra
- wet-alert-info
- wet-alert-success
- wet-alert-warning
- wet-badge-info
- wet-badge-success
- wet-button-primary
- wet-button-default
- wet-button-link
- wet-panel
- wet-well
- wet-list-inline
- wet-list-spaced
- wet-list-group
- wet-table-basic
- wet-table-responsive
- wet-labels
- wet-code
- wet-code-prettify
- wet-colour
- wet-datatables
- wet-datalist-polyfill
- wet-equalize
- wet-expand-hide
- wet-grid-system
- wet-headings
- wet-images
- wet-jumbotron
- wet-keyboard
- wet-margin-proximity
- wet-meter
- wet-modal-popup
- wet-multimedia-player
- wet-opacity
- wet-panels
- wet-pills
- wet-quotations
- wet-reflowing
- wet-secondary-menu
- wet-session-timeout
- wet-share-widget
- wet-tabbed-interface
- wet-zebra

## How to use placeholders

Each snippet uses Tab-stops so you can quickly fill in content:

- ${1:placeholder} — first editable field
- ${2:placeholder} — second editable field
- $0 — final cursor position

Press Tab to move through the placeholders.

## Authoring guidance

- Replace placeholder text with real content before publishing
- Validate the final markup against the latest GCWeb, WET and GCDS before publication
- Use the [W3C HTML Validator](https://validator.w3.org/nu/#textarea) to make sure there are no errors in the HTML
- Feel free to customize the HTML snippets however you like. It's also appreciated if you want to collaborate with the file in this project! :)

## Accessibility notes

All web pages must met WCAG 2.1 Level AA standards. These snippets are designed with accessibility in mind and include patterns for:

- skip links
- ARIA labels and landmarks
- descriptive labels for forms and search
- status messaging for alerts
- keyboard-friendly disclosure and modal patterns

For production use, review the final markup against WCAG guidance and the current Canada.ca Content Style Guide implementation standards.
