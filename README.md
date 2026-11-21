# Docs-as-Code Starter

A tiny static website built with HTML, CSS and JavaScript, used to practise the docs-as-code workflow: raising an issue, updating documentation on a branch, and merging it through a pull request. The page has a demo button that updates a status message and a small mock API (`window.fakeApi`) you can call from the browser console.

## Installation and setup

1. Clone the repository:
   ```
   git clone https://github.com/walkinsrenaldo/docs-as-code-starter.git
   ```
2. Open the project folder:
   ```
   cd docs-as-code-starter
   ```
3. Open `index.html` in a web browser. No installs or build steps are needed.
   (Optional: use the VS Code "Live Server" extension.)

## Usage

1. Open `index.html` in your browser. The page shows **Status: ready**.
2. Click the **Click me** button. The status text changes to **Status: clicked at** followed by the exact time of your click, down to the second.
3. Try the mini API: open the browser console (right-click the page, choose **Inspect**, then the **Console** tab) and run:
   ```js
   window.fakeApi.ping("hello")
   ```
   It returns an object like this:
   ```js
   { ok: true, echo: "hello", timestamp: "2026-11-21T03:10:51.952Z" }
   ```
   - `ok`: `true` when the call succeeds
   - `echo`: the message you passed in
   - `timestamp`: the time of the call (UTC, ISO format)

## Contribution guidelines

1. **Raise an issue first.** Every new feature, bug fix or documentation change must be created as a GitHub Issue before work starts.
2. **Use a branch.** Never commit directly to `main`. Name branches after the work, e.g. `feature/add-form` or `docs/readme-update`.
3. **Write clear commits.** Use short, descriptive messages, e.g. `docs: update README`.
4. **Open a pull request.** When your work is done, open a PR from your branch into `main`.
5. **Link the issue.** Any PR that resolves an issue must state `Closes #issue-number` in its description.
6. **Review before merging.** At least one other team member should review the PR before it is merged.
7. **Confirm closure.** After merging, check that the linked issue was closed automatically.