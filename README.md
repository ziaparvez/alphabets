# Alphabet Adventure

A self-contained, interactive alphabet-learning webpage. Press a letter to see
the letter, a matching word, and a picture. The page uses emoji pictures by
default and can optionally load your own images.

## Run locally

Open `index.html` in a modern web browser. No build tools or dependencies are
required.

## Use the page

- Press **A–Z** on the keyboard or click a letter to display it.
- The page starts with a random letter each time it is loaded.
- Press **Ctrl+Shift+E** (or **⌘+Shift+E** on Mac) to edit the displayed
  letter's word and emoji. On a touchscreen, touch and hold the page title to
  open the quick-actions menu. Edits are saved in this browser.
- Press **Ctrl+Shift+S** (or **⌘+Shift+S** on Mac) to choose which letters
  appear. The touchscreen quick-actions menu also opens these settings. Hidden
  letters are excluded from keyboard selection and the random starting letter.
  Settings are saved in this browser.
- Press **Ctrl+Shift+Enter** (or **⌘+Shift+Enter** on Mac) to toggle fullscreen.
- Other ordinary keys are ignored. Browsers may reserve some shortcuts, and
  **Escape** exits fullscreen.
- The displayed letter animates when it changes. The animation respects the
  device's reduced-motion preference.

## Use your own pictures

Choose a picture folder on the page. Image files are matched by letter or
word, without regard to capitalization. For example:

```text
pictures/
├── A.png
├── ball.jpg
├── cat.webp
└── ...
```

The supported letters are A–Z, and the matching words are listed in the page
(Apple, Ball, Cat, and so on). If no matching image is found, the page displays
the default emoji picture.

## Publish with GitHub Pages

The workflow in `.github/workflows/deploy-pages.yml` deploys the page when
changes are pushed to the `master` branch. It can also be started manually from
the repository's **Actions** tab.

To enable deployment, set the repository's Pages source to **GitHub Actions**
under **Settings → Pages → Build and deployment**.
