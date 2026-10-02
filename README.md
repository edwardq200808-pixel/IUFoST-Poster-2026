# Conference Poster Author Website

A simple responsive website for visitors who scan a QR code on your conference poster.

## Open in VS Code

1. Download and unzip this folder.
2. Open VS Code.
3. Choose **File > Open Folder**.
4. Select `conference_poster_author_site`.
5. Open `index.html`.
6. For the easiest preview, install the VS Code extension **Live Server**.
7. Right-click `index.html` and choose **Open with Live Server**.

You can also simply double-click `index.html` and open it in a browser.

## Files

- `index.html` – page content
- `styles.css` – layout and visual design
- `script.js` – mobile navigation and automatic footer year

## What to replace first

Search `index.html` for:
- `Your Poster Title Goes Here`
- `Conference Name 2026`
- `Poster No. XX`
- `Author Two`
- `Author Three`
- `Author Four`
- `your.email@example.com`
- all `href="#"` placeholders

## Author photos

The starter version uses initials so it works immediately.

To use profile photos instead, replace:

```html
<div class="avatar avatar-1" aria-hidden="true">GH</div>
```

with:

```html
<img class="avatar" src="images/guanqiu-huang.jpg" alt="Guanqiu Huang" />
```

Then create an `images` folder and place the photo inside.

## Add LinkedIn and ORCID links

Example:

```html
<div class="link-row">
  <a href="https://www.linkedin.com/in/USERNAME/" target="_blank">LinkedIn</a>
  <a href="https://orcid.org/0000-0000-0000-0000" target="_blank">ORCID</a>
  <a href="mailto:name@university.edu">Email</a>
</div>
```

## Add your poster image

Replace the `.poster-placeholder` block in `index.html` with:

```html
<img class="poster-image" src="images/poster.jpg" alt="Conference poster" />
```

Then add to `styles.css`:

```css
.poster-image {
  width: 100%;
  display: block;
}
```

## Add your poster PDF

Place `poster.pdf` in the project folder and add:

```html
<a href="poster.pdf" target="_blank">View poster PDF</a>
```

## Publishing free

Good simple options:
- GitHub Pages
- Netlify
- Cloudflare Pages

Once published, generate a QR code using the final website URL and place it on your poster.
