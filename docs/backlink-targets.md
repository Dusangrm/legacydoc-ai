# Backlink targets — shortlist (2026-05-10)

A judgement-driven shortlist of 12 targets, sorted by **expected value per
hour of effort**. Honest take: most directories now require login,
captcha, or email confirmation. Don't expect a one-day batch submission
sweep. Aim for **one well-prepared submission per session**, not volume.

## Grading rubric

- **A** — High relevance, public indexable page, dev/AI-coding audience,
  reasonable acceptance rate.
- **B** — Relevant. Free submission. Possible indexing value. Lower
  acceptance certainty.
- **C** — Low relevance. Useful only as a discovery surface, not a
  ranking signal.
- **D** — Spammy / forced paid / not crawlable / no public listing page.
  **Do not submit.**

## Submission feasibility flags

- **Login** — needs an account (GitHub OAuth, Google, email/password)
- **Captcha** — needs a real human to pass an interactive challenge
- **Email** — needs to click a confirmation link in your inbox
- **PR** — submission happens via GitHub Pull Request (you control the
  diff, but the maintainer needs to merge)
- **None** — pure form submission with no human-in-the-loop signals
  (rarely real anymore)

## Shortlist

| # | Platform | URL | Type | Login? | Captcha? | Email? | Free? | Auto-submit? | Quality | Recommended action |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | **awesome-vscode** | https://github.com/viatsko/awesome-vscode | VS Code list | GitHub login | No | No | Yes | No (PR) | A | **Open a PR** adding LegacyDoc AI under the AI/Documentation section. Real-person task. Highest-value link in this list — well-indexed, dofollow, dev-targeted. |
| 2 | **awesome-cursorrules** | https://github.com/PatrickJS/awesome-cursorrules | AI coding list | GitHub login | No | No | Yes | No (PR) | B | Add a section/example showing how to drop the LegacyDoc AI context pack into a Cursor `.cursorrules` workflow. Real-person task. Niche but exact-audience. |
| 3 | **DevHunt** | https://devhunt.org/ | Indie dev launches | Yes (GitHub OAuth) | No | Likely | Yes | No | B | Real-person submission. Aim for a Tuesday or Wednesday launch slot. Use the 80-char tagline + 300-char description from `docs/submission-copy.md`. |
| 4 | **Uneed.best** | https://www.uneed.best/submit-a-tool | Curated weekly | Yes (Twitter/Google) | No | No | Yes (free + paid lanes) | No | B | Real-person submission. Free lane has multi-week queue; paid lane is fast. Choose free unless time-pressured. |
| 5 | **Product Hunt** | https://www.producthunt.com/ | Launch platform | Yes | No | Yes | Yes | No | B | Do **not** submit casually. Prepare assets (gallery, hunter, first-hour comments) and pick a launch day. One shot per product. Defer until the GitHub repo + The Next AI / AISO Tools listings are live so the launch isn't bare. |
| 6 | **IndieHackers / Products** | https://www.indiehackers.com/products | Indie founder community | Yes (email or social OAuth) | No | Yes | Yes | No | B | Real-person submission. Adds a product page that ranks for `legacydoc ai` and shows in the IH product feed. Cross-link to the website. |
| 7 | **FutureTools** | https://www.futuretools.io/submit-a-tool | AI tools directory | Email field | Possibly | Likely (confirmation) | Yes | No | B | Real-person submission. Description must avoid overpromise. Use the 160-char short description from `docs/submission-copy.md`. |
| 8 | **InsidrAI** | https://insidr.ai/submit-tool/ | AI tools directory | Email field | Probably | Yes | Yes | No | C | Real-person submission. Lower authority, decent indexing. Use only after the higher-priority submissions land. |
| 9 | **AIWizard** | https://aiwizard.ai/submit-ai-tool | AI tools directory | Probably no login | Likely (Cloudflare) | Possibly | Yes | Maybe | C | Try the form once with a real person (not automation). Cloudflare bot detection is the main gate. |
| 10 | **AITools.fyi** | https://aitools.fyi/submit | AI tools directory | Possibly | Likely | Possibly | Yes | No | C | Real-person submission. Use after the A/B tier. |
| 11 | **AIToolBoard** | https://aitoolboard.com/submit | AI tools directory | Possibly | Possibly | Likely | Yes | No | C | Real-person submission. Lower authority, fast acceptance. |
| 12 | **BetaList** | https://betalist.com/submit | Founder/MVP launches | Yes | No | Yes | Yes (free + paid) | No | B | Real-person submission. Free lane is slow; explicit "early access / beta" framing helps. Optional. |
| 13 | **AInexfinder** | https://ainexfinder.com/submit | AI tools directory | No obvious login for form | No obvious captcha in static HTML | Yes (approval email) | Yes | No | B | Real-person submission. Free listing, stated 24-48h review, and stated dofollow backlink. Requires richer assets: logo, category, features, detailed description, terms checkbox. |
| 14 | **airesources.dev** | https://github.com/catalinpit/airesources | AI coding resources repo | GitHub login | No | No | Yes | No (PR) | A-/B+ | Prepare a PR adding LegacyDoc AI under `src/content/resources/extensions/`. Strong developer relevance; do after the public profile repo is live so maintainers see a credible product footprint. |
| 15 | **awesome-ai-coding-tools** | https://github.com/ai-for-developers/awesome-ai-coding-tools | AI coding tools list | GitHub login | No | No | Yes | No (PR) | A | Active repo, ~1.7k stars, has CONTRIBUTING, and accepts AI developer tools. Prepare a PR under Code Review and Refactoring or Documentation after the public profile repo is live. |
| 16 | **awesome-vibe-coding** | https://github.com/ai-for-developers/awesome-vibe-coding | Vibe coding resources list | GitHub login | No | No | Yes | No (PR) | A-/B+ | Very relevant to current positioning. Candidate sections: Extensions & Plugins or Project Documentation. Use restrained wording: audit-ready context pack / cleanup readiness, not security scanner. |
| 17 | **awesome-ai-devtools** | https://github.com/jamesmurdza/awesome-ai-devtools | AI developer tools list | GitHub login | No | No | Yes | No (PR) | A- | Strong developer audience, ~3.7k stars. Candidate sections: IDE Extensions, Documentation Generation, or PR & Code Review Bots. Higher bar; submit only after GitHub public profile and 1-2 listings are live. |
| 18 | **awesome-code-ai** | https://github.com/sourcegraph/awesome-code-ai | AI coding tools list | GitHub login | No | No | Yes | No | D | Archived repository. Do not submit. Keep only as research reference. |

## Already submitted (from previous rounds — do not re-submit)

| Date | Platform | Status | Notes |
| --- | --- | --- | --- |
| 2026-05-09 | The Next AI (`thenextai.com`) | Submitted | Codex confirmed `success: true`. Watch for approval email + listing URL. |
| 2026-05-10 | AISO Tools (`aisotools.com`) | Submitted | Codex confirmed `{"success":true,"message":"Submission received! We'll review your tool within 24 hours."}`. |

## Targets explicitly **not** recommended

| Platform | Reason |
| --- | --- |
| TheresAnAIForThat (TAAFT) | Free queue is months; paid review charges. Skip until paid budget is decided. |
| Toolify.ai | Cloudflare-gated, requires login, low public-page authority for new entries. Effort > value. |
| StackShare | Aimed at company tech stacks, not extensions. Wrong audience. |
| AlternativeTo | Forces you to be an "alternative to" something specific; LegacyDoc AI's positioning is its own category. Better as a manual edit later. |
| Open VSX Registry | Not a "link submission" — it requires actually publishing the VSIX. **Defer until 0.2.3 is decided** (separate workflow, separate risk). |
| Devpost | Hackathon-driven, not a directory. Wrong audience. |
| Coderoma, Aipedia, generic "AI tool wall" sites | Spam-adjacent, low authority, no human curation. Submitting hurts more than helps. |

## Realistic submission cadence

- **Week 1**: Publish the GitHub public profile repo. Submit DevHunt and
  Uneed.best.
- **Week 2**: Open the awesome-vscode PR. Confirm The Next AI / AISO
  Tools listings are live and link back. Prepare / optionally open the
  airesources.dev PR if the public profile repo is already live.
- **Week 3**: IndieHackers product page. FutureTools.
- **Week 4**: Product Hunt launch (only if Week 1–3 produced any
  referral traffic in GA).
- **Beyond**: Lower-tier C-grade directories as time allows.

## Hard rules for submissions (apply every time)

- Always submit `https://www.romanticode.com/tools/ai-code-audit-report/`
  as the **primary URL**. Not the homepage. The tool page is the most
  conversion-relevant landing page.
- Exception: extension/resource repositories such as `airesources.dev` may link
  to `https://www.romanticode.com/legacydoc-ai/` when the list format is
  product/extension-centric rather than report/tool-centric. Keep the
  Marketplace URL in the PR body when possible.
- Always include the **Marketplace** install URL when there is a separate
  install/download field.
- Always submit `contact@romanticode.com` as contact, not a personal
  email.
- Never accept a directory's "we'll publish it as nofollow unless you
  pay" upsell.
- Never accept a directory that demands a reciprocal backlink ("add our
  badge to your homepage and we'll list you"). Treat it as D-grade.
- Always paste the 300-character description from `docs/submission-copy.md`
  unmodified, so messaging stays consistent across listings.

## Outcome tracking

Keep a single submission log at the bottom of this file (or in
`docs/submission-copy.md` Section 8 if you prefer). Each entry should
record:

- Date submitted
- Platform
- URL of submission form used
- Status returned (success / pending / rejected)
- Public listing URL (when approved)
- Date the public listing was first crawlable

Without this log, the same target gets re-submitted by a future agent and
the team loses track of who is in queue where.

### Submission log

| Date | Platform | Status | Public listing URL | Crawl-confirmed | Notes |
| --- | --- | --- | --- | --- | --- |
| 2026-05-09 | The Next AI | Submitted | _pending_ | _pending_ | Codex auto-submitted; awaiting approval email. |
| 2026-05-10 | AISO Tools | Submitted | _pending_ | _pending_ | Codex auto-submitted; 24-hour review window. |

---

## Submission pack — AInexfinder

Real-person submission pack for `https://ainexfinder.com/submit`. Form
takes ~5 minutes. Stated review window 24–48 hours, stated dofollow
backlink. Verify the dofollow claim once a listing actually publishes.

### Identity

| Field | Value |
| --- | --- |
| Product name | LegacyDoc AI |
| Vendor / company | RomantiCode |
| Primary URL | `https://www.romanticode.com/tools/ai-code-audit-report/` |
| Marketplace install URL | `https://marketplace.visualstudio.com/items?itemName=ruilegendoc.legacy-doc-ai` |
| Demo / example URL | `https://www.romanticode.com/examples/ai-code-audit-report/` |
| Contact email | `contact@romanticode.com` |
| Pricing | Freemium (Free 5 generations/day, Pro $29 one-time) |
| Category (primary) | Developer Tools / Coding & Development |
| Category (secondary, if dual select) | Code Documentation / Code Review / AI Coding Tools |

### Tagline (50–80 char)

> AI code audit reports for AI-generated code, run inside VS Code (BYOK).

(72 characters)

### 300-character description (paste verbatim)

> LegacyDoc AI is a VS Code extension that turns AI-generated, vibe-coded,
> and legacy codebases into audit-ready context packs. Generate JSDoc,
> Markdown docs, Mermaid architecture maps, module summaries, areas to
> inspect, and cleanup priorities. Runs inside VS Code. BYOK. No code
> storage or proxying by RomantiCode.

(298 characters — same string used everywhere else for consistency.)

### 500–800 character description

> LegacyDoc AI is a VS Code extension for understanding and preparing
> codebases — legacy projects, AI-generated MVPs, vibe-coded prototypes,
> and inherited apps — before cleanup, refactor, review, or handoff. From
> a folder you select inside VS Code, it generates an AI code audit
> report: project overview, Mermaid architecture map, module and folder
> summaries, areas to inspect, cleanup priorities, and an AI-ready
> context pack you can hand to Claude Code, Cursor, or Codex.
>
> It is BYOK. Your code is sent directly to the AI provider you configure
> (Anthropic, OpenAI, Google Gemini, xAI, or any OpenAI-compatible
> endpoint). Nothing is stored or proxied by RomantiCode. Free tier
> includes 5 generations per day; Pro is a one-time $29 unlock for
> unlimited generations and project-level analysis.

(746 characters)

### 3–5 key features (paste as bullet list)

1. **AI code audit reports** — structured audit document with project
   overview, architecture map, module summaries, areas to inspect, and
   cleanup priorities.
2. **Mermaid architecture diagrams** — module-relationship graphs
   rendered directly in VS Code, with built-in syntax validation.
3. **JSDoc, comments, and Markdown docs** — three output modes (inline,
   Markdown file, or both), with a diff preview before any code is
   modified.
4. **AI-ready context packs** — a standalone Markdown context bundle you
   can attach to a Claude Code, Cursor, or Codex session.
5. **BYOK across providers** — Anthropic, OpenAI, Google Gemini, xAI, or
   any OpenAI-compatible endpoint. No RomantiCode-side AI cost.

### Privacy / boundary statement (paste verbatim if asked)

> Runs inside VS Code + BYOK. No code storage or proxying by RomantiCode.
> Code is sent directly to the AI provider you configure.

### Logo / icon URL candidates

In order of preference:

1. `https://www.romanticode.com/favicon.svg` — verified live, returns
   `image/svg+xml`. Best for sites that accept SVG.
2. `https://www.romanticode.com/favicon.ico` — verified live, returns
   `image/vnd.microsoft.icon`. Use only when SVG is rejected.
3. **No 512×512 square PNG asset exists yet.** If AInexfinder requires a
   square PNG specifically, see the "Risk" section below.

### Screenshot / preview image candidates

1. `https://www.romanticode.com/images/legacydoc-hero.png` — verified
   live (HTTP 200, `image/png`). Use as the primary screenshot.
2. **No 1200×630 OG image, no in-VS-Code screenshot library yet.** Do not
   invent screenshots. Submit with only the hero image and accept the
   risk of a "needs more visuals" rejection.

### Tags / keywords (paste 8–10)

`ai code audit`, `vibe code cleanup`, `ai generated code`,
`code documentation`, `vs code extension`, `architecture map`,
`context pack`, `byok`, `claude code`, `cursor`

### Bound copy rules — do not write in any free-text field

- `your code never leaves your machine`
- `local-only`
- `runs entirely on your machine`
- `complete security audit`
- `guaranteed production ready`
- `one-click cleanup`
- `fully automatic`

If the form forces a binary "is this a security tool?" question, answer
**no**. LegacyDoc AI prepares codebases for review; it does not perform
security testing.

### Real-person submission steps

1. Open `https://ainexfinder.com/submit` in a browser session that can
   solve a captcha if one appears.
2. Paste each field above directly. Do not paraphrase the description or
   the privacy statement — listing-to-listing consistency matters more
   than variety.
3. Upload `https://www.romanticode.com/favicon.svg` if SVG is accepted;
   otherwise fall back to `favicon.ico`. If a separate hero image is
   required, use `https://www.romanticode.com/images/legacydoc-hero.png`.
4. Tick the terms / quality checkbox **only after** confirming the form
   does not require a reciprocal backlink ("add our badge to your homepage
   and we'll list you"). If it does, abort and downgrade AInexfinder to
   Grade D in this file.
5. Submit. Do not click any "boost listing" / "fast review" upsell
   without explicit user approval.

### What to record after submission

Append to the **Submission log** above:

- Date submitted
- Email confirmation received? (yes/no, time)
- Listing approval email received? (yes/no, date)
- Public listing URL once live
- Date the listing first appeared in `site:ainexfinder.com legacydoc`
- Whether the listing is dofollow (inspect the published page's
  `<a rel>` attribute)

### Risk

- **No square 512×512 logo PNG.** If the form rejects SVG and demands a
  square PNG, the submission is blocked until one is exported. Cheapest
  fix: render the SVG to a 512×512 PNG once and host it at
  `/images/legacydoc-icon-512.png`.
- **No screenshot library beyond the hero image.** Most directories want
  2–3 in-product screenshots. Acceptance odds drop with only one image.
- **Reciprocal-backlink demand.** AInexfinder advertises a free dofollow
  listing, but if the form silently demands a backlink-back, treat it as
  the same prohibited pattern as Toolify and abort.

---

## PR pack — airesources.dev (`catalinpit/airesources`)

Real-person GitHub PR pack. The repo is an active Astro site (default
branch `main`, last push 2026-05-08, 11 stars), schema enforced by Zod.
Maintainer merged a comparable PR ("Add OpenClaw to extensions") on
2026-05-08 — a clean, schema-compliant PR has a realistic chance of
acceptance within 1–2 weeks.

### Repo facts (verified 2026-05-11)

| Field | Value |
| --- | --- |
| Repo | `catalinpit/airesources` |
| Default branch | `main` |
| Stack | Astro 5 + Tailwind CSS 4 + pnpm |
| Schema | `src/content.config.ts` (Zod, `defineCollection` for `categories` and `resources`) |
| Required fields | `name`, `description`, `categorySlug` |
| Optional fields | `link`, `iconUrl`, `previewImage`, `type`, `pricing.{type,tiers,details}`, `models`, `tags`, `prompt`, `example`, `author`, `sponsored` |
| Pricing enum | `free` / `paid` / `freemium` / `byok` / `top-up` |
| Build verification | `pnpm install && pnpm build` (build fails on schema violations) |
| CONTRIBUTING.md | none |
| PR template | none |
| Existing slug `legacydoc-ai` | not present (clean slot) |

### Target file path

`src/content/resources/extensions/legacydoc-ai.md`

(`extensions` is the canonical category slug for VS Code-style
extensions — confirmed via
`src/content/categories/extensions.json`:
`{"title":"Extensions","description":"AI-powered extensions and plugins
for your favorite editors","categorySlug":"extensions"}`.)

### File contents (drop-in, schema-validated)

```md
---
name: LegacyDoc AI
description: VS Code extension that generates AI code audit reports, JSDoc, Markdown docs, and Mermaid architecture maps from your codebase. BYOK to your AI provider.
categorySlug: extensions
link: "https://www.romanticode.com/legacydoc-ai/"
iconUrl: "https://www.romanticode.com/favicon.svg"
previewImage: "https://www.romanticode.com/images/legacydoc-hero.png"
type: extension
pricing:
  type: freemium
  tiers:
    - name: Free
      price: $0
    - name: Pro
      price: $29 one-time
  details: Free tier includes 5 generations per day. Pro unlocks unlimited generations, project-level analysis, and custom prompt templates.
tags:
  - ai code audit
  - documentation
  - architecture
  - context pack
  - byok
---
```

Field-choice rationale:

- `link` points to the **product page**, not the tool page. The tool
  page is one click in. Product pages tend to be more evergreen for
  directory listings.
- `iconUrl` uses SVG; airesources renders favicons via `<img>`, modern
  browsers handle SVG fine, and several existing entries use SVG.
- `previewImage` is added because the schema supports it and we have a
  verified hero image. Many existing entries omit it; including ours
  gives our row a slight visual edge.
- No `models` field — the gold-standard `openclaw.md` (most recently
  merged PR) omits it. Adding it would make our entry longer than peers
  without changing acceptance probability.
- `tags` kept short (5 entries), aligned with the directory's existing
  tag vocabulary.

### PR title

`Add LegacyDoc AI to extensions`

(Mirrors the merged "Add OpenClaw to extensions" pattern verbatim.)

### PR body

```md
Adds LegacyDoc AI, a VS Code extension that generates AI code audit
reports, JSDoc, Markdown docs, and Mermaid architecture diagrams from a
local codebase.

- File added: `src/content/resources/extensions/legacydoc-ai.md`
- Category: `extensions` (matches `src/content/categories/extensions.json`)
- Pricing type: `freemium`
- Schema fields used: `name`, `description`, `categorySlug`, `link`,
  `iconUrl`, `previewImage`, `type`, `pricing`, `tags`
- All optional fields validated against `src/content.config.ts`
- `pnpm build` passes locally

Product page: https://www.romanticode.com/legacydoc-ai/
Tool page: https://www.romanticode.com/tools/ai-code-audit-report/
Marketplace: https://marketplace.visualstudio.com/items?itemName=ruilegendoc.legacy-doc-ai

Thanks for maintaining the directory.
```

### Real-person fork → PR steps

```bash
# 1. Fork via the GitHub web UI (https://github.com/catalinpit/airesources)
#    while signed in as Dusangrm. Do NOT script the fork.

# 2. Clone YOUR fork to a fresh working directory.
#    Do NOT touch the extension repo or romanticode-site.
cd "/Users/dusang/文件/AI INDIE"
git clone https://github.com/Dusangrm/airesources.git airesources-fork
cd airesources-fork

# 3. Branch off main.
git checkout -b add-legacydoc-ai

# 4. Drop the prepared file in. Use the exact frontmatter above.
mkdir -p src/content/resources/extensions
# Then create src/content/resources/extensions/legacydoc-ai.md with the
# contents from the "File contents" block.

# 5. Verify the build BEFORE committing. This is the gate that catches
#    schema mistakes the maintainer would otherwise have to flag.
pnpm install
pnpm build
# expected: "✓ Completed in <Xms>" with 0 errors.

# 6. Commit with a clean, single-purpose message.
git add src/content/resources/extensions/legacydoc-ai.md
git commit -m "Add LegacyDoc AI to extensions"

# 7. Push the branch to your fork.
git push -u origin add-legacydoc-ai

# 8. Open the PR via GitHub web UI. Use the PR title and PR body above.
#    Target: catalinpit/airesources main.

# 9. Do NOT @-mention the maintainer. The repo is small and surfaces
#    PRs organically.
```

### Possible rejection reasons (and the response for each)

| Reason | Response |
| --- | --- |
| Schema validation fails (`pnpm build` errors) | Fix locally, force-push the same branch. CI re-triggers automatically. |
| Maintainer asks to drop `previewImage` because peers don't have it | Drop the field, force-push. Don't argue. |
| Maintainer asks to switch `link` to the tool page or homepage | Match maintainer preference. Editorial choice wins. |
| Maintainer asks to remove `tags` because category already conveys them | Remove `tags`, keep everything else. |
| Maintainer says "we don't list paid tools" | Drop the `pricing` block, keep `type: extension`. The free tier is real. |
| PR sits unreviewed for 14+ days | Add a single, polite comment with the build status. Do **not** spam commits. |
| Hard reject ("not a fit") | Accept. Do not re-submit a renamed copy. Move that effort to a different directory. |

### Re-submit policy if rejected

- 0–24 hours after rejection: do nothing. Re-read the rejection cold.
- Within 7 days: address every concrete point and reopen exactly one PR
  with the changes the maintainer asked for.
- After 14 days of silence on the reopened PR: stop. Spend that effort on
  a different directory. There is no fix for "maintainer doesn't reply".

### Build-time verification before pushing

```bash
cd "/Users/dusang/文件/AI INDIE/airesources-fork"
pnpm install
pnpm build

# Quick frontmatter sanity check independent of the build:
head -25 src/content/resources/extensions/legacydoc-ai.md
```

### What to record after submission

Append to the **Submission log** above:

- PR URL (`https://github.com/catalinpit/airesources/pull/<n>`)
- PR opened date
- PR status (open / approved / changes requested / merged / rejected)
- Public listing URL once merged (typically
  `https://airesources.dev/extensions/legacydoc-ai/` — verify on merge)
- Date the listing first appeared in `site:airesources.dev legacydoc`

## PR target notes — GitHub awesome lists

These are **not** automatic submissions. Open PRs only after the public
`Dusangrm/legacydoc-ai` profile repo is live, so maintainers can verify the
product without seeing private source.

### ai-for-developers/awesome-ai-coding-tools

Recommended section:

- Primary: `Code Review and Refactoring`
- Secondary: `Documentation`

Proposed entry:

```md
- **[LegacyDoc AI](https://www.romanticode.com/tools/ai-code-audit-report/)** – VS Code extension that generates AI code audit context packs, Mermaid architecture maps, and cleanup readiness notes from your codebase with your own AI provider key.
```

PR title:

```md
Add LegacyDoc AI to AI coding tools
```

### ai-for-developers/awesome-vibe-coding

Recommended section:

- Primary: `Extensions & Plugins`
- Secondary: `Project Documentation`

Proposed entry:

```md
* [LegacyDoc AI](https://www.romanticode.com/tools/ai-code-audit-report/) — VS Code extension for turning vibe-coded or legacy projects into audit-ready context packs, architecture diagrams, and cleanup readiness notes.
```

PR title:

```md
Add LegacyDoc AI to vibe coding tools
```

### jamesmurdza/awesome-ai-devtools

Recommended section:

- Primary: `IDE Extensions`
- Secondary: `Documentation Generation`

Proposed entry:

```md
- [LegacyDoc AI](https://www.romanticode.com/tools/ai-code-audit-report/) — VS Code extension that creates code documentation, Mermaid architecture diagrams, and AI code audit context packs using your own AI provider key.
```

PR title:

```md
Add LegacyDoc AI
```

### PR safety notes

- Do not say "open source" or imply the commercial product source is public.
- Do not say "local-only" or "your code never leaves your machine."
- Acceptable privacy wording: "Runs inside VS Code + BYOK. No code storage or
  proxying by RomantiCode."
- Link to the tool page, not the homepage.
- If a maintainer asks for source code, respond that the product is commercial
  and distributed through VS Code Marketplace; the public repo is a docs/profile
  repo only.
