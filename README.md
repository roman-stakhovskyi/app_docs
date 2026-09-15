# DopaSpace app documents

The privacy policies, terms and support pages the stores ask for, served by GitHub Pages so
DopaSpace apps need no domain and no backend.

Published at <https://roman-stakhovskyi.github.io/app_docs/>.

## Layout

```
index.html              every app, linked
style.css               one stylesheet for all of them
<app-name>/
  index.html            what the app is, and its documents
  privacy.html
  terms.html
```

One folder per app, named as the app is written in a URL. Adding an app is a folder and a
section in `index.html`.

## Editing

The pages are plain HTML on purpose: no build step, no generator to keep alive. A correction
is an edit and a push; GitHub Pages redeploys on its own.

Change the date at the top of a page whenever its wording changes — a policy that says when it
last moved is the only kind a store reviewer can check.

## Publishing

Settings → Pages → Source: *Deploy from a branch*, branch `main`, folder `/ (root)`.
`.nojekyll` is there so files and folders starting with an underscore are served as they are.
