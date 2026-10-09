---
name: shopline-app-listing-writer
description: Use this skill whenever the user wants to write Shopline app marketplace listing content for a plugin or app — specifically any combination of: operation guide (操作说明), app description (应用描述, ≤200 words), product features (产品特色, up to 3 entries with title + description), and about section (关于, ≤5000 characters). Trigger on requests like "帮我写插件的应用描述", "write the operation guide for my app", "帮我写三条产品特色", "生成Shopline应用市场上架内容", "write the About section for my plugin", or whenever the user uploads a screenshot of the Shopline listing form fields (操作说明 / 产品特色介绍 / 关于). Also trigger when the user wants all four sections at once. Always produce English output unless the user explicitly requests Chinese.
---

# Shopline App Listing Writer

A skill for producing the four standard content blocks required to publish a plugin on the Shopline App Marketplace. Each block has fixed field names, character/word limits, and audience expectations. This skill ensures every block is on-brand, within limits, technically accurate, and optimized for merchant comprehension.

---

## The Four Blocks

| Block | Shopline field name | Limit | Audience |
|---|---|---|---|
| 1 | 操作说明 (Operation Guide) | No hard limit; aim for 300–600 words | Merchants installing for the first time |
| 2 | 应用描述 (App Description) | ≤ 200 words | Merchants browsing the marketplace |
| 3 | 产品特色介绍 (Product Features) | 3 entries max; each: title ≤80 chars, description ≤300 chars | Merchants scanning listing at a glance |
| 4 | 关于 (About) | ≤ 5000 characters | Merchants doing deep evaluation |

---

## Step 1 — Gather inputs

Before writing, collect the following. Infer from conversation context first; ask only for genuine gaps.

1. **Plugin name** — exact name as it appears in the Shopline admin
2. **What the plugin does** — core workflow in one sentence
3. **Key features** — 3–5 concrete capabilities (what the user actually does, not marketing adjectives)
4. **Third-party integrations** — any APIs, services, or platforms the plugin connects to (e.g., Cathay Insurance, 17TRACK, Shopline Billing API)
5. **Developer / brand name** — the company that built the plugin; this must appear in the app description (see brand rule below)
6. **Setup steps** — the actual sequence a merchant follows from install to go-live; ask if not in context
7. **Any existing docs, PRD, user manual, or FAQ** in the conversation — extract from these first

---

## Step 2 — Brand rule (mandatory)

**The app description must include the developer's brand name.** Default pattern:

> "…developed by **[Brand Name]**…" or "…built for [platform] merchants by **[Brand Name]**."

Place the brand mention naturally — either in the opening sentence or the closing sentence of the description. Never omit it. If the user specifies an exact brand phrase (e.g., "Silk Software", "SilkSoft"), use it verbatim, with bold formatting.

---

## Step 3 — Write Block 1: Operation Guide (操作说明)

**Purpose:** Step-by-step installation and first-use instructions. This is a reference doc, not a sales pitch.

**Format rules:**
- Use numbered steps with bold step labels: `**Step 1 — [action verb phrase]**`
- Each step: 1–3 sentences. State what the merchant does, where in the UI, and what the outcome is.
- Cover in this order: install/authorize → complete setup checklist (if applicable) → configure required settings → fund/connect external dependencies → go live → core recurring workflow (e.g., how to file a claim, how to process a return)
- End with the most common ongoing action (the thing merchants will do repeatedly after setup)
- No marketing language. No adjectives that don't describe a UI state or action.

---

## Step 4 — Write Block 2: App Description (应用描述)

**Purpose:** The first thing a merchant reads on the marketplace listing. Must make the value proposition and workflow clear in ≤200 words.

**Format rules:**
- Word count: strictly ≤200. Count and state the word count in a comment after the block.
- Paragraph structure: opening (what it does + brand mention) → core automated workflow → what merchants see/manage → key integrations or trust signals → closing brand/positioning line.
- Brand name: bold, placed in paragraph 1 or the final sentence (see brand rule above).
- No bullet points — this is a prose paragraph block.
- Do not start sentences with "We" — write from the product's perspective ("The plugin…", "Merchants can…", "Insurance is issued…").
- Forbidden phrases: "seamless", "powerful", "robust", "game-changer", "cutting-edge", "innovative solution".

---

## Step 5 — Write Block 3: Product Features (产品特色介绍)

**Purpose:** Three scannable feature cards. Each card = one title + one description. Merchants read these to decide if the plugin solves their specific problem.

**Format rules:**
- Exactly 3 features (Shopline requires at least 3; the form allows up to 3).
- Title: ≤100 characters. Bold in the output. Format: `**[Benefit phrase] — [mechanism phrase]**`. Never start with a verb ("Automate…" is weak; "Fully automated policy issuance — zero manual steps" is strong).
- Description: ≤400 characters (~60–80 words). One dense paragraph. State: what happens, when, what the merchant doesn't have to do, and one concrete edge case or detail that proves the feature is real (not marketing fluff).
- Cover a spread of concerns: one feature on the core automated workflow, one on the merchant-facing management/reporting, one on a differentiated detail (financial transparency, edge case handling, multi-language support, etc.).
- No overlap between feature descriptions. Each must be about a different capability.

---

## Step 6 — Write Block 4: About (关于)

**Purpose:** The comprehensive description for merchants doing a detailed evaluation. More depth than the app description; still focused on what the merchant experiences, not internal implementation.

**Format rules:**
- ≤5,000 characters. State the approximate character count in a comment after the block.
- Use **bold subheadings** for each section. Suggested sections (adapt as needed):
  - What the plugin does (2–3 sentences)
  - [Core workflow area 1] (e.g., Wallet and billing)
  - [Core workflow area 2] (e.g., Policy management and claims)
  - [Core workflow area 3] (e.g., Payouts and commissions)
  - Configuration
  - Built by [Brand Name] (closing paragraph: 3–5 sentences on the company and positioning, ending with support contact)
- Do not repeat the app description verbatim — go deeper on mechanics.
- End with: `For support, contact: [support email]`

---

## Step 7 — Output format

- Default output: a **single Markdown file** at `/mnt/user-data/outputs/[plugin-slug]_listing_content.md` containing all four blocks, clearly labelled with `## 1. Operation Guide`, `## 2. App Description`, `## 3. Product Features`, `## 4. About`.
- If the user only wants one or two specific blocks, produce only those — but still output to a file.
- After the file is written, call `present_files` so the user can download it.
- Do NOT produce all four blocks inline in chat as long prose — always write to file.

---

## Quality checklist (run mentally before saving the file)

- [ ] Word count on app description ≤200 — verified and noted
- [ ] Character count on About ≤5,000 — verified and noted  
- [ ] Brand name appears (bolded) in app description
- [ ] Product features: exactly 3 entries, each title ≤100 chars, each description ≤400 chars
- [ ] Operation guide: numbered steps, bold step labels, no marketing language
- [ ] Zero use of: seamless, powerful, robust, game-changer, cutting-edge, innovative
- [ ] Each feature description covers a different capability (no overlap)
- [ ] About section has bold subheadings and ends with support contact

---

## Example titles for product features (reference only — do not copy verbatim)

- `Fully automated policy issuance — zero manual steps`
- `One-click claims and appeals — fully in-app`
- `Wallet, billing, and monthly commissions in one place`
- `Real-time sync with no manual export needed`
- `Multi-currency support with operator-configured exchange rate markup`

Use these as structural models. Always replace with content specific to the actual plugin being documented.
