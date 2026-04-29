# Advanced Tools

These are optional. Do not use this page until your site is already published.

The main class path is:

```text
GitHub + Antigravity + GitHub Pages
```

## VS Code
VS Code is another code editor. It is not required for this tutorial.

Use it only if you already know it or your instructor asks you to.

## GitHub Desktop
GitHub Desktop is not needed for this tutorial.

Use Antigravity Source Control for the class workflow.

## Codex
Codex can help revise code or explain files after your site is published.

Do not use it as part of the first publishing path unless your instructor asks you to.

## Claude Code
Claude Code can help with code edits after your site is published.

Some setups require terminal access, so it is not part of the beginner path.

## GitHub CLI
GitHub CLI is a terminal tool for advanced GitHub workflows.

It is not required for uploading, publishing, committing, or pushing in this tutorial.

## Issue Generation
Generated issues can help an instructor manage a larger class workflow.

Students do not need generated issues to publish their websites.

## Structure-Checking Action
This repo includes an optional GitHub Actions workflow that checks whether `index.html` is at the root of the repository.

It is a feedback tool, not a deployment tool.

The workflow can help students diagnose:

- missing `index.html`
- an extra folder layer
- files uploaded to the wrong place

## Actions-Based Pages Deployment
GitHub Pages can publish from a branch or from a GitHub Actions workflow.

For this class, use:

```text
Settings -> Pages -> Deploy from a branch -> main -> / (root)
```

Actions-based deployment is useful when a site has a build step, such as a framework or static site generator. This tutorial assumes a plain static site with files like `index.html`, `style.css`, `script.js`, and `images/`.
