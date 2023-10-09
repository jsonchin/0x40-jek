# 0x40-jek

Forked from https://github.com/mon/0x40-web.

# Instructions for self to rebuild/deploy.

Install node.js deps.

```bash
npm install
```

Build the `dist` dir with

```bash
npx webpack
```

Copy the `./respacks` into `dist/`.

Push to the `gh-pages` branch using subtrees so the `dist/` dir is the base dir of the github page:

```bash
git add dist
git commit -m "..."
git subtree push --prefix dist origin gh-pages
```
