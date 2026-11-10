# Slipstream Financial documentation

A small MkDocs guide for the custom WordPress site. Edit the Markdown files in `docs/`; navigation is in `mkdocs.yml` and brand styling in `docs/style.css`.

## Local preview

```sh
python3 -m pip install -r requirements.txt
mkdocs serve
```

## Build and check

```sh
mkdocs build --strict
```

The generated output is in `site/`. Rebuild it whenever the source changes. No publishing is performed by the build command.

## Scope

The base covers page editing, homepage sections, blog/resources, Customizer settings, menus and Gravity Forms integration. Facts are drawn from the local theme implementation. Database-dependent details still need verification. See `docs/developers.md` for the handoff checklist.
