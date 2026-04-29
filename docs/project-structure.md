# Project Structure Guide

GitHub Pages needs `index.html` at the root of the repository.

## Correct

When you open the repo on GitHub, `index.html` is visible right away.

```text
my-website/
  index.html
  style.css
  script.js
  images/
    portrait.jpg
    background.png
```

This works because the homepage file is at the top level.

## Incorrect: Extra Folder Layer

When you open the repo on GitHub, you see a folder first.

```text
my-website/
  final-project/
    index.html
    style.css
    script.js
    images/
```

This usually happens when you upload the whole folder instead of the files inside it.

Fix it by moving these to the root:

```text
index.html
style.css
script.js
images/
```

## Incorrect: Wrong File Name

```text
my-website/
  Index.html
  style.css
```

Rename `Index.html` to `index.html`.

## Incorrect: CSS Path Does Not Match

If your HTML says:

```html
<link rel="stylesheet" href="css/style.css">
```

Then your repo needs:

```text
my-website/
  index.html
  css/
    style.css
```

If your CSS file is next to `index.html`, use:

```html
<link rel="stylesheet" href="style.css">
```
