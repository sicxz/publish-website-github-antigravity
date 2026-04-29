# Publish Your Existing Website with GitHub + Antigravity

A beginner-friendly tutorial for design students who already have a completed HTML/CSS website folder and need to publish it with GitHub Pages.

No GitHub Desktop. No VS Code required. No terminal required.

[Jump to tutorial start](#tutorial-start)

## Goal
Students will publish an existing website project through GitHub Pages and connect it to Antigravity for future edits.

## What you will finish
- A GitHub repository containing your website files
- An `index.html` file at the root of the repository
- A live GitHub Pages website
- A cloned copy of the repo open in Antigravity
- One small edit committed and pushed from Antigravity
- Two submission links: your repo URL and your live site URL

## The simple model
GitHub stores the site.

Antigravity edits the site.

GitHub Pages publishes the site.

## About the optional Action
This repo includes an optional GitHub Actions structure check. It checks for beginner mistakes like a missing root-level `index.html` or an extra folder layer.

It does not publish the site.

For plain static student sites, the default publishing path is still:

```text
Settings -> Pages -> Deploy from a branch -> main -> / (root)
```

Actions-based Pages deployment is better when a site has a build step or custom deployment process. This tutorial assumes a plain static site with files like `index.html`, `style.css`, `script.js`, and `images/`.

## Why this tutorial starts in GitHub
You may already have your files open in Antigravity. That is fine.

The reason this tutorial starts by uploading to GitHub is that GitHub Pages can only publish files that are in a GitHub repository. A normal folder on your computer is not public yet, even if Antigravity can edit it.

For beginners, the clearest order is:

1. Put the finished website files in GitHub.
2. Turn on GitHub Pages.
3. Clone the GitHub repo into Antigravity.
4. Use Antigravity for future edits.

This avoids the most common setup problems: uploading the wrong folder, missing `index.html`, or trying to push from a folder that is not connected to GitHub yet.

## Can I start from Antigravity instead?
Yes, but it adds more setup.

If your project is already open in Antigravity, Antigravity can help commit and push changes after the folder is connected to a GitHub repository. That usually means:

1. Git is installed on the computer.
2. The folder is a Git repository.
3. The repository has a GitHub remote.
4. You are signed in or authenticated so GitHub accepts the push.

That is a good workflow later. For this class, use the GitHub-first path below so everyone reaches a live site with fewer setup variables.

## Do I need Git installed?
For the upload and publish steps on GitHub.com, no.

For cloning, committing, and pushing from Antigravity, yes. Antigravity's Source Control features rely on Git. If Git is missing, Antigravity may ask you to install it or source control may not work correctly.

You do not need to use the terminal in this tutorial, but Git still needs to exist on the machine for local commit and push workflows.

## Will Antigravity automatically send my files to GitHub?
No. Creating or saving a file in Antigravity changes the copy on your computer.

To send changes to GitHub, use Source Control:

1. Save the file.
2. Commit the change.
3. Push or sync.

Commit saves a checkpoint. Push sends it to GitHub.

## Tutorial Start

## Before you start
You need:

- a GitHub account
- Antigravity installed
- Git installed on your computer if you will clone, commit, and push from Antigravity
- a completed project folder
- an `index.html` file

## Step 1: Check your project folder
Open your project folder before you upload anything.

Correct:

```text
project-folder/
  index.html
  style.css
  script.js
  images/
```

Wrong:

```text
project-folder/
  another-folder/
    index.html
    style.css
    script.js
```

Your `index.html` file must be at the top level of the repository. GitHub Pages needs that file as the homepage.

## Step 2: Create a new GitHub repository
1. Go to GitHub.
2. Click **New repository**.
3. Name it clearly, such as `portfolio-site` or `project-2-website`.
4. Set it to **Public**.
5. Do not add a README if you are uploading an existing project that already has files.
6. Click **Create repository**.

## Step 3: Upload the project files
1. In your new repository, click **Add file**.
2. Click **Upload files**.
3. Drag in the contents of your project folder, not the containing folder.
4. Click **Commit changes**.

> Warning: Do not upload the whole folder if it creates an extra folder layer. Your `index.html` should be visible on the first page of the repo.

## Step 4: Publish with GitHub Pages
1. Open your repository on GitHub.
2. Click **Settings**.
3. Click **Pages** in the left sidebar.
4. Under **Source**, choose **Deploy from a branch**.
5. Under **Branch**, choose `main`.
6. Under **Folder**, choose `/ (root)`.
7. Click **Save**.
8. Wait for the Pages URL to appear.

It may take a minute or two. The live URL usually looks like:

```text
https://your-username.github.io/your-repo-name/
```

## Step 5: Clone/open the repo in Antigravity
1. Go back to the main page of your GitHub repository.
2. Click the green **Code** button.
3. Copy the repository URL.
4. Open Antigravity.
5. Click **Clone Repository**.
6. Paste the repository URL.
7. Choose where to save the folder on your computer.
8. Open the cloned folder in Antigravity.

Why clone instead of just opening your old folder? Cloning gives Antigravity a local copy that is already connected to GitHub. That makes commit and push much simpler.

## Step 6: Make one small edit in Antigravity
1. Open `index.html`.
2. Edit one small line of text.
3. Save the file.
4. Open **Source Control**.
5. Write a short commit message, such as `Update homepage text`.
6. Click **Commit**.
7. Click **Push** or **Sync**.

Commit saves the change. Push sends it back to GitHub.

## Step 7: Check the live site
1. Return to your GitHub Pages URL.
2. Refresh the page.
3. Verify that your Antigravity edit appears.

If the change does not appear right away, wait a minute and refresh again.

## What to submit
Submit both links:

- GitHub repository link
- GitHub Pages live site link

## Common problems
- **I see a folder instead of `index.html`.** You probably uploaded the whole project folder. Move the files inside it to the root of the repo.
- **My Pages site is 404.** Check that Pages is set to `main` and `/ (root)`, then wait a minute or two.
- **I edited in Antigravity but GitHub did not change.** Make sure you committed and pushed.
- **Antigravity says Git is missing.** Install Git, restart Antigravity, then try cloning or Source Control again.
- **Antigravity opens my files but Source Control is empty.** You may have opened a normal folder instead of the cloned GitHub repo.
- **I committed but forgot to push.** Open Source Control in Antigravity and click **Push** or **Sync**.
- **My images are broken.** Check the image file names and folder paths.
- **My file is named `Index.html` instead of `index.html`.** Rename it to lowercase `index.html`.
- **My CSS path is wrong.** Check that the path in your HTML matches the CSS file location.

## Extra guides
- [Student checklist](docs/student-checklist.md)
- [Project structure guide](docs/project-structure.md)
- [Troubleshooting guide](docs/troubleshooting.md)
- [Optional advanced tools](docs/advanced-tools.md)
- [Instructor notes](docs/instructor-notes.md)

## For Instructors
This repo keeps the main student path intentionally narrow. Optional tools and automation notes live in the `docs/` folder so the README can stay focused on publishing the actual student project.

Platform references:

- [Google Antigravity codelab](https://codelabs.developers.google.com/getting-started-google-antigravity)
- [GitHub: Set up Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
- [GitHub Pages: Configure a publishing source](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
