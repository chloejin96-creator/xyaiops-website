# XYaiops Website

Static English landing page for XYaiops, an AI-powered vulnerability lifecycle management platform.

## Files

- `index.html` - homepage content
- `styles.css` - responsive visual design
- `.nojekyll` - tells GitHub Pages to publish the static files as-is
- `CNAME.example` - template for a future custom domain file

## Publish with GitHub Pages

1. Create a GitHub repository, for example `xyaiops-website`, under `chloejin96-creator`.
2. Upload or push these files to the repository root.
3. In GitHub, open **Settings > Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.
6. After GitHub builds the site, it will be available at:
   `https://chloejin96-creator.github.io/xyaiops-website/`

For a user or organization homepage repository named `chloejin96-creator.github.io`, the site will publish at:
`https://chloejin96-creator.github.io/`

## Connect a Custom Domain

GitHub Pages supports both an apex domain such as `example.com` and a `www` subdomain such as `www.example.com`. GitHub recommends using `www` because it is the most stable custom-domain option.

When the real domain is known:

1. Commit and push the included `CNAME` file. It contains `xyaiops.com`.
2. In **Settings > Pages > Custom domain**, enter `xyaiops.com` and save.
3. Enable **Enforce HTTPS** after GitHub finishes issuing the certificate.

Recommended DNS setup:

- `www` subdomain: create a `CNAME` record pointing `www` to `chloejin96-creator.github.io`.
- Apex/root domain: create `A` records pointing `@` to GitHub Pages IPs, then let GitHub redirect between apex and `www`.

Current GitHub Pages IPv4 addresses:

- `185.199.108.153`
- `185.199.109.153`
- `185.199.110.153`
- `185.199.111.153`

Optional IPv6 `AAAA` records:

- `2606:50c0:8000::153`
- `2606:50c0:8001::153`
- `2606:50c0:8002::153`
- `2606:50c0:8003::153`

Do not include the repository name in the DNS `CNAME` target. Use `chloejin96-creator.github.io`, not `chloejin96-creator.github.io/<repo-name>`.

Also verify the domain in GitHub account settings to reduce takeover risk.

Official references:

- https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages
- https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
