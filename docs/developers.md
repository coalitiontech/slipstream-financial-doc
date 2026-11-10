# Developer handoff

## Verified source structure

Theme directory: `wp-content/themes/slipstream-financial-wp/`.

| Path | Responsibility |
| --- | --- |
| `front-page.php` | Homepage block content or fallback section composition |
| `blocks/<slug>/` | Block metadata, rendering, styles and optional scripts |
| `acf-json/` | ACF field definitions |
| `inc/customizer.php` | Header, footer and inner-page defaults |
| `inc/setup.php` | Menu locations and theme support |
| `inc/blog.php` | Blog composition |
| `page-templates/inner-page.php` | Inner Page template |
| `page-templates/resources.php` | Resources listing template |
| `assets/css/tokens.css` | Shared brand colors and typography |

This is a classic PHP theme using ACF Pro Gutenberg blocks. Header/footer settings use the WordPress Customizer. Form sections integrate with Gravity Forms. Read the theme’s `AGENTS.md` and conventions before changing code.

## Brand palette

| Role | Color |
| --- | --- |
| Deep ink / footer | `#0d0326` |
| Primary purple | `#a42eff` |
| Soft purple | `#ab3aff` |
| Deep purple | `#7829b3` |
| Cyan accent | `#64fff0` |
| White | `#ffffff` |

The documentation uses deep purple for readable links on white, with dark navigation and cyan highlights.

## Extend this documentation

- Confirm active theme/plugins, page URLs, template assignments and navigation assignments in WordPress.
- Add field-by-field walkthroughs for the actual pages and blocks in use.
- Confirm form IDs, notifications and integrations.
- Add current WordPress screenshots with sensitive information removed.
- Document deployment, backups, caching and any SEO tooling after verifying the actual setup.

Keep this guide focused on editing the site. Label unverified behavior and unfinished sections clearly. Theme seed scripts and design proposals are not proof of current live content.
