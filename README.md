# regastudios.com

The Rega Studios website: one static page (`index.html`) with no build step and nothing to install.

## Before you publish

- **Contact email:** the page uses `hello@regastudios.com`. If you want a different address, search `index.html` for `hello@regastudios.com` and change both places it appears.

## Adding the example photos and film

The Examples section shows three original photographs and the film made from them. They live in the `assets` folder; upload that folder to the repository alongside `index.html`. To change the example later, replace the files with new ones of the same names (listed in `assets/README.txt`).

## Publish on GitHub Pages

1. Create a new repository on GitHub, for example `regastudios-site`.
2. Upload `index.html` and `CNAME` to the root of the repository. Use **Add file → Upload files**, then **Commit changes**.
3. Go to **Settings → Pages**.
   - Under **Source**, choose **Deploy from a branch**.
   - Select the `main` branch and the `/ (root)` folder, then **Save**.
4. In the same Pages settings, check that **Custom domain** shows `regastudios.com`. The `CNAME` file sets it automatically.

## Point your domain at GitHub

Add these records at the company where regastudios.com is registered (GoDaddy, Namecheap, Google/Squarespace, and so on).

| Type  | Name / Host | Value                     |
|-------|-------------|---------------------------|
| A     | @           | 185.199.108.153           |
| A     | @           | 185.199.109.153           |
| A     | @           | 185.199.110.153           |
| A     | @           | 185.199.111.153           |
| CNAME | www         | YOUR-GITHUB-USERNAME.github.io |

Remove any old A or CNAME records for `@` and `www` that point somewhere else.

DNS changes can take from a few minutes up to a day to take effect. Once GitHub confirms the domain, go back to **Settings → Pages** and tick **Enforce HTTPS**.

## Updating the site

Edit `index.html` on GitHub (open the file and click the pencil icon), then commit. The live site updates within a minute or two.
