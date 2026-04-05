# JobMonkeyGO — Marketing Site

Static marketing / app-landing site for [JobMonkeyGO](https://jobmonkeygo.com), a mobile-first gig marketplace for Hong Kong.

Built with [Jekyll](https://jekyllrb.com) and [Pico CSS](https://picocss.com).

---

## Pages

| Page | URL | Description |
|---|---|---|
| Home | `/` | Hero, features overview, download links |
| Privacy Policy | `/privacypolicy/` | PDPO-compliant privacy policy |
| Terms of Use | `/termsofuse/` | Terms and conditions |
| 主頁 (ZH-HK) | `/zh-hk/` | Traditional Chinese home |
| 私隱政策 (ZH-HK) | `/zh-hk/privacypolicy/` | Traditional Chinese privacy policy |
| 使用條款 (ZH-HK) | `/zh-hk/termsofuse/` | Traditional Chinese terms of use |

---

## Local Development

### Prerequisites

- Ruby 3.x (`brew install ruby`)
- Bundler (`gem install bundler`)

### Setup

```bash
bundle install
```

### Serve with live reload

```bash
bundle exec jekyll serve --livereload
```

Site runs at `http://localhost:4000`.

### Build only (no server)

```bash
bundle exec jekyll build
```

Output is written to `_site/`.

### Quick preview without Ruby

If you just want to preview an existing build:

```bash
python3 -m http.server 4000 --directory _site
```

---

## Project Structure

```
_config.yml          # Site settings (title, URL, theme colour, i18n)
_layouts/
  default.html       # Single shared layout (header, footer, nav)
_data/
  i18n/
    en.yml           # English strings
    zh-hk.yml        # Traditional Chinese strings
assets/
  css/
    styles.css       # Base typography
    custom.css       # Layout, components, responsive styles
  img/               # App screenshots, favicon, etc.
index.md             # English homepage
privacypolicy.md     # English privacy policy
termsofuse.md        # English terms of use
zh-hk/               # Traditional Chinese pages (mirrors root structure)
```

---

## Configuration

Key settings in `_config.yml`:

| Key | Purpose |
|---|---|
| `url` | Canonical domain — must match your OAuth consent screen privacy policy URL |
| `title` | Site / app name |
| `theme_color` | Pico CSS accent colour |
| `bg_color` | `light`, `dark`, or `auto` |
| `gtag` | Google Analytics measurement ID (optional) |

---

## Deployment

The site is a plain Jekyll static build — deploy the contents of `_site/` to any static host (GitHub Pages, Netlify, Cloudflare Pages, etc.).

For GitHub Pages with a custom domain, add a `CNAME` file to the repo root containing your domain (e.g. `jobmonkeygo.com`).

---

## Related

- [JobMonkeyGO App repo](../JobMonkeyGO/) — React + Capacitor mobile app
