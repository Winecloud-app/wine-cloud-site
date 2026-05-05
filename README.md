# Wine Cloud — public site

Static pages served via GitHub Pages from the `main` branch of
`Winecloud-app/wine-cloud-site`.

| Path        | Purpose                                                              |
| ----------- | -------------------------------------------------------------------- |
| `/`         | Tiny landing page (marketing URL). Links to support and privacy.     |
| `/privacy/` | App Store privacy policy (Apple-required).                           |
| `/support/` | App Store support page (Apple-required) with FAQ + support email.    |

## Hosting

- Source: this branch (`main`), root.
- Public URL: `https://winecloud-app.github.io/wine-cloud-site/`
- `.nojekyll` is present so files are served verbatim (no Jekyll processing).
- All three pages carry `<meta name="robots" content="noindex,nofollow">`.
  Privacy + support are reviewer / ICO-compliance surfaces, not
  search-discovery surfaces; the landing page is also kept noindex while
  the App Store listing is the canonical surface.

## Editing

These pages are intentionally hand-written HTML — no build step, no JS, no
fonts loaded over the network. Edit the HTML directly, push, and GitHub
Pages picks it up within ~60 seconds.

The brand tokens (slate-blue background `#252B3B`, gold `#c4963a`, cream
`#F5F0E6`, Georgia serif) live in `_shared.css`.

## Authoritative values

- Effective date on `/privacy/`: 2 May 2026.
- Support email: `Support@winecloud.co.uk` (display capitalisation; SMTP is
  case-insensitive).
- Data controller: Kris Cattaneo, individual sole trader based in York,
  United Kingdom. Apple Developer enrollment is Individual under the same
  identity.
