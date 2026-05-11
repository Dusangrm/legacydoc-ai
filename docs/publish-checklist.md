# Publish checklist — public profile repository

A real-person checklist for publishing this draft as a public GitHub
repository. **Do not run any of these steps automatically.** Each step is
written so a human can read it, decide, and execute.

---

## 1. Repo name candidates

Live availability check on GitHub (2026-05-10):

| Candidate | URL probe | Status | Tradeoffs |
| --- | --- | --- | --- |
| **`legacydoc-ai`** ⭐ recommended | `Dusangrm/legacydoc-ai` | Available (404) | Cleanest match to the product name. Visually aligned with the Marketplace publisher `ruilegendoc.legacy-doc-ai`. Strong SEO anchor for "LegacyDoc AI". Does NOT collide with the private repo `Dusangrm/legacy-doc-ai` because GitHub treats hyphens as significant. |
| `legacydoc-ai-docs` | `Dusangrm/legacydoc-ai-docs` | Available (404) | Most explicit signal that this is documentation, not source. Slightly weaker SEO. Acceptable second choice if you want to leave room for a later open-source repo named `legacydoc-ai`. |
| `romanticode-public-profile` | `Dusangrm/romanticode-public-profile` | Available (404) | Matches the local draft folder name. Honest, but reads like an internal project name and weakens brand SEO. Not recommended as the public-facing URL. |
| `romanticode` | `Dusangrm/romanticode` | Available (404) | Brand-clean name but lives under `Dusangrm/` which dilutes the brand. See "Account choice" below. |
| `legacy-doc-ai` | `Dusangrm/legacy-doc-ai` | **TAKEN** (your existing private repo) | Cannot reuse. |

### Recommendation

**Use `Dusangrm/legacydoc-ai`** (no hyphen between "legacy" and "doc").

Final repo URL would be:

```
https://github.com/Dusangrm/legacydoc-ai
```

This is the strongest single citable URL for the brand without requiring an
organization account.

---

## 2. Account choice — personal vs organization

Live check on GitHub (2026-05-10):

- `github.com/Dusangrm` → personal account, exists, has the private extension
  repo
- `github.com/romanticode` → **already owned by an unrelated user** ("王金剑",
  18 public repos, unrelated to this product). **You cannot register
  `romanticode` as your GitHub login.**
- `github.com/RomantiCode` → same name, GitHub login uniqueness is
  case-insensitive, also taken
- `github.com/RomantiCode-HQ` and `github.com/romanticodehq` → likely
  available, but introduce a "-HQ" suffix that looks slightly off-brand

### Recommendation

**Stay on the personal account `Dusangrm`.**

Reasons:

- The brand name `romanticode` is taken at the GitHub-account level, so a
  brand-clean org URL (`github.com/romanticode/legacydoc-ai`) is not
  achievable.
- A "-HQ" suffix org would look improvised compared to the existing
  professional website at `https://www.romanticode.com/`.
- Submission directories accept any GitHub URL; they do not penalize
  personal accounts.
- A future migration is cheap: GitHub repo transfer to an organization
  preserves the URL via redirect.

If you later want a brand-clean org URL, the realistic options are:

- Reach out to the current owner of `github.com/romanticode` (low success
  rate, takes effort)
- Use a near-name org like `RomantiCodeIO`, `getromanticode`, `ruilegendoc`
  (your Marketplace publisher handle), or a deliberate variant

For now, **don't fight that battle**. Ship the personal repo.

---

## 3. Pre-publish checklist (run yourself before pushing)

```bash
cd "/Users/dusang/文件/AI INDIE/romanticode-public-profile"

# Confirm there is no source code, no secrets, no API keys
ls -R
grep -rEi "api[_-]?key|secret|token|sk-|creem_(test_|[a-z0-9])" .
# expected: only the harmless reference 'creem' appearing inside the public
# checkout URL (https://www.creem.io/payment/prod_6A1crhhY1jAOyEPrIkJPuY)

# Re-run the forbidden-phrase scan
grep -rEi "your code never leaves your machine|local-only|runs entirely on your machine|complete security audit|guaranteed production ready|guarantee production ready|one-click cleanup|fully automatic" \
  README.md docs/links.md docs/submission-copy.md
# expected: only the do-not-say block in docs/submission-copy.md

# Confirm every romanticode.com URL uses www and trailing slash
grep -rEo "https?://[^ )\"']*romanticode\.com[^ )\"']*" \
  README.md docs/links.md docs/submission-copy.md \
  | sort -u
# expected: every page URL ends with /
```

If anything unexpected appears, fix it locally before publishing.

---

## 4. Create the public repo (real-person, GitHub web UI)

1. Open https://github.com/new while signed in as `Dusangrm`.
2. **Repository name**: `legacydoc-ai`
3. **Description**: `Public product profile for LegacyDoc AI — AI code audit
   reports and cleanup readiness for AI-generated codebases (VS Code).`
4. **Visibility**: Public.
5. **Do not** check "Add a README file" (we already have one).
6. **Do not** add `.gitignore` or LICENSE from the template — see step 6
   below for the LICENSE decision.
7. Click **Create repository**.

You should land on the empty-repo "quick setup" screen with an SSH/HTTPS URL
ready to copy.

---

## 5. Push the local draft

In the empty draft directory:

```bash
cd "/Users/dusang/文件/AI INDIE/romanticode-public-profile"

git init -b main
git add README.md docs/
git status
# verify only README.md and docs/ are staged

git commit -m "Initial public profile for RomantiCode / LegacyDoc AI"

# Use the URL GitHub gave you on the empty-repo page:
git remote add origin https://github.com/Dusangrm/legacydoc-ai.git
git push -u origin main
```

If GitHub asks for credentials, prefer a fine-grained personal access token
(PAT) over a password. The PAT only needs `Contents: Read and Write` on
this single repo.

---

## 6. LICENSE / NOTICE decision

This repo intentionally contains no source code. You still want some form
of license so people understand the docs aren't free to repackage as if
they were the product.

Two acceptable options:

- **Option A (recommended)**: do not add an OSI license. Add a one-line
  `LICENSE` file that says:
  > © RomantiCode. All rights reserved. The LegacyDoc AI software is a
  > commercial product distributed via the VS Code Marketplace. This
  > repository contains documentation only.
- **Option B**: Add `CC-BY-4.0` so others can quote your docs with
  attribution. This is friendlier for community sharing.

If you skip this step entirely, GitHub treats the repo as "all rights
reserved by default", which is fine but slightly less clear.

---

## 7. Post-publish verification

Within 5 minutes of `git push`:

```bash
# Repo is live and public
curl -sS -o /dev/null -w "%{http_code}\n" \
  https://github.com/Dusangrm/legacydoc-ai
# expected: 200

# README renders correctly
curl -sSL https://github.com/Dusangrm/legacydoc-ai \
  | grep -oE "RomantiCode|LegacyDoc AI" | head

# All romanticode.com links in README still resolve to 200 (or 308 → 200)
for u in \
  https://www.romanticode.com/ \
  https://www.romanticode.com/legacydoc-ai/ \
  https://www.romanticode.com/tools/ai-code-audit-report/ \
  https://www.romanticode.com/examples/ai-code-audit-report/ \
  https://www.romanticode.com/use-cases/vibe-code-cleanup/ \
  https://www.romanticode.com/blog/ai-code-audit-checklist/ ; do
  echo "$(curl -sS -o /dev/null -w '%{http_code}' "$u")  $u"
done
```

Within 24 hours:

- Click every link inside the rendered README on github.com to verify the
  Markdown links work.
- Open the docs/ files via the GitHub UI and confirm tables render.

Within 1 week:

```bash
# Did Google start indexing the new repo?
# Run this in the browser, not curl, because Google requires JS:
#   site:github.com/Dusangrm/legacydoc-ai
#   site:github.com Dusangrm legacydoc-ai LegacyDoc AI
```

Within 2–4 weeks:

- GA4 → Reports → Acquisition → Traffic acquisition → look for a
  `referral` source `github.com`
- GSC → Performance → Search results → look for queries containing
  `legacydoc ai`
- Ahrefs / Webmaster tools → Backlinks profile → confirm the new GitHub
  repo appears as a referring domain to `www.romanticode.com`

---

## 8. Things explicitly NOT to do in this batch

- Do not push the existing extension repo `Dusangrm/legacy-doc-ai` to
  public. Source code stays private until a separate, intentional decision.
- Do not bump VS Code extension version `0.2.2 → 0.2.3` just to align with
  this checklist. Keep version bumps for real product changes.
- Do not create a GitHub organization to "look bigger". Personal account is
  enough at this scale.
- Do not import any of your private repo files (icons, screenshots, code
  snippets) without confirming they are safe to publish. The public
  repository must remain documentation-only.

---

## 9. If you want to delay publishing

It is fine to keep this draft local for another sprint. The benefit of
publishing is:

- One more high-domain-authority page (`github.com/...`) linking to your
  canonical URLs
- A stable, citable URL for directory submissions
- A discoverable answer for `site:github.com legacydoc ai` searches

The risk of publishing prematurely is:

- A weak README that gets cached by Google before you polish it

This draft is ready to ship. Polish opportunities are minor (LICENSE
choice, optional `topics` on the GitHub repo settings page, optional
banner image). They do not block the first push.
