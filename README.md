# QuickyHug documentation

Source for the QuickyHug documentation website at <https://quickyproducts.github.io/QuickyHug-docs/>.

Same setup as [QuickySitter-docs](https://github.com/QuickyProducts/QuickySitter-docs): Jekyll, built by GitHub Pages from the `devel` branch.

## Building locally

```bash
bundle install
bundle exec jekyll serve
# open http://127.0.0.1:4000/QuickyHug-docs/
```

## Pages

| Page | File |
|---|---|
| HUD Manual | `pages/qh/quickyhug-manual.md` |
| Recommended Viewer Settings | `pages/qh/quickyhug-viewer-settings.md` |
| Poses and Menus | `pages/qh/quickyhug-poses.md` |
| Updating to a New HUD | `pages/qh/quickyhug-update.md` |

The numbered pictures are inline SVG over images cut from the HUD textures. The images come from `docs/build_images.ps1` in the QuickyHug project; after a texture change cut them again and check the callout positions.

## Licensing

- **Jekyll theme** (`_layouts/`, `_includes/`, `css/`, `js/`, …): [MIT](licenses/LICENSE-THEME.txt), Copyright (c) 2016 Tom Johnson.
- **Navgoco sidebar component**: [BSD](licenses/LICENSE-BSD-NAVGOCO.txt).
- **Documentation text and images**: TODO.

QuickyHug is not affiliated with or sponsored by Linden Research.
