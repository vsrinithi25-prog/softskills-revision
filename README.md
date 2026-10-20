# Essential Communication & Social Skills III — Revision

A small, mobile-friendly revision site built with plain HTML, CSS and JavaScript. It works without a build step and can be published with GitHub Pages.

## What is included

- Five expandable unit cards with key ideas and quick-revision prompts.
- Searchable vocabulary and commonly confused words.
- Shuffled multiple-choice quiz sets, scoring, mistake review and up to 30 saved attempts.
- A local notes search helper. It is rule-based search, not AI, and only searches the text included in `app.js`.
- Responsive layout and offline-friendly core functionality.

## Source and accuracy note

The referenced conversation preview available while preparing this project did not include the actual syllabus index, unit notes, vocabulary list or readable transcription of the scanned previous-year paper. The included five topics and revision text are therefore a **general starter set**, not verified course notes. Check the unit titles and facts against your syllabus and replace or extend the data in `app.js` before relying on it for an exam.

The conversation refers to a previous-year paper, but no paper questions or verified details were accessible. No question is represented here as coming from that paper. Any paper details supplied later should be labeled **reported / unverified** unless the scan is legible and has been checked against the source.

## Open locally in VS Code

1. Download or clone this project folder to your computer.
2. In VS Code, choose **File → Open Folder…** and select the folder containing `index.html`, `styles.css` and `app.js`.
3. Open `index.html` in a browser. You can also install the VS Code **Live Server** extension, right-click `index.html`, and choose **Open with Live Server** for a local preview.
4. No sign-in, server, package installation or build command is needed.

## Publish with GitHub Pages

1. Sign in to GitHub and create a new **public repository** (for example, `soft-skills-revision`). Do not initialize it with a README if you will be pushing this folder as-is.
2. In VS Code, open the project folder. Open **Terminal → New Terminal**.
3. Run these commands, replacing `YOUR-USERNAME` with your GitHub username and `soft-skills-revision` with your repository name:

   ```sh
   git init
   git add .
   git commit -m "Create revision website"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/soft-skills-revision.git
   git push -u origin main
   ```

   If Git asks you to authenticate, complete the browser sign-in flow. GitHub no longer accepts an account password for Git over HTTPS.

4. On GitHub, open the repository and go to **Settings → Pages**.
5. Under **Build and deployment**, select **Deploy from a branch**. Choose branch **main** and folder **/(root)**, then save.
6. Wait for Pages to publish. The site link will be `https://YOUR-USERNAME.github.io/soft-skills-revision/`. It can take a few minutes to appear.
7. After edits, save in VS Code and run `git add .`, `git commit -m "Update revision content"`, and `git push`. Pages republishes the pushed changes.

For a personal site repository named `YOUR-USERNAME.github.io`, the URL is `https://YOUR-USERNAME.github.io/` instead.

## Personal data and browser storage

Quiz history is stored in the browser's `localStorage` on the device where the quiz is taken. It is not synced across devices, accounts or browsers. Clearing site data removes it. The Ask helper runs locally. Google sign-in and cloud sync are not included.

## Editing the course content

Open `app.js`. The `units` array contains each unit's title, summary, points and quick prompt. The `vocab` array contains searchable terms. The `questions` array contains quiz questions, choices, correct-choice index and answer explanation. Keep each correct index aligned with its choice array.
