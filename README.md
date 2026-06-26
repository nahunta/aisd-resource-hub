# AISD TEA Takeover Resource Hub

A public-facing community resource hub tracking the potential TEA (Texas Education Agency) takeover of Austin ISD.

**Live site:** Hosted on GitHub Pages from the `main` branch root.

---

## Adding a New Organization

Find this comment in `index.html` inside the `.card-grid` div:

```html
<!-- ORG CARD — duplicate this block to add a new organization -->
<div class="org-card">
  <p class="org-card-name">Stop Austin Takeover</p>
  <a class="org-card-link" href="http://stopaustintakeover.org" target="_blank" rel="noopener noreferrer">
    Visit →
  </a>
</div>
<!-- END ORG CARD -->
```

Copy the entire block (from `<!-- ORG CARD -->` to `<!-- END ORG CARD -->`), paste it after the last existing card, and update:
1. The text inside `<p class="org-card-name">` — the organization name
2. The `href` attribute on the `<a>` tag — the URL

---

## Adding a New Article

Find this comment in `index.html` inside the `.article-list` div:

```html
<!-- ARTICLE — duplicate this block to add a new article -->
<a
  class="article-card"
  href="https://example.com/article"
  target="_blank"
  rel="noopener noreferrer"
>
  <div>
    <p class="article-title">Article Title Here</p>
    <p class="article-source">Publication Name</p>
  </div>
  <span class="article-arrow" aria-hidden="true">→</span>
</a>
<!-- END ARTICLE -->
```

Copy the block, paste it after the last existing article, and update:
1. The `href` — the article URL
2. The text inside `<p class="article-title">` — the article headline
3. The text inside `<p class="article-source">` — the publication name

---

## Enabling GitHub Pages

In the repository settings on GitHub:
- Go to **Settings → Pages**
- Set **Source** to `Deploy from a branch`
- Set **Branch** to `main`, folder `/` (root)
- Save — the site will be live at `https://<username>.github.io/<repo-name>/`
