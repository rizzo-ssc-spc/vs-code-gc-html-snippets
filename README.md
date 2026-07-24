# GCWeb, GCDS, and WET HTML snippets

A reusable snippet library for Government of Canada web development patterns across GCWeb, GCDS, and WET.

## Beta status

This snippet pack is currently in beta.

- Snippets are actively updated as GCWeb, WET, and GCDS examples evolve
- Some prefixes and snippet bodies may still change between versions
- Feedback and contribution are welcome

## Contributing

- Open an issue for bugs, broken snippets, or standards drift
- Propose snippet updates by sharing before/after examples
- Include links to the official GCWeb, WET, or GCDS reference used

This project is optimized for VS Code and VS Code-based editors, and may also be used in other IDEs with conversion or manual setup.

## What this repo includes

- WET snippets for common components and plugin patterns
- GCWeb snippets for Canada.ca page structures and UI patterns
- GCDS snippets for design-system-based components

## Repository files

- gc-web-snippets.code-snippets: the main snippet library in VS Code JSON format
- README.md: installation and usage guide
- snippets-test.html: local test page for trying prefixes quickly

## Quick start (VS Code)

1. Open [gc-web-snippets.code-snippets](https://github.com/rizzo-ssc-spc/vs-code-gc-html-snippets/blob/main/gc-web-snippets.code-snippets)
2. Copy all content
3. In VS Code, press Ctrl+Shift+P and run Snippets: Configure Snippets
4. Choose HTML (global or workspace)
5. Paste the snippet JSON and save
6. Open an HTML file and test a prefix such as wet-panels

## Installation details

### Option A (recommended): configure snippets from VS Code UI

1. Open [gc-web-snippets.code-snippets](https://github.com/rizzo-ssc-spc/vs-code-gc-html-snippets/blob/main/gc-web-snippets.code-snippets)
2. Copy all content
3. Open the VS Code
4. Press Ctrl+Shift+P
5. Run Snippets: Configure Snippets
6. Choose either:
   - New Global Snippets file
   - New Snippets file for workspace
7. Select HTML
8. Paste the content of [gc-web-snippets.code-snippets](https://github.com/rizzo-ssc-spc/vs-code-gc-html-snippets/blob/main/gc-web-snippets.code-snippets)
9. Save and reload VS Code if prompted

### Option B: copy directly to the snippets file

Windows path:

%APPDATA%\Code\User\snippets\html.code-snippets

Steps:

1. Open the file above
2. Paste the content of gc-web-snippets.code-snippets
3. Save
4. Reload VS Code

## Use in other IDEs and editors (not tested - beta)

Needs format-specific setup.

### Compatibility at a glance

- Cursor, VSCodium, Windsurf, Theia-based editors: direct support
- JetBrains IDEs (WebStorm, IntelliJ IDEA, PhpStorm): convert to Live Templates XML
- Sublime Text: convert to .sublime-completions or .sublime-snippet
- Adobe Dreamweaver: create snippets manually in the Snippets panel

### VS Code-based editors (Cursor, VSCodium, Windsurf)

1. Copy the full content of [gc-web-snippets.code-snippets](https://github.com/rizzo-ssc-spc/vs-code-gc-html-snippets/blob/main/gc-web-snippets.code-snippets)
2. Open the editor snippet configuration command
3. Open HTML snippets
4. Paste, save, and reload
5. Test using a prefix such as wet-panels

### JetBrains IDEs

JetBrains does not read VS Code snippet JSON directly.

1. Open [gc-web-snippets.code-snippets](https://github.com/rizzo-ssc-spc/vs-code-gc-html-snippets/blob/main/gc-web-snippets.code-snippets)
2. Copy all content
3. Convert VS Code snippets JSON to Live Templates XML
4. In the IDE, open Settings > Editor > Live Templates
5. Create a group such as GCWeb-WET-GCDS
6. Import the converted XML
7. Set the template context to HTML
8. Save and test abbreviations

### Sublime Text

1. Open [gc-web-snippets.code-snippets](https://github.com/rizzo-ssc-spc/vs-code-gc-html-snippets/blob/main/gc-web-snippets.code-snippets)
2. Copy all content
3. Convert snippets to Sublime format
4. Open Preferences > Browse Packages
5. Create a folder such as User/GCWebSnippets
6. Add converted snippet file(s)
7. Restart Sublime Text and test triggers

### Adobe Dreamweaver

Dreamweaver does not import VS Code JSON snippets directly.

Recommended approach: start with a small "starter pack" of high-use snippets and expand over time.

1. Open Dreamweaver and open your site/project first
2. Open the Snippets panel (Window > Snippets)
3. Create a folder for team snippets (for example GCWeb-WET-GCDS)
4. In that folder, create a new snippet
5. Set the snippet type:
   - Insert Block: inserts a full HTML block at the cursor (best for most snippets)
   - Wrap Selection: wraps selected text in markup (useful for patterns such as callouts)
6. Give the snippet a clear name using the VS Code prefix as reference (for example "wet-alert")
7. Copy one snippet body from [gc-web-snippets.code-snippets](https://github.com/rizzo-ssc-spc/vs-code-gc-html-snippets/blob/main/gc-web-snippets.code-snippets) and paste it into Dreamweaver snippet content
8. Replace VS Code placeholder syntax with plain sample text before saving:
   - Replace ${1:...}, ${2:...}, etc.
   - Remove $0
9. Save and test in an HTML page by inserting it from the Snippets panel
10. Repeat for the next most-used snippet

Dreamweaver notes:

- Snippets are inserted from the Snippets panel
- VS Code placeholders such as ${1:Header} are not interpreted by Dreamweaver
- Choice placeholders such as ${1|default,primary,...|} are also not supported

## Verify installation

1. Open or create an HTML file
2. Type a prefix such as wet-panels, wet-datatables, or gcds-details
3. Trigger snippet insertion (usually Tab or Enter depending on editor)
4. Confirm the HTML block is inserted

## Common prefixes (quick reference)

GCWeb examples:

- gcweb-alert-info
- gcweb-alert-warning
- gcweb-alert-danger

GCDS examples:

- gcds-lang-toggle
- gcds-sr-only
- gcds-stepper
- gcds-table
- gcds-grid
- gcds-notice
- gcds-pagination
- gcds-error-message
- gcds-icon

WET examples:

- wet-panels
- wet-alert
- wet-button
- wet-text-colour
- wet-overlay
- wet-tabbed-interface
- wet-datatables
- wet-datatables-options

Tip: use your editor's snippet search to browse all prefixes in gc-web-snippets.code-snippets.

## Placeholder syntax

The snippet file uses VS Code tab stops:

- ${1:placeholder}: first editable field
- ${2:placeholder}: second editable field
- $0: final cursor position

## Authoring and maintenance guidance

- Keep [gc-web-snippets.code-snippets](https://github.com/rizzo-ssc-spc/vs-code-gc-html-snippets/blob/main/gc-web-snippets.code-snippets) as the source of truth
- Validate generated HTML before publishing
- Re-check patterns against current GCWeb, WET, and GCDS documentation
- Keep prefixes stable across tools when converting to other IDE formats

## Accessibility and content quality

- Snippets are designed to support accessible markup patterns
- Final pages must still be reviewed for WCAG conformance and policy compliance
- Validate output with the Nu HTML checker: https://validator.w3.org/nu/#textarea

## Source references

- GCWeb and WET index: https://wet-boew.github.io/GCWeb/index-en.html
- WET working examples: https://wet-boew.github.io/v4.0-ci/demos/index-en.html
- GC Design System: https://design-system.canada.ca/en/
