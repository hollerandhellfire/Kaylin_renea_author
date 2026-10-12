# Kaylin Renea — Author Page

The official author page for **Angela Kay Smith, writing as Kaylin Renea**, author of the Holler & Hellfire Universe.

Published by **WEBBS Entrepreneurship**.

---

## What's on the page

The page is a single scrolling site with six sections, in this order:

1. **Hero** — solo author portrait, pen name, and the series tagline ("the corridors are open")
2. **About** — the author bio and a "Field record" quick-facts card
3. **The Books** — covers and one-line hooks for Books 1–6, each paired with its track from the album *REFLECTION*, plus Book 6B (*Kasdeja & Velvet*) as the bridge to the Expansion Arc
4. **The Heart of the Series** — the series theme ("a relationship built on trust and belief") beside the H&H seal
5. **The Publisher** — WEBBS Entrepreneurship credits with the duo photo
6. **Support** — a button linking to the Holler & Hellfire GoFundMe

The page works on phones, tablets, and desktops. The ember animation in the hero turns itself off for visitors who have "reduce motion" turned on.

---

## Files

```
site/
├── index.html            The whole page: content, styles, and the ember animation
├── README.md             This file
└── img/
    ├── kaylin-portrait.jpg   Hero portrait (solo)
    ├── webbs-duo.jpg         Kaylin Renea and Brian Lee Webb
    ├── hh-seal.jpg           Gold H&H seal with ravens
    ├── cover-b1.jpg          Fallin' for a Fallen
    ├── cover-b2.jpg          The Devil's in the Details
    ├── cover-b3.jpg          Strike Me Down
    ├── cover-b4.jpg          All Hell Breaks Loose
    ├── cover-b5.jpg          Written in the Stars
    ├── cover-b6.jpg          Outlaw Heaven
    └── cover-b6b.jpg         Kasdeja & Velvet
```

All images are compressed JPEGs. Covers are 600 × 957 pixels. Photos are 1000 × 1250 pixels. The whole site is about 1.4 MB.

---

## Hosting the site yourself (Netlify or GitHub Pages)

The page is currently published as a Claude artifact. That host adds the opening HTML tags automatically, so `index.html` starts at the `<title>` line. **Before you upload it anywhere else, add the opening and closing tags.**

### Step 1: Add the page wrapper

1. Open `index.html` in any text editor.
2. Paste these lines at the very top, above `<title>`:

```html
<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<meta name="description" content="Kaylin Renea, author of the Holler & Hellfire Universe: Appalachian Gothic romance from Pike County, Kentucky.">
```

3. Find the line `</style>` and paste these two lines right after it:

```html
</head>
<body>
```

4. Paste these lines at the very bottom of the file:

```html
</body>
</html>
```

5. Save the file.

### Step 2a: Deploy on Netlify (easiest)

1. Go to **app.netlify.com** and sign in.
2. Open **Sites**, then choose **Add new site → Deploy manually**.
3. Drag the whole `site` folder onto the upload box.
4. Netlify gives you a live link in under a minute.
5. To use your own domain, open **Domain settings** and add it there.

### Step 2b: Deploy on GitHub Pages

1. Create a new repository on GitHub (for example, `kaylin-renea-author-page`).
2. Upload everything inside the `site` folder, keeping the `img` folder as it is.
3. Open the repository's **Settings → Pages**.
4. Under **Source**, choose **Deploy from a branch**, pick `main`, and choose the `/ (root)` folder.
5. Click **Save**. Your link appears at the top of that page within a few minutes.

---

## How to make common edits

All edits happen in `index.html`. Use your editor's Find feature (Ctrl+F or Cmd+F) to jump to the text below.

| To change… | Search for… | What to do |
|---|---|---|
| The bio | `Kaylin Renea is the pen name` | Edit the four paragraphs inside `<div class="letter">` |
| The quick-facts card | `Field record` | Each fact is one `<div class="row">` line |
| A book's hook | The book's title, such as `Strike Me Down` | Edit the text inside `<p class="hook">` |
| A book's soundtrack line | `On <i>REFLECTION</i>` | Change the track name inside `<b>` |
| A book cover | `cover-b1.jpg` (and so on) | Replace the image in `img/` using the same file name |
| The GoFundMe link | `gofund.me` | Replace the web address |
| The footer | `&copy; 2026` | Edit the two lines in `<footer>` |

### Swapping a photo or cover

1. Save the new image as a JPEG.
2. Keep the same shape: covers are tall (about 5 × 8), portraits are 4 × 5.
3. Keep the file under about 300 KB so the page stays fast.
4. Give it the exact same file name as the old one and replace it in `img/`.

### Changing the colors

The colors are set once near the top of `index.html`, inside `:root`. Change a value there and it updates everywhere on the page.

| Name | Used for | Current color |
|---|---|---|
| `--coal` | Page background | Near-black brown `#100b08` |
| `--hearth` | Raised panels | Dark hearth brown `#1a120d` |
| `--seam` | Borders and lines | Burnt umber `#3a2718` |
| `--bone` | Main text | Warm bone `#efe4d0` |
| `--ash` | Small labels | Ash tan `#a8977f` |
| `--brass` | Buttons and names | Engraved brass `#c9a46a` |
| `--ember` | Fire highlights | Ember orange `#e0762a` |

### Fonts

The fonts load free from Google Fonts. No download or license is needed.

- **IM Fell English SC** — headings and the pen name
- **Crimson Pro** — body text
- **Special Elite** — typewriter-style labels

---

## Before sharing the link

- [ ] **Check the bio.** It was drafted from the series bibles and still needs Angela's review.
- [ ] **Hometown.** No hometown is listed yet. Add one to the bio and the quick-facts card if wanted.
- [ ] **Contact email.** No email is on the page yet. Add one to the Support section if wanted.
- [ ] **Buy links.** The books don't have store links yet. Add Amazon or other retailer links once they are live.
- [ ] **Sharing.** The Claude artifact is private until it is shared from its Share menu.

---

## Canon notes

The book order, couples, and hooks match the H&H series bible and the H&H Universe Timeline:

| Book | Title | Couple | *REFLECTION* track |
|---|---|---|---|
| 1 | Fallin' for a Fallen | Dixie & Azazel | Before the Compact |
| 2 | The Devil's in the Details | Della & Samyaza | What the Ground Keeps |
| 3 | Strike Me Down | Carla June & Baraqiel | Tuesday Special |
| 4 | All Hell Breaks Loose | Mercy & Armaros | Spell-Breaker |
| 5 | Written in the Stars | June & Kokabiel | Every Star I Named |
| 6 | Outlaw Heaven | Ensemble, five couples | Outlaw Heaven |
| 6B | Kasdeja & Velvet | Velvet Thornbloom & Kasdeja | — |

If a title, couple, or track changes in the canon bibles, update this table and the matching book card in `index.html`.

---

## Credits

- **Brian Lee Webb** — CEO and Founder, WEBBS Entrepreneurship
- **Angela Kay Smith, writing as Kaylin Renea** — Author, Holler & Hellfire Universe

© 2026 WEBBS ENTREPRENEURSHIP. Holler & Hellfire™ and Kaylin Renea™. All rights reserved.
