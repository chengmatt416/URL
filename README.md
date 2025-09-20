# Static URL Shortener

This is a static URL shortener site deployed via GitHub Pages and mapped to your custom domain: **twtech.qzz.io**.

## How to Add a New Short URL

1. Edit `urls.json` and add a new mapping:
    ```json
    {
      "shortcode": "https://destination.url"
    }
    ```
2. Commit and push your changes to the `main` branch.
3. GitHub Actions will automatically redeploy your site.

## How Redirection Works

- Visit `twtech.qzz.io/shortcode`
- The site reads `urls.json` and redirects you to the mapped URL.

## Custom Domain Setup

- The file `CNAME` contains your custom domain.
- Make sure your DNS has a CNAME record for `twtech.qzz.io` pointing to `chengmatt416.github.io`.

## Limitations

- Mappings are static; to add or change a short URL, edit the JSON file and redeploy.
- No backend, no analytics.
