# Analytics Portfolio — GitHub Pages

A responsive one-page portfolio built with plain HTML, CSS, and JavaScript. It works directly with GitHub Pages and requires no build tools.

## 1. Customize the site

Open `index.html` and replace:

- `Your Name`
- `YN` in the logo
- `YOUR_USERNAME`
- `YOUR_LINKEDIN`
- `youremail@example.com`
- Placeholder project descriptions and links
- Certification names/statuses

Open `styles.css` to change the colors at the top under `:root`.

## 2. Add your profile photo

Place your photo at:

`assets/profile.jpg`

Then replace this block in `index.html`:

```html
<div class="profile-placeholder">
  <span>Add your photo</span>
  <small>assets/profile.jpg</small>
</div>
```

with:

```html
<img class="profile-placeholder" src="assets/profile.jpg" alt="Portrait of Your Name">
```

## 3. Add your resume

Delete the placeholder `assets/resume.pdf`, then copy your real PDF into the `assets` folder using the exact name:

`resume.pdf`

## 4. Upload to GitHub

Create a repository named:

`YOUR_USERNAME.github.io`

Upload all files from this folder into the repository root.

Your repository should look like:

```text
YOUR_USERNAME.github.io/
├── index.html
├── styles.css
├── script.js
├── README.md
└── assets/
    ├── profile.jpg
    └── resume.pdf
```

## 5. Enable GitHub Pages

1. Open the repository on GitHub.
2. Select **Settings**.
3. Select **Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose the `main` branch and `/ (root)`.
6. Click **Save**.

Your website will appear at:

`https://YOUR_USERNAME.github.io`

## 6. Connect a custom domain

In **Settings → Pages**, enter your domain in **Custom domain**.

At your domain registrar, create:

- A `CNAME` record for `www` pointing to `YOUR_USERNAME.github.io`
- GitHub's required A records for the root/apex domain, if you plan to use the domain without `www`

Refer to GitHub's current custom-domain documentation before changing DNS records.

## Notes

- This template is inspired by the general dark, minimalist, long-scroll portfolio style popularized by Brittany Chiang, but it is an original implementation.
- All content is static, so the contact button opens the visitor's email app.
- No backend is required.
