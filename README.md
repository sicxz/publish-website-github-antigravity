# Publish Your Existing Website with GitHub + Antigravity

A beginner-friendly tutorial for design students who already have a completed HTML/CSS website folder and need to publish it with GitHub Pages.

No GitHub Desktop. No VS Code required. No terminal required.

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

## Before you start
You need:

- a GitHub account
- Antigravity installed
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
