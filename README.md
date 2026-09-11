# Filippo Ricci — Academic Homepage

This folder contains a simple static website. You do not need any special software to edit it.

## Files

- `index.html` — all the written content and page structure.
- `style.css` — visual appearance: spacing, typography, colours and mobile layout.
- `Filippo_Ricci_CV.pdf` — the CV linked from the homepage.

## How to preview the site

The simplest method is to double-click `index.html`. It will open in your browser.

If the browser blocks local PDF links, start a small local server instead:

1. Open a terminal inside this folder.
2. Run `python3 -m http.server 8000`.
3. Open `http://localhost:8000` in the browser.

## How to edit text

Open `index.html` in a text editor such as Visual Studio Code.

Most visible text is written directly between HTML tags. Example:

```html
<h2>Private mathematics tutoring</h2>
<p>I offer individual tutoring...</p>
```

Change only the text between the opening and closing tags.

## How to update the CV

Export your latest CV as PDF, name it `Filippo_Ricci_CV.pdf`, and replace the old PDF in this folder.

## How to add a testimonial

Find the section with `id="feedback"` in `index.html`.
Replace the empty-state card or add a new block like this:

```html
<blockquote class="card">
  <p>“Filippo explains difficult ideas clearly and prepares useful exercises.”</p>
  <footer>— First name, Analysis I student</footer>
</blockquote>
```

Only publish real reviews for which the student has agreed to publication.

## How to change colours

At the very top of `style.css` there is a block called `:root`.
The main site colour is controlled by:

```css
--accent: #244a73;
```

Change the hexadecimal value to another colour if desired.

## Publishing with GitHub Pages

1. Create a free GitHub account if you do not already have one.
2. Create a new repository, for example `filipporicci.github.io`.
3. Upload the three website files to the repository.
4. In the repository, open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select the `main` branch and `/root`, then save.
7. GitHub will publish the site at `https://filipporicci.github.io` if that repository name is available for your account.

If you choose a different repository name, GitHub Pages will show you the final site address in the Pages settings.

## Recommended future additions

- Professional photo.
- ORCID once useful for publications.
- GitHub link when your programming projects are ready to show.
- Publications / preprints section when available.
- Talks and conferences section.
- A dedicated tutoring form, e.g. Google Forms, if tutoring activity grows.
