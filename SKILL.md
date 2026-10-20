---
name: seo-humanized-article-with-image
description: "Trigger: BoxCount Packing Tips article, SEO article, humanized article, packing guide, article with image. Create one production-ready BoxCount article with SEO metadata, humanized copy, tests, and xKiro imagery."
license: Apache-2.0
metadata:
  author: "luisg"
  version: "1.0"
---

## Activation Contract
Use for exactly one new or revised BoxCount Packing Tips article per invocation.

## Hard Rules
- Inspect the article model/content, renderer, tests, and assets before editing; preserve existing behavior and touch only the requested article.
- Compose `references/workflows.md`, the SEO workflow, Humanizer principles, and the local `xkiro-image-generation` skill; do not copy their long contents.
- Draft JTBD and search intent internally, write useful factual content, then humanize the full draft. Use natural keywords, structured sections, practical lists/checklists/tables/callouts, internal links, calculator CTA, canonical path, accessible alt/caption, and meta description <=160 characters.
- Use only `XKIRO_API_KEY` and explicit `openai/gpt-image-2.5` when available. Never print secrets, prompts, base64, or response bodies; keep SVG fallback, verify a valid file, and never claim image success otherwise.
- Add/update tests before implementation where feasible; run the full test suite and build. Never run `npm audit fix`.
- Never begin a second article without explicit confirmation.

## Decision Gates
| Condition | Action |
|---|---|
| Existing model/renderer convention | Extend it; do not invent a parallel shape |
| Image generation fails | Preserve/use SVG fallback and report failure |
| Facts or intent are uncertain | State limits or ask; never fabricate |

## Execution Steps
1. Inspect current implementation and assets; load local references and image-skill guidance.
2. Define JTBD/intent, metadata, outline, links, and CTA; implement one article.
3. Generate/verify the hero, add tests, run tests/build, and inspect the diff.

## Output Contract
Return: status, article slug, word count, files, image result, tests/build, risks, and next action.

## References
- `references/workflows.md` — external SEO/Humanizer workflows and operational composition rules.
- `assets/article-schema.json` — BoxCount article data shape.
- `../xkiro-image-generation/SKILL.md` — local image-generation contract.
