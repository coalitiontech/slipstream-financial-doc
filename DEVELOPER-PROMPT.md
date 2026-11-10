# Prompt to complete the documentation

Copy the prompt below into your development AI while both the documentation repository and the current WordPress theme are available. Supply the site URL and theme path if they are not already in its workspace.

```text
Complete the existing Slipstream Financial WordPress documentation with small, targeted additions. Work directly in the documentation repository and preserve the base already created.

Start by reading README.md, mkdocs.yml, docs/*.md, and applicable AGENTS.md instructions. Inspect the current WordPress theme, its ACF JSON fields, block renderers, templates, Customizer controls, menus and form integration. If an authorized WordPress admin session is available, verify the actual page configuration there. Ask for missing access only when needed; continue source-based documentation work independently.

Preserve these existing elements:
- The README exactly as it is.
- The MkDocs setup, current navigation order and page filenames.
- The purple/navy/cyan styling in docs/style.css.
- Existing useful copy, basic instructions and the three WordPress editing screenshots in docs/img/.
- The distinction between verified implementation and details still awaiting confirmation.

Extend the appropriate existing pages rather than rewriting the guide. Correct an existing statement only when current code or the actual admin interface proves it inaccurate, and report that correction. Add a new page or navigation item only when a substantial topic genuinely cannot fit an existing page. Do not redesign the documentation, switch frameworks, or reintroduce storefront/product instructions from the old template.

Prioritize practical instructions for a nontechnical site editor:
1. Identify the real homepage, content pages, Resources/blog pages and their templates. Explain which content comes from blocks, posts, Customizer settings or theme defaults.
2. Add short walkthroughs for the blocks actually used: locating the block in List View, editing its named fields, updating images/buttons/repeater rows, previewing and saving. Do not document every unused starter block just because it exists in the code.
3. Verify header/footer controls and menu locations, then document how to maintain them.
4. Confirm the forms actually used and explain field editing, confirmations, notifications and testing. Do not expose private recipient addresses, entries, credentials or license keys.
5. Add verified project-specific notes for blog categories, featured images and resource listings. Include maintenance/deployment details only when confirmed and relevant.

Use actual field labels and page names. Never treat seed scripts, sample pages, PHP fallback content or design proposals as proof of production configuration. The existing Finley CTA screenshots show an unpublished demonstration page, not production page content. Do not turn that example into a published page.

Keep the current screenshots. Add only a few additional screenshots if essential to explain an otherwise unclear step. Capture the real admin UI, crop browser tabs/bookmarks and remove sensitive information; do not fabricate screenshots. Inspect every new image for readability before adding it.

Keep changes scoped to documentation and its generated site output. Do not change site content, theme code, plugins, configuration or credentials to make the documentation match. Do not publish, deploy, commit or push unless separately requested. If access is unavailable, record a concise verification item in docs/developers.md instead of guessing.

Before finishing:
- Review the diff for unnecessary rewrites and preserve unrelated changes.
- Verify internal Markdown links, image paths and navigation.
- Run mkdocs build --strict to regenerate site/ and resolve build warnings/errors.
- Run git diff --check.
- Report what was added or corrected, what was verified in source versus WordPress admin, and any specific remaining verification items.
```
