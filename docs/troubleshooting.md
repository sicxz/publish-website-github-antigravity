# Troubleshooting

## Problem
I see a folder instead of `index.html`.

## Cause
You probably uploaded the whole project folder. GitHub Pages needs `index.html` at the root of the repo.

## Fix
Open the folder in GitHub, move `index.html`, `style.css`, `script.js`, and `images/` to the root, then delete the empty extra folder.

## Problem
My Pages site is 404.

## Cause
GitHub Pages may not be enabled yet, it may still be publishing, or `index.html` may be in the wrong place.

## Fix
Go to **Settings** -> **Pages**. Set **Source** to **Deploy from a branch**, **Branch** to `main`, and **Folder** to `/ (root)`. Save, wait a minute or two, then refresh the live URL.

## Problem
I edited in Antigravity but GitHub did not change.

## Cause
Saving a file only changes your local copy. GitHub changes after you commit and push.

## Fix
Open **Source Control** in Antigravity. Commit the change, then click **Push** or **Sync**.

## Problem
I committed but forgot to push.

## Cause
The change is saved locally, but it has not been sent back to GitHub.

## Fix
Open **Source Control** in Antigravity and click **Push** or **Sync**. Then check the file on GitHub.

## Problem
My images are broken.

## Cause
The image path in your HTML or CSS does not match the real file name or folder.

## Fix
Check spelling, capitalization, and folders. If your file is `images/photo.jpg`, your HTML should use `images/photo.jpg`.

## Problem
My file is named `Index.html` instead of `index.html`.

## Cause
GitHub Pages expects the homepage file to be named `index.html` for this tutorial.

## Fix
Rename the file to lowercase `index.html`, commit the rename, and push.

## Problem
My CSS path is wrong.

## Cause
The `href` in your HTML does not match where your CSS file actually lives.

## Fix
If `style.css` is next to `index.html`, use:

```html
<link rel="stylesheet" href="style.css">
```

If `style.css` is inside a `css` folder, use:

```html
<link rel="stylesheet" href="css/style.css">
```
