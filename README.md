<p align="center">
  <img src="logo.png" alt="Key Rush logo" width="140">
</p>

<h1 align="center">Key Rush</h1>

<p align="center">
  A fast, friendly typing speed test in a single HTML file.<br>
  Built by <strong>Shubham Gautam</strong> with plain HTML, CSS and vanilla JavaScript.
</p>

<p align="center">
  <a href="https://<your-username>.github.io/key-rush/">Live demo</a> &middot;
  <a href="#run-it-locally">Run locally</a> &middot;
  <a href="#publish-on-github">Publish on GitHub</a> &middot;
  <a href="#customize-it">Customize</a>
</p>

---

## Features

- **Four difficulty levels:** Basic, Medium, Hard and Extra Hard
- **Test durations:** 15, 30, 45 or 60 seconds
- **WPM** (words per minute) and **KPM** (keystrokes per minute)
- **Live accuracy and error tracking** while you type
- **A different paragraph every attempt**, built from a large pool of sentences
- **Personal WPM history graph** with filters, plus your **personal best** overall and per level
- **Results saved in your browser** (localStorage), so they are still there next time
- **No leaderboard, no account, no database, no tracking**
- **Responsive light blue design with dark blue accents**, plus a **light / dark theme switch**
- Works offline. There are no dependencies, no build step and no external requests.

## Run it locally

You do not need to install anything.

1. Download or clone this repository.
2. Double-click `index.html`.

Or serve the folder with any static server, for example `python3 -m http.server` and open `http://localhost:8000`.

## How it works

| Metric | Meaning |
| --- | --- |
| **WPM** | Correct characters typed, divided by 5, per minute. This is the standard "net" speed. |
| **Raw WPM** | All characters typed (right or wrong), divided by 5, per minute. |
| **KPM** | Every key press per minute, including Backspace. |
| **Accuracy** | Correct key presses out of all character key presses. A mistake still counts after you fix it. |
| **Errors** | Wrong characters typed. "Left uncorrected" shows mistakes still on screen when time ended. |

Tips: the timer starts on your first key. Press **Esc** at any time to restart with a new paragraph.

## Publish on GitHub

### Option A: upload in the browser (no Git needed)

1. Sign in at [github.com](https://github.com) and click **New repository** (the **+** menu, top right).
2. Name it `key-rush`, set it to **Public**, and click **Create repository**.
3. On the new repository page click **uploading an existing file**.
4. Drag in every file from this folder: `index.html`, `README.md`, `LICENSE`, `logo.svg`, `logo.png` and `social-preview.png`.
5. Write a commit message such as `Add Key Rush` and click **Commit changes**.

### Option B: with Git

```bash
cd key-rush
git init
git add .
git commit -m "Add Key Rush"
git branch -M main
git remote add origin https://github.com/<your-username>/key-rush.git
git push -u origin main
```

### Turn it into a live website with GitHub Pages

1. In the repository open **Settings**, then **Pages**.
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Choose branch **main** and folder **/ (root)**, then click **Save**.
4. After a minute your game is live at `https://<your-username>.github.io/key-rush/`.
5. Paste that link into the "Live demo" line at the top of this README and into the repository's **About** box (the gear icon on the repository page).

### Make the repository easy to find and use

- In **About**, add a short description and topics such as `typing-test`, `wpm`, `vanilla-js`, `html`, `css`, `javascript`, `github-pages`.
- Under **Settings > General > Social preview**, upload `social-preview.png` so links to the repo show a nice card.
- Keep the `LICENSE` file so others know they are free to use and adapt the project.

## Let others use it

Because Key Rush is a single file with an MIT license, anyone can use it in three ways:

- **Play:** open your GitHub Pages link.
- **Fork:** click **Fork** on GitHub to get their own copy, then edit and publish it with their own Pages site.
- **Download:** click **Code > Download ZIP**, or copy `index.html` anywhere.

Contributions are welcome. A good workflow is: fork, create a branch, make a change, and open a pull request with a short description and a screenshot if the look changed.

## Customize it

Everything lives in `index.html`:

- **Paragraphs:** edit the `POOLS` object near the top of the `<script>`. Add your own sentences for any level. Keep them plain ASCII so every keyboard can type them.
- **Durations or levels:** change `DURATIONS` and `LEVELS`.
- **Colors:** change the CSS variables at the top of the `<style>` block. Light theme values are in `:root`, dark theme values are in `[data-theme="dark"]`.
- **Reset your own data:** use the **Clear saved results** button, or clear site data for the page in your browser.

## Privacy

Key Rush never sends anything anywhere. Your settings and results are stored only in your browser's localStorage, and clearing site data removes them.

## Credits and license

Created by **Shubham Gautam**. Released under the [MIT License](LICENSE).

The Key Rush logo is an original keycap-style K mark made for this project and is covered by the same license.
