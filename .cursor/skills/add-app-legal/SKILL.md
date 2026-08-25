---
name: add-app-legal
description: Adds a new app's privacy policy and terms pages on this GitHub Pages site (folder, bilingual HTML, homepage card). Use when the user asks to add política de privacidade, termos e condições, PP, terms, or legal pages for another app.
---

# Add app privacy and terms

Static site. One folder per app. Copy `_templates/app/` — do not invent a new layout.

## Checklist

1. Choose a URL slug: lowercase, hyphens, no spaces (`tabela-xyz`).
2. Copy `_templates/app/` to `{slug}/`.
3. Replace every `{{…}}` placeholder in the three HTML files.
4. Write **Portuguese first**, then **English**, from the app’s real behavior (accounts, analytics, IAP, third parties, affiliation disclaimer).
5. Add a card on root `index.html` (same `card` markup as TACO / IBGE / Loterias).
6. Add a README bullet with links to the hub, privacy, and terms.
7. If the native app still points at old URLs, tell the user the public URLs:
   - `https://rodrigofranzoi.github.io/{slug}/privacy.html`
   - `https://rodrigofranzoi.github.io/{slug}/terms.html`

## Placeholders

| Token | Example |
| --- | --- |
| `{{SLUG}}` | `loterias` |
| `{{APP_NAME}}` | `Loterias Brasil` |
| `{{PLATFORMS}}` | `iOS · Android` (hub card tag on the home page) |
| `{{HUB_BLURB}}` | One sentence for the home card |
| `{{NOTICE}}` | Affiliation / “not official” disclaimer on the hub |
| `{{PRIVACY_SUMMARY_PT}}` / `_EN` | What the app stores and sends |
| `{{TERMS_SUMMARY_PT}}` / `_EN` | What the app is and is not |
| `{{UPDATED_PT}}` | `25 de agosto de 2026` |
| `{{UPDATED_EN}}` | `25 August 2026` |

Keep chrome identical to `loterias/` (shared `style.css`, lang anchors, footer). No inline `<style>`.

## Do not

- Put legal HTML at the site root except the existing IBGE redirects.
- Skip English.
- Claim official partnership unless the user confirms it.
