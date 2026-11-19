# Developer handoff

## Verified source structure

Theme directory: `wp-content/themes/slipstream-financial-wp/`.

| Path | Responsibility |
| --- | --- |
| `front-page.php` | Homepage block content or fallback section composition |
| `blocks/<slug>/` | Block metadata, rendering, styles and optional scripts |
| `acf-json/` | ACF field definitions |
| `inc/customizer.php` | Header, footer, blog hero and inner-page defaults |
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

## Verification log

| Item | Status |
| --- | --- |
| Theme paths, Customizer controls, menu locations, block field labels | Verified from theme source |
| Homepage section order on page **Home** | Reported verified in the developer’s local admin walkthrough |
| Banking & Treasury hero and body blocks | Rechecked November 19, 2026: active theme `slipstream-financial-wp`, page uses `page-templates/inner-page.php`; body begins with Logos Strip and has no Solution Hero block |
| Posts page **Blog**, category **News**, Blog Hero label “Knowledge Base” | Verified in local admin |
| Gravity Forms **1 Homepage Hero** and **2 Contact Lead** (+ field labels) | Verified in local admin |
| Menu location → menu assignments | Verified in local admin |
| Original `wp-*.png` editing screenshots | Captured November 10, 2026, using an unpublished example |
| Numbered admin screenshots | Added in the developer’s November 19, 2026 walkthrough; private fields obscured |
| Production URLs, hosting, caching, SEO plugins | Not verified here |
| GF notification recipients / delivery | Intentionally omitted (private); confirm in WP admin |
| Whether **Resources** should be restored vs using **Blog** | Needs production decision |

## Public-repo safety

Do not add custom login URLs, credentials, license keys, private email addresses, notification recipients, Local MySQL sockets, `wp-config` values or submission data to this repository. Prefer field names and admin paths over secrets.

## Extend this documentation

- Confirm active theme/plugins, page URLs, template assignments and navigation on production.
- Replace local screenshots with production captures when the live admin differs, cropping browser chrome and removing sensitive information.
- Document deployment, backups, caching and SEO tooling only after verifying the actual setup.

Keep this guide focused on editing the site. Label unverified behavior clearly. Theme seed scripts and design proposals are not proof of current live content.
