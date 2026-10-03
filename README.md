# .htaccess Recipes

Copy-paste Apache `.htaccess` recipes for speed, SEO, and security. Each file in `recipes/` is self-contained — drop its contents into your site's `.htaccess`.

## Recipes

| Recipe | What it does |
|---|---|
| `recipes/https-redirect.htaccess` | Forces HTTPS with a 301 redirect (keeps query strings) |
| `recipes/browser-caching.htaccess` | Long-term caching for images/fonts/CSS/JS, fresh HTML |
| `recipes/gzip-compression.htaccess` | GZIP-compresses text assets — cuts transfer size ~60–80% |
| `recipes/hotlink-protection.htaccess` | Blocks other sites hotlinking your images/files (saves bandwidth) |
| `recipes/security-headers.htaccess` | X-Frame-Options, nosniff, Referrer-Policy, hides server/PHP signatures |

## Usage

1. Back up your existing `.htaccess`.
2. Append the recipe you need (edit domain names first, e.g. in `hotlink-protection.htaccess`).
3. Test with curl: `curl -I https://yourdomain.com/`.

> **Note:** HSTS in `security-headers.htaccess` is commented out — only enable it once you are 100% sure HTTPS works everywhere on the domain.

MIT licensed.
