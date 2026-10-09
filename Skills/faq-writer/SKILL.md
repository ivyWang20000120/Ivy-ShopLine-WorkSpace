---
name: faq-writer
description: Use this skill whenever the user wants to write, draft, or generate a FAQ (常见问题) document for a product, feature, plugin, app, policy, or service — especially technical/B2B FAQs like the "FMS Member Custom Points Plugin FAQ" style (Q1/A, Q2/A numbered format with bold key terms, plain gray background, centered title). Trigger on requests like "帮我写一个FAQ", "生成产品FAQ文档", "write a FAQ for my app/plugin", "FAQ格式文档", or when the user references an existing FAQ and wants a similar one for a different project. Produces a clean, scannable Q&A document that surfaces edge cases, defaults, and policy boundaries rather than generic marketing copy.
---

# FAQ Writer

A skill for producing tight, technical-style FAQ documents in the "FMS Member Custom Points Plugin FAQ" format: a centered title, numbered Q&A pairs (Q1/A, Q2/A...), bold key terms inside answers, and answers that state concrete defaults, edge cases, and policy boundaries instead of vague marketing language.

## When to use this

Use whenever someone wants a FAQ for:
- A plugin / app / feature (e.g. Shopify/Shopline apps, SaaS features, internal tools)
- A policy or process (refunds, data retention, onboarding)
- Any product where users will ask "how does X work", "what happens if Y", "can I do Z"

Do NOT reach for generic conversational Q&A phrasing — this skill's whole value is being **specific, structured, and unambiguous**.

## Step 1: Gather the raw material

Before writing anything, collect (ask the user if missing, but infer from conversation context first):

1. **What is the product/feature?** One-line description of what it does.
2. **Who is the audience?** (merchants, developers, end customers, internal staff)
3. **What are the core mechanics?** How rules/settings/flows work, step by step.
4. **What are the tricky edge cases and defaults?** This is the most important input — good FAQs exist specifically to resolve ambiguity: timing behavior, conflicts, disabling/deleting, uninstall/data retention, limits, error states.
5. **Any existing docs, specs, or a reference FAQ** to mirror the tone/scope of.

If the user gave enough context already (like an existing FAQ to model after, or a spec doc pasted earlier in conversation), don't stop to ask — extract what you can and note any real gaps as a single clarifying question at most.

## Step 2: Pick the questions

A good FAQ in this style has 5–10 questions, ordered roughly as:

1. **What does it do?** (one-sentence positioning question, always first)
2. **How do I use/set it up?** (the core workflow, step-by-step with →)
3. One or more **"what is [ambiguous concept]?"** questions — this is where you disambiguate any setting that has more than one interpretation (timing, scope, matching logic). Explicitly state the recommended/default option and why.
4. **State-change questions**: what happens when you disable, delete, edit, or pause something.
5. **Conflict/limit questions**: can two rules overlap, is there a cap, priority order.
6. **Lifecycle/data questions**: uninstall, data retention, refunds/reversals, exports.

Skip questions that are pure marketing ("why should I use this?") unless the user explicitly wants that tone — this format is a reference doc, not a sales page.

## Step 3: Write each answer

Follow these rules strictly — they are what make this format work:

- **Format**: `Q{n}: {question}` on its own line, blank line, then `A: {answer}`.
- **One answer = one short paragraph.** 2–4 sentences max. If an answer needs more, it's actually two questions — split it.
- **Bold the load-bearing terms**, not whole sentences: settings names, states (enabled/disabled), key nouns (rules, points, fixed number), and any stated limit or default (e.g. **one active rule per product per store**). Bold is used to let someone scanning the page find the operative fact instantly — don't bold connective words.
- **State the default explicitly and say why**, when a setting has options: *"The default recommendation is X for [concrete reason]."* Never leave a "which should I pick" question unanswered.
- **Name the exact mechanism**, don't hand-wave. Compare:
  - Weak: "Points are given after the order is processed."
  - Strong: "Points are attempted after the order reaches **paid** (payment confirmed) according to [platform]'s order model."
- **Cover the negative case.** For any conditional behavior, state what does NOT happen and when (e.g. "unpaid or partially shipped orders do not trigger issuance under this option").
- **Use plain declarative sentences.** No hedging ("might", "could potentially") — if the real behavior is uncertain, say what governs it (e.g. "follows the policy published with the App") rather than guessing.
- **Steps use arrows**, not numbered sub-lists, when describing a short UI workflow: `Open X → Create Y → Select Z → Save.`

## Step 4: Assemble the document

- Centered `# {Product Name} FAQ` title at the top.
- Plain numbered Q/A pairs in order, one blank line between Q and A, one blank line (visually, a bit of extra space) between each Q&A pair.
- No extra sections (no "Contact us", no TOC, no icons) unless asked — keep it as lean as the reference format.

## Step 5: Output

- Default to a **Markdown file** (`.md`) in `/mnt/user-data/outputs/`, since this is a standalone reference document the user will reuse/share (see file-creation guidance: standalone deliverables → file, not inline chat).
- If the user explicitly wants a Word document (`.docx`) for distribution to clients or non-technical stakeholders, use the `docx` skill instead and apply the same structural rules (bold key terms, Q/A pairs, centered title) using Word heading/paragraph styles.
- If the user wants it to visually match a screenshot's styling (centered title, specific background), and they want an actual rendered visual rather than an editable doc, an HTML version can be offered — but Markdown is the right default deliverable.

## Example skeleton to follow

```
                    {Product Name} FAQ

Q1: What does {the product} do?

A: It lets {audience} do {core action} by {mechanism}.

Q2: How do I {primary action}?

A: {Step} → {Step} → {Step} → Save. You can {secondary actions}.

Q3: What is "{ambiguous setting}"?

A: {Option A} means {precise behavior}. {Option B} means {precise
behavior}, and {edge case/negative case}. The default recommendation
is {X} because {reason}.

Q4: What happens if I {state change, e.g. disable/delete/uninstall}?

A: {Precise consequence}. {What is preserved vs. lost, if relevant}.

Q5: Can {conflict/limit question}?

A: {Stated limit or rule}, {short reason}.
```

Use this skeleton as structural scaffolding, not literal text — always replace with the specifics of the actual product being documented.
