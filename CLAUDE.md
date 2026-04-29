# InflaScoreIn_Web

Static marketing and legal pages for InflaScore (炎值), an anti-inflammatory lifestyle tracking iOS app.

## Project

- Platform: Cloudflare Pages (static, no build step)
- Output directory: `public`
- Languages: English + 中文 (separate HTML files per language)
- Remote: `git@github.com:Andylee24/InflaScoreIn_Web.git` (SSH)

## File Structure

```
public/
├── index.html / index-zh.html       ← Landing pages (EN/中文)
├── privacy.html / privacy-zh.html   ← Privacy Policy
├── terms.html / terms-zh.html       ← Terms & Conditions
├── styles.css                       ← Shared styles
└── _headers                         ← Cloudflare security headers
stitch-reference/                    ← Design reference (not deployed)
```

## Conventions

- Always update both EN and ZH versions when editing page content
- Never show technical implementation details (SwiftUI, SwiftData, iOS 17+) on public pages — use user-facing language
- Chinese pages use Noto Sans SC font, `lang="zh-CN"`
- Language switcher in nav: separate pages, not JS toggle
- Legal pages are App Store submission drafts — need counsel review before publishing
- Mobile responsive breakpoints: 1024px, 768px, 480px
