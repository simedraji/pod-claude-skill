# Automation & Finance for POD Sellers

## Automation stack

| Tool | Best for |
|---|---|
| **n8n** | Self-hosted, highly flexible automation — good fit for a technical seller (matches Med's background in smart-control-systems/JARVIS-style assistants); ideal for connecting AI APIs (OpenRouter/Claude) to POD workflows |
| **Zapier** | Easiest no-code automation, large app library, good for beginners |
| **Make (Integromat)** | Visual, more powerful branching logic than Zapier, still no-code |
| **Obsidian / Notion** | Personal knowledge base + course content management (matches the structure of the uploaded POD Master Hub) |

### Common POD automation blueprints to teach
1. **Niche/keyword research pipeline**: scraper or API pull (EverBee/eRank export) → AI summarization (Claude/ChatGPT) → auto-populate a spreadsheet/Notion database of validated niches.
2. **Design-to-listing pipeline**: AI design generation → auto-upload to Printify/Printful → AI-generated SEO title/tags/description → auto-publish to Etsy/Shopify.
3. **Order/zabon (زبون) support pipeline**: incoming customer message (Etsy/Shopify/TikTok) → AI draft reply → human approval → send. Useful for a JARVIS-style assistant since it keeps a human in the loop for quality control.
4. **Social content pipeline**: trending audio/topic detection → AI script generation → ffmpeg-based video assembly → scheduled posting.

## Payment providers (relevant for Morocco-based sellers)

| Provider | Notes |
|---|---|
| **Payoneer** | Most widely supported for receiving Etsy/Amazon/marketplace payouts in Morocco; multi-currency receiving accounts |
| **Wise** | Good for low-fee currency conversion and holding multiple currencies; check current Morocco-specific account support before relying on it for a course module, as supported countries/features change |
| **PayPal** | Widely accepted by buyers but historically more limited for direct withdrawal in Morocco — confirm current status, this has shifted over time |
| **Stripe** | Needed for some Shopify payment setups; availability/limitations vary by country — verify current Morocco support before teaching as a default |

*Always verify current country support/fees with a quick search before presenting these as fixed facts in a course — payment-provider availability for Morocco changes periodically.*

## Pricing & margin math (teach this before any platform-specific fee module)

```
Retail Price = COGS + Platform Fees (%) + Shipping Cost (if not bundled) + Target Margin
```

- **COGS** = base product cost from supplier (Printify/Printful/Gelato) + their fulfillment/shipping charge to you.
- **Platform Fees**: Etsy ≈ 11–15% baseline (more with Offsite Ads); TikTok Shop ≈ 20–35% effective (commission + referral fee + returns). See `marketplace-fees-affiliate.md`.
- **Target Margin**: recommend students aim for 30–40%+ net margin after all fees and COGS, especially early on while volume is low and ad spend is untested.

## Finance & KPI tracking — minimum dashboard for a POD shop
- Revenue by platform (Etsy / Shopify / TikTok Shop)
- COGS and fee load by platform (track separately — they differ a lot)
- Net margin per product/niche (kills products that look like best-sellers by revenue but are losing money after TikTok Shop's effective 25–35% cost)
- Ad spend / commission spend vs. resulting revenue (ROAS) per channel
- Monthly/quarterly review cadence — matches the user's existing Obsidian structure (Weekly/Monthly/Quarterly Review notes)

## SOP/checklist template (for PODAcademy lesson handouts)
1. Niche validated (search volume + competition + willingness to pay checked)
2. 10–15 designs created per niche, IP-safety checked
3. Listings published with 2026-compliant SEO (title/tags/photos/video/shipping price)
4. Pricing math run against target margin before publishing
5. Pinterest/TikTok organic content scheduled
6. TikTok Shop affiliate program configured (commission rate modeled against effective cost, not sticker rate)
7. Weekly KPI review against the dashboard above
