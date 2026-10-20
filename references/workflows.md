# Workflow composition

## External workflow sources
- SEO content writer: https://github.com/Yaroslavle/seo-content-writer-claude-skill
- Humanizer: https://github.com/blader/humanizer

Use the SEO workflow for search intent, JTBD framing, keyword placement, useful structure, metadata, internal linking, and editorial quality. Use Humanizer principles across the complete draft: remove generic AI phrasing, vary rhythm and sentence shape, prefer concrete observations and direct language, avoid padding and unsupported certainty, and preserve the author's useful specificity. Treat both sources as guidance, not text to reproduce.

## BoxCount operating rules
- Produce one article at a time and follow the existing article model, renderer, route, asset naming, and test conventions.
- Required data: slug, category, readingTime, title, summary, seoTitle, metaDescription (<=160 characters), focusKeyword, canonicalPath, hero, relatedSlugs, and sections.
- Include natural focus-keyword usage, useful internal links, a clear calculator CTA, and accessible image alt/caption. Prefer scannable headings, steps, checklists, tables, and callouts only when they improve the answer.
- Verify claims against available product/code context; mark uncertainty rather than inventing facts. Generate imagery only through the local xKiro skill using `XKIRO_API_KEY` and `openai/gpt-image-2.5`; keep a valid SVG fallback and report the actual result.
- Test before/with implementation where feasible, then run the full suite and build. Do not run `npm audit fix`.
