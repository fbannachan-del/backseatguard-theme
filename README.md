# BackSeatGuard — Shopify Theme

Theme repo for **[backseatguard.com](https://backseatguard.com)** — waterproof dog car seat cover brand.

## Brand

| | |
|--|--|
| **Name** | BackSeatGuard |
| **Tagline** | Keep the dog. Protect the seats. |
| **Product** | Waterproof dog car seat hammock |
| **Vibe** | Clean, premium pet/car gear — white, near-black, one accent colour |

## Connect this repo to Shopify

1. Shopify admin → **Online Store → Themes**
2. On your theme → **…** → **Connect theme library to GitHub** (or **Add theme → Connect from GitHub**)
3. Authorize GitHub if asked
4. Select:
   - **Organization/user:** `fbannachan-del`
   - **Repository:** `backseatguard-theme`
   - **Branch:** `main`
5. Confirm connection

Shopify will sync theme files with this repo. After that, pushes to `main` update the theme (depending on your connect settings).

### Alternative: Shopify CLI

```bash
# Install once: npm i -g @shopify/cli @shopify/theme
cd backseatguard-theme
shopify theme pull --store YOUR_STORE.myshopify.com
# edit files
shopify theme push
# or: git add/commit/push if GitHub is connected
```

## Workflow with Grok / AI

1. You connect Shopify → this repo (or pull theme into this folder)
2. Share this folder as context in the session
3. Design changes are made in Liquid / CSS / JSON here
4. You push to GitHub or `shopify theme push`

## Folder layout (after theme sync)

Typical Dawn-style structure:

```
assets/          # CSS, JS, images
config/          # settings_schema.json, settings_data.json
layout/          # theme.liquid
locales/
sections/        # hero, header, featured collection, etc.
snippets/
templates/       # index.json, product.json, …
```

## Current status

- [x] GitHub repo created
- [ ] Shopify connected to this repo
- [ ] Full theme files synced (pull or Shopify push)
- [ ] Design polish (colours, hero, product cards, spacing)

## Notes

- Do **not** commit secrets (API keys, `.env`).
- Prefer editing via Git + Shopify connect, not only the online code editor, once linked.
