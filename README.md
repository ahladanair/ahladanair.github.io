# Ahlad Nair — Portfolio Website

A single-page, clean & minimal portfolio site. Everything (HTML, CSS, JS) lives in one file: `index.html`. That makes it easy to upload and edit on GitHub even if you're new to it.

## 1. Put it on GitHub

1. Go to [github.com](https://github.com) and log in (create a free account if you don't have one).
2. Click the **+** icon (top right) → **New repository**.
   - Name it either:
     - `yourusername.github.io` → this makes your site live at `https://yourusername.github.io` (use your *exact* GitHub username), **or**
     - anything else, like `my-portfolio` → this makes your site live at `https://yourusername.github.io/my-portfolio`
   - Set it to **Public**.
   - Click **Create repository**.
3. Click **Add file → Upload files**, then drag in `index.html`.
4. Click **Commit changes**.

## 2. Turn on GitHub Pages

1. In your repo, go to **Settings → Pages** (left sidebar).
2. Under "Build and deployment", set **Source** to `Deploy from a branch`.
3. Set **Branch** to `main` and folder to `/ (root)`. Click **Save**.
4. Wait about a minute, then refresh — GitHub will show you the live URL at the top of that page.

## 3. Connect the contact form (Formspree — free, no coding)

Your form is already wired up in the code, it just needs your own form ID:

1. Go to [formspree.io](https://formspree.io) and sign up for free.
2. Click **New Form**, name it (e.g. "Portfolio Contact"), and confirm your email.
3. Formspree gives you a URL like `https://formspree.io/f/abcdwxyz`.
4. Open `index.html`, find this line near the bottom:
   ```html
   <form id="contactForm" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
5. Replace `YOUR_FORM_ID` with your actual ID (e.g. `abcdwxyz`), save, and re-upload to GitHub.

Messages people send through your site will now land straight in your inbox.

## 4. Things to personalize

Open `index.html` in any text editor (or right on GitHub using the pencil ✏️ icon) and update:

- **Your photo**: replace the circular "AN" placeholder — swap the `<div class="avatar">...</div>` block for an `<img src="your-photo.jpg" ...>` tag (upload the image to the repo first).
- **Bio text**: the two paragraphs under "About."
- **Projects**: each card's title, description, and the "Add screenshot" thumbnail (same idea — swap in an `<img>` tag).
- **Gallery photos**: same approach for each `+ Add photo` box.
- **Social links**: your real email, Instagram, LinkedIn, GitHub in the Contact section.

No need to touch the CSS unless you want to change colors or layout — the design is complete and responsive on mobile as-is.
