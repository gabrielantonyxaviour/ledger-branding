# Ledger — Brand Voice & Principles

The non-visual side of the brand. If you're writing copy, naming a UI element, or making a judgment call about whether something fits — read this first.

## Voice

**Spare. Precise. Cold. Confident.**

Bloomberg terminal, not social app. State facts, don't sell.

| Don't | Do |
|---|---|
| "Successfully completed transaction" | "Payment landed." |
| "🎉 Your worker just won a bid!" | "Bid won." |
| "We've updated your reputation, congratulations!" | "Reputation +1." |
| "Launch your AI agent today!" | "Mint a worker. Bid on jobs. Get paid in USDC." |
| "Our amazing reputation system makes everything trustable!" | "Reputation is signed by employers. Verifiable on-chain." |

### Status message patterns (lock these)

- `[Subject] [verb-past-tense].` — "Worker accepted."
- `[Action] in [duration].` — "Payment landed in 4s."
- `[Stat] [delta].` — "Reputation +1."
- `[State] · [detail]` — "Bidding · 3 bids"

### Banned

- Exclamation marks
- Emojis
- The words: "amazing", "awesome", "sleek", "modern" (in product copy)
- "🚀" and any rocket / moon imagery
- "Successfully" (just say what happened)
- "We're thrilled to announce…"

## Visual principles

1. **Money is sacred.** Gold `#E8D4A0` appears max 3 times per screen — the single most important $ value, the wordmark, and at most one scoped earnings figure. Never on buttons. Never decorative.

2. **Cyan is the only "alive" color.** Live activity, AXL packets, primary buttons, links. Never on money. Never on static decoration.

3. **Numbers in Fraunces, words in Inter.** Religiously. Money / counts / ratings → serif. Everything else → grotesque.

4. **Tabular figures everywhere.** `font-feature-settings: 'tnum'` so `9.99` and `10.00` align.

5. **Mono for anything copy-pasteable.** Addresses, hashes, CIDs, peer IDs. Body font on a hash = reject and re-render.

6. **One bold typographic moment per screen.** Usually a single huge number or huge name in Fraunces. Don't compete with it.

7. **Density over whitespace.** Information-rich, not airy. Polymarket, not Apple marketing.

8. **No photography.** Custom geometric / cinematic / pure typography / on-chain data rendered as UI. This product is software, not lifestyle.

9. **Live data feels alive.** Subtle pulses, smooth tickers, never abrupt state changes. Respect `prefers-reduced-motion`.

10. **The iNFT is the hero.** Every worker has a visual identity. Treat avatars like watch dials — symmetrical, precise, refined. NEVER faces. NEVER robots.

## Banned visual treatments

- Gradients (anywhere, ever)
- Glassmorphism / frosted glass effects
- Drop shadows
- Glow / bloom / outer halos
- 3D effects, beveling, embossing
- Sparkle / star particles
- Rounded blob shapes
- Stat-card hero grids (lead with the primary action)
- 2×2 / 3×3 feature card grids ("bento" layouts)
- Search-icon-inside-search-bar
- Back-buttons at top of detail/new pages (use Cancel/Close in context)
- Generic placeholders ("John Doe", "Lorem ipsum", "user@example.com", "—")
- Robot heads / brain emojis for "AI agent"
- Cube / blockchain illustrations for "on-chain"
- Rocket ships / moons for "launch"

## Iconography

- **Lucide React** for utility icons only (close, search, settings, copy, external-link, chevron). Stroke 1.5, muted slate by default, white on hover.
- **Custom geometric forms** for hero / identity contexts — worker avatars (concentric rings + hex), empty states, success illustrations.
- Worker avatars look like **watch dials** — symmetrical, precise, no faces, no avatars, no emoji.

## Empty states & placeholders

- Use real-shape data, not "John Doe" / "Lorem ipsum"
- ENS names: `worker-001.<team>.eth` shape
- Addresses: real Base/0G shape (`0x742d35Cc6634C0532925a3b844Bc9e7595f0bEb1`)
- USDC values: actual USDC amounts to 2 decimals (`12,847.50 USDC`)

## When in doubt

> Bloomberg terminal, not consumer crypto. Stripe Press, not Web3 hype.

If a decision feels "amazing", "sleek", or "fun" — reconsider. Restraint is the brand.
