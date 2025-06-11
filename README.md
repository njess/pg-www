# Proof Group Website

This repository contains the static files for the Proof Group website. It is designed to be hosted using [GitHub Pages](https://pages.github.com/).

## Hosting on GitHub Pages

1. **Create a repository** on GitHub and push the contents of this project to the `main` branch.
2. In the repository **Settings**, navigate to **Pages**.
3. Select the `main` branch as the source and keep the root folder (`/`) for the site content.
4. Save the settings. GitHub will build the site and provide a public URL in the form `https://<username>.github.io/<repository>/`.

Once the build completes, visiting that URL will serve `index.html` from the repository.

## Using a Custom Domain

1. Create a file named `CNAME` in the repository root that contains only your custom domain, for example:

   ```
   example.com
   ```

2. Commit and push the `CNAME` file to the `main` branch. GitHub Pages will automatically use the domain in this file.
3. Update your domain's DNS records:

   - If you are using an **A record**, point it to GitHub's servers:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - Alternatively, create a **CNAME record** pointing your domain to `<username>.github.io`.

4. After the DNS changes propagate, the custom domain will load your site. You can also enable HTTPS in the Pages settings once the domain is configured.

## Directory Structure

- `index.html` – Main landing page
- `writing/` – Articles and other long-form content
- `img/` – Images used on the site

## Adding or Updating Content

All pages are plain HTML. Simply edit the files and commit the changes to update the website. Images placed in the `img/` directory can be referenced by relative path.

---

For additional details about custom domains and GitHub Pages, see the official [GitHub Pages documentation](https://docs.github.com/en/pages).
