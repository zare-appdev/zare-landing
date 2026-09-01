# Zare landing page

A plain, static one-page site — no build step, no dependencies. Everything it needs is inside
this folder: `index.html`, `privacy.html`, `terms.html`, `styles.css`, and `assets/`.

Because it's fully self-contained, this whole folder can be copied straight into a brand-new,
empty repo and it will work immediately — nothing here reaches back into the rest of the Zare
app's code.

## Putting it on the internet with GitHub Pages (free)

1. On github.com, create a new repository (it can be named anything, e.g. `zare-landing`).
   It needs to be a **public** repo for free GitHub Pages hosting.
2. Copy everything inside this `landing-page` folder into that new repo, so `index.html` sits
   at the top level of the repo (not inside a subfolder).
3. Push it to GitHub (commit + push, same as any other repo).
4. In that repo on github.com, go to **Settings → Pages**.
5. Under "Build and deployment", set **Source** to "Deploy from a branch", pick the **main**
   branch and the **/ (root)** folder, then save.
6. Wait a minute or two. GitHub will give you a live URL that looks like
   `https://<your-github-username>.github.io/<repo-name>/`.

That URL is what you'll paste into App Store Connect for:
- **Privacy Policy URL** → `https://.../privacy.html`
- **Support URL** → the homepage itself, `https://.../` (it has the contact email on it)
- **Marketing URL** (optional) → same homepage

If you'd rather use your own domain name (like `zareapp.com`) instead of the `github.io`
address, that's a later, optional step — buy the domain, add a `CNAME` file to the repo with
the domain name in it, and point the domain's DNS at GitHub. Not required to launch.
