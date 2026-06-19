# Design Tools & AI Prompt Library

## Tool stack

| Tool | Use |
|---|---|
| **Canva** | Fast mockups, listing images, size charts, beginner-friendly design |
| **Photoshop / Illustrator / Affinity Designer** | Professional vector/raster design, print-ready files (300 DPI, correct color profile) |
| **Kittl** | Print-ready artwork + design variants, popular specifically in the POD community for fast text-based designs |
| **Midjourney / Ideogram / Flux / Leonardo AI** | AI image generation for illustration-style designs — always check output for accidental resemblance to copyrighted characters/logos before listing |
| **ChatGPT / Claude / DeepSeek / Gemini / Grok** | Copywriting (titles, tags, descriptions), niche brainstorming, design brief generation |
| **Mockey AI / Print2Social** | Auto-generate extra product mockups and repeatable social promo posts |

## Design principles to teach
- **300 DPI minimum**, transparent PNG for apparel, correct safe-print-area per product type (varies by supplier — always check the specific platform's template).
- **Typography**: one "hero" font (bold, personality-driven) + one support font (clean, readable) — avoid using 3+ fonts in one design.
- **Color**: 2–3 colors max for apparel (keeps print cost down on some suppliers and reads better at small thumbnail size); home decor/posters can use a fuller palette.
- **IP/copyright safety**: never use copyrighted characters, sports league logos, brand names, or song lyrics in designs — this is the #1 cause of takedowns/account bans on Etsy, Amazon, and TikTok Shop.

## AI Prompt Library (ready-to-use templates)

### Niche research prompt
```
Act as a print-on-demand niche researcher. I want to explore the [BROAD NICHE] category
(e.g. pets, professions, hobbies). Generate 10 micro-niche ideas using an
Identity × Interest framework (a specific type of person + a specific occasion/interest),
avoiding generic/overused angles. For each, suggest 3 product types (apparel, drinkware,
home decor, etc.) and a one-line reason why this micro-niche could convert well in [target market].
```

### Design brief prompt
```
Write a design brief for a [PRODUCT TYPE] targeting [MICRO-NICHE]. Include: main text/slogan
(short, punchy, under 8 words), suggested font style (hero + support), suggested color palette
(2-3 colors), and a one-sentence visual concept description an illustrator or AI image tool
could use to generate the artwork. Avoid any copyrighted names, characters, or logos.
```

### Etsy SEO listing prompt
```
Write an Etsy listing for [PRODUCT] in the [NICHE] niche. Output:
1. Title (under 70 characters, primary keyword in first 40 characters, format:
   [Primary Keyword] | [Secondary Keyword + modifier] | [Occasion/Recipient Keyword])
2. 13 tags (mix of broad, long-tail, and occasion/recipient keywords, no duplication of the title)
3. A description (150-300 words) that is genuinely useful/readable (not keyword-stuffed) to
   support dwell time, written in a warm, benefit-focused tone, ending with a clear CTA.
```

### TikTok Shop affiliate hook/script prompt
```
Write 3 short (15-20 second) TikTok Shop video scripts for [PRODUCT] in the [NICHE] niche.
Each script needs: a hook in the first 1-2 seconds, a clear visual/voiceover demonstrating
the product benefit, and a soft CTA pointing to the pinned product link. Keep tone native
to TikTok (casual, not ad-like).
```

### Darija/Arabic-language listing & content prompt (for PODAcademy's MENA-facing students)
```
اكتب وصف Etsy listing لـ[المنتج] فالنيتش ديال [NICHE]، بالدارجة المغربية (ماشي المصرية)،
بأسلوب دافئ وواضح، كيخدم على الـ"dwell time"، ومزيان للزبون اللي كيقرا الوصف قبل الشراء.
```

## How to combine with Anthropic API in Artifacts
If building an in-house AI design/listing tool for PODAcademy students (e.g., a Claude-powered listing generator widget), use the `anthropic_api_in_artifacts` capability — call the prompts above as system/user messages, optionally with structured JSON output for plugging into a UI (title/tags/description fields).
