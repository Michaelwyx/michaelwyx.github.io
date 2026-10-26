# Yixuan Wang's homepage

This repository is the **source of the live academic homepage** at
<https://michaelwyx.github.io/>. GitHub Pages publishes the root of `main`.
It is a static HTML/CSS site: no package installation, build step, or secret is
needed to edit it. The Google Analytics measurement ID in `index.html` is a
public site identifier, not a credential.

## Where to work

- Edit `index.html`, `style.css`, and the assets under `images/` and `data/`
  here for changes to the published homepage.
- `privacy.html` describes the site's GA4 measurement. Keep it and the GA4 tag
  in `<head>` together. The property is **Yixuan Wang Homepage**
  (`G-X5J1JC9597`). GA4 reports aggregate visits and approximate geography;
  it does not expose individual visitor IP addresses.
- A separate private repository, `Michaelwyx/personal-homepage`, holds an
  **unpublished photo-gallery prototype** and older source assets. Its local
  checkout has been at `/Users/yixuanwang/Documents/Claude/Projects/homepage`.
  Do not copy its root into this repository: that would publish the gallery
  placeholders and overwrite the current analytics setup.
- The visitor-map prototype is also unpublished. The live homepage currently
  has no visitor-map section. Do not publish sample dots as real traffic.

## Publish a homepage edit

1. Fetch/pull `main` and check `git status` before editing. Preserve unrelated
   local changes.
2. Edit only the files needed. Preview `index.html` in a browser at desktop
   and phone widths when layout changes; check local asset links.
3. Run `git diff --check`, review the diff, then commit and push `main` when
   the user has authorized publication.
4. Check the latest Pages build with
   `gh api repos/Michaelwyx/michaelwyx.github.io/pages/builds/latest`, and
   verify the live URL. GitHub Pages deployment is asynchronous.

The gallery and visitor map are separate future decisions. They are currently
unpublished by user choice. If asked to publish either, confirm which sample
content should remain and distinguish it from real photos or visitor data.
