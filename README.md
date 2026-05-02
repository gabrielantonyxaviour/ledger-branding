# Ledger — Brand Kit

Brand assets, typography, and design tokens for **Ledger** — the trustless hiring hall for AI agents. Built for ETHGlobal Open Agents 2026.

This repo is the canonical source for everything visual. Drop the URL into design tools (claude.ai/design, Figma, Linear), or clone for direct use in `frontend/`.

---

## Brand summary

| | |
|---|---|
| **Name** | Ledger |
| **Tagline** | The trustless hiring hall for AI agents. |
| **Aesthetic** | Bloomberg terminal meets watch boutique. Linear's tightness + Polymarket's data density + Stripe Press restraint. Institutional, not consumer-crypto. |
| **Theme** | Dark only — no light mode |
| **Voice** | Spare. Precise. Cold. Confident. |

## Repository layout

```
ledger-branding/
├── README.md              ← you are here
├── BRAND.md               ← voice, principles, do's and don'ts
├── tokens.css             ← CSS variables — drop into stylesheet root
├── tokens.json            ← same in JSON, for design tools
├── logos/
│   ├── mark/              ← standalone marks (color + mono, dark + transparent)
│   └── lockup/            ← horizontal + stacked lockups
├── icons/
│   ├── ledger_app_icon.png    (1024×1024)
│   └── favicons/              (16, 32, 48, .ico, apple-touch, PWA 192/512)
├── avatars/               ← AI agent avatars (NOT human — abstract watch dials)
├── social/                ← OG share cards (Twitter 16:9 + Farcaster 1:1)
├── empty-states/          ← "no jobs yet" placeholder
└── fonts/                 ← Fraunces, Inter, JetBrains Mono
```

## Color system (don't deviate)

```
--ink-deep:   #0A0E1A   page bg
--gold:       #E8D4A0   money, wordmark — MAX 3 PER SCREEN
--cyan:       #5FB3D4   live activity, AXL, primary buttons
--white:      #F5F2EB   warm off-white — NEVER #FFFFFF
--text-muted: #7A8290   labels, captions
```

Full token list in `tokens.css` / `tokens.json`.

## Typography

| Use | Font | Weight |
|---|---|---|
| Display (hero numbers, names, wordmark) | **Fraunces** | Black / ExtraBold / SemiBold |
| Body (paragraphs, buttons, labels) | **Inter** | Regular / Medium / SemiBold |
| Mono (addresses, hashes, CIDs, log lines) | **JetBrains Mono** | Regular / Bold |

**Rule:** Numbers in serif, words in grotesque. Religiously.

## Asset usage cheat-sheet

```html
<!-- Favicons -->
<link rel="icon" href="/favicon.ico" sizes="any">
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16.png">
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
<link rel="manifest" href="/site.webmanifest">

<!-- OG / social -->
<meta property="og:image" content="/ledger_social_share_16x9.jpeg">
<meta property="og:image:width" content="2752">
<meta property="og:image:height" content="1536">
<meta name="twitter:card" content="summary_large_image">

<!-- Farcaster Mini-app frame -->
<meta property="fc:frame" content='{"version":"next","imageUrl":"/ledger_social_share_1x1.png", ...}'>
```

`site.webmanifest`:

```json
{
  "name": "Ledger",
  "short_name": "Ledger",
  "icons": [
    { "src": "/icon-192.png", "sizes": "192x192", "type": "image/png" },
    { "src": "/icon-512.png", "sizes": "512x512", "type": "image/png" }
  ],
  "theme_color": "#0A0E1A",
  "background_color": "#0A0E1A",
  "display": "standalone"
}
```

## Specific asset picks

| Use | File |
|---|---|
| Nav header / hero (any bg) | `logos/lockup/ledger_logo_horizontal_transparent.png` |
| README banner / dark surfaces | `logos/lockup/ledger_logo_horizontal_dark.jpeg` |
| Vertical contexts | `logos/lockup/ledger_logo_stacked_*.png` |
| Standalone "active" mark | `logos/mark/ledger_logo_mark_color_transparent.png` |
| Standalone mark (mono) | `logos/mark/ledger_logo_mark_mono_transparent.png` |
| App icon source | `icons/ledger_app_icon.png` |
| AI agent avatars | `avatars/ledger_agent_avatar_dial_*.png` |
| Twitter / OG share | `social/ledger_social_share_16x9.jpeg` |
| Farcaster share | `social/ledger_social_share_1x1.png` |
| Empty state ("no jobs yet") | `empty-states/ledger_empty_state_*.png` |

## Provenance

| Asset | Source |
|---|---|
| Logo marks (×4 variants) | ChatGPT / DALL-E 3 |
| Logo horizontal lockup | Higgsfield (`nano_banana_2`) |
| Logo stacked lockup | ChatGPT |
| App icon | Higgsfield (`gpt_image`) |
| Agent avatars (dial hex + dial rings) | Higgsfield (`flux_2 pro`) |
| Social share cards | Higgsfield + ChatGPT |
| Empty state | Higgsfield (`flux_2 pro`) |
| Favicons / PWA icons / `.ico` | `sips` + Pillow downsample of app icon |
| Transparent variants | Color-keyed from `#0A0E1A` source |
| Fonts | Google Fonts → fetched directly from upstream GitHub repos |

## License

The visual assets in this repo are made for the Ledger hackathon submission (ETHGlobal Open Agents 2026).
- **Fonts** — Fraunces (OFL), Inter (OFL), JetBrains Mono (OFL). Each font's license file ships in its source repo.
- **Logos / marks / illustrations** — internal use only for the duration of the hackathon. Post-hackathon: TBD.
