# anfisacullins.com

A single-page static site with no build step. To preview it, open `index.html` in a browser.

- `index.html`: the whole site, including its styles
- `resume/AnfisaCullins_Resume.pdf`: the resume the "Download resume" buttons link to
- `CNAME`: tells GitHub Pages to serve the site at anfisacullins.com

## Publish on GitHub Pages (free)

1. Create a public GitHub repository, for example `anfisacullins.com`, and upload everything in this folder.
2. In the repository, go to Settings → Pages → Source: "Deploy from a branch", choose `main` and `/ (root)`, then Save.
3. In Namecheap, go to Domain List → anfisacullins.com → Advanced DNS and add these records:
   - Four **A records**, each with host `@`, one for each of: 185.199.108.153, 185.199.109.153, 185.199.110.153 and 185.199.111.153
   - One **CNAME record** with host `www` and value `<your-github-username>.github.io`
   - Remove the default Namecheap parking records.
4. Back in Settings → Pages, enter `anfisacullins.com` as the custom domain. Once the certificate is ready, tick "Enforce HTTPS". DNS changes can take a few hours to take effect.
