# The Abbecue, website

The single-page site for The Abbecue. It is one self-contained file, `index.html`, so it can be hosted anywhere with no build step. The only external resource is the Google Fonts stylesheet, which loads automatically over the internet.

## Publish with GitHub Pages

GitHub Pages gives the site a public web address that works on any device, including phones, at no cost.

### Option A, through the GitHub website (no terminal)
1. Sign in at github.com and choose New repository.
2. Name it `abbecue-website`, set it to Public, and create it.
3. On the repository page choose Add file, then Upload files.
4. Drag in `index.html` and `.nojekyll` from this folder, then Commit.
5. Open Settings, then Pages.
6. Under Build and deployment, set Source to Deploy from a branch, Branch to `main`, folder `/ (root)`, and Save.
7. Wait one to two minutes. The address appears at the top of the Pages screen.

Your address will look like:
`https://<your-username>.github.io/abbecue-website/`

### Option B, with Git on your computer
```
cd "abbecue-website"
git init
git add .
git commit -m "Publish The Abbecue website"
git branch -M main
git remote add origin https://github.com/<your-username>/abbecue-website.git
git push -u origin main
```
Then enable Pages in Settings as in steps 5 to 7 above.

## Custom domain (abbecue.com), optional
1. Add a file named `CNAME` to the repository containing one line: `www.abbecue.com`.
2. At your domain registrar, add a CNAME record for `www` pointing to `<your-username>.github.io`, and the four GitHub A records for the apex domain.
3. In Settings, Pages, enter the custom domain and enable Enforce HTTPS once it validates.

## Files
- `index.html`, the complete website.
- `.nojekyll`, tells GitHub Pages to serve the files as is.
