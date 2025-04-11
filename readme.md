
# md2website: markdown to static website builder

Example websites:

- [asyncze.com](https://asyncze.com)

## Usage

Change default config

```python
PAGE_TITLE                  = "Michael (@asyncze)"
POSTS_ON_INDEX              = False
DIST_PATH                   = "/dist"
LOAD_FOLDER                 = False
LOAD_FOLDER_FLAGS           = False
AUTHOR                      = "@asyncze"
X_URL                       = "https://x.com/asyncze"
DESCRIPTION                 = "Self-funded software engineer"
FAVICON                     = ""
GOOGLE_TAG                  = ""
APP_NAME                    = "Michael (@asyncze)"
SOCIAL_IMAGE                = ""
```

See **demo_website** folder for folder structure.

```bash
.venv/bin/python md2website.py /demo_website
```

Replace `.venv/bin/python` with path to your `python`.

### Notes

- Page navigation is generated from `nav.md`.
- Post header anchors and table of contents are automatically generated from `##` and `###` tags (if `toc`-flag is set to `true` in `__flags`).
