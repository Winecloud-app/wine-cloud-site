# Wine Cloud — public site

Static pages served via GitHub Pages from the `gh-pages` branch of
`Winecloud-app/wine-cloud`.

| Path        | Purpose                                                              |
| ----------- | -------------------------------------------------------------------- |
| `/`         | Tiny landing page (marketing URL). Links to support and privacy.     |
| `/privacy/` | App Store privacy policy (Apple-required).                           |
| `/support/` | App Store support page (Apple-required) with FAQ + support email.    |

## Hosting

- Source: this branch (`gh-pages`), root.
- Public URL (interim): `https://winecloud-app.github.io/wine-cloud/`
- Public URL (final): `https://bettonwines.co.uk/wine-cloud/` — pending DNS /
  Betton Wines site swap.
- `.nojekyll` is present so files are served verbatim (no Jekyll processing).

## Editing

These pages are intentionally hand-written HTML — no build step, no JS, no
fonts loaded over the network. Edit the HTML directly, push, and GitHub
Pages picks it up within ~60 seconds.

The brand tokens (slate-blue background `#252B3B`, gold `#c4963a`, cream
`#F5F0E6`, Georgia serif) live in `_shared.css`.

## Outstanding placeholders

- Body strings still say "Wine Cloud" — placeholder pending the rebrand
  pick on CAS-10. Sed pass at rebrand drop.
- Otherwise filled: effective date 2 May 2026, support email
  `support@bettonwines.co.uk`, data-controller line scoped to "Kris
  Cattaneo, t/a Betton Wines, York, United Kingdom" per board decision
  (sole-trader framing — Betton Wines Ltd does not exist as a UK
  registered company; Apple enrollment is Individual under Kris).
