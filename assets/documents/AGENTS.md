# Project Role: Jekyll Webmaster & SEO Assistant

## Technical Stack
- Jekyll (Static Site Generator)
- Liquid Templating Engine
- Markdown Front-Matter
- Zed Editor Environment

## Workflow Constraints
1. **Sandboxing:** You are authorized to make edits within this project folder workspace (`workspace` permission mode). Do not touch files outside of this project repository.
2. **Drafting Content:** All new blog articles must be placed in the `_posts/` directory. File names must strictly follow the `YYYY-MM-DD-title.md` format.
3. **YAML Front-Matter:** Published Markdown content must include valid front matter with `layout`, `title`, a concise `description`, and `tags`. Aim for descriptions under 160 characters as an editorial convention, not a search-engine limit. Repository documentation and GitHub templates are exempt. Exclude internal documentation from the generated site.

## SEO & Content Rules
- **Alt Tags:** Give informative images purpose-appropriate alternatives; use `alt=""` for decorative images. Complex graphics need equivalent text for their meaningful information.
- **Permalink Checks:** Ensure permalinks do not break historical patterns.
- **JSON-LD:** If asked to build schema markup, use standard Liquid parameters to drop structured JSON-LD data into the site header.

## Scope and ownership
- This repository owns the public Kaffeinated Kodemonkey Jekyll website, within the wider KKM-AI-Assist-Platform business initiative.
- Retain Jekyll, Liquid, existing hosting, and the current design foundation. Make focused improvements; do not migrate frameworks, redesign the entire site, or introduce paid services without an explicit request.
- Internal management, marketing automation, WEAR-TTP, and other applications have separate repositories/projects. Link dependencies to their owning repository; do not implement their backends here.
- vtiger owns client records and client-facing workflows. osTicket owns internal tasks/support workflows. GitHub owns software issues and implementation evidence. Do not duplicate their records in the public site.
- Never commit credentials, private client information, raw analytics exports, or unpublished audit evidence to this public repository.

## Start every implementation
1. Read applicable instructions; inspect the current branch, status, relevant source, and issue history. Preserve unrelated changes.
2. Only Heather may modify `main` or `master`; Codex may inspect them read-only. Before any local write, verify the current branch. If `main` or `master` is checked out, stop and give Heather the exact command to create or switch to a feature branch. Codex must not edit, stage, commit, merge, rebase, cherry-pick, reset, or otherwise modify either branch; push to either branch (including explicit refspecs); merge PRs into either; delete either; or change/bypass branch protections. General authorization such as “continue” does not override this restriction. For an action affecting either branch, explain it and provide Heather the exact command to run herself. This is an agent behavior rule, not an enforceable GitHub restriction; only claim remote protection after verifying settings.
3. Identify the issue and acceptance criteria. Reuse existing includes, layouts, styles, plugins, and content conventions.
4. Inspect existing GitHub projects, milestones, labels, and issues before creating equivalents. Do not invent issue numbers or claim remote writes without confirmation.
5. Work on a focused branch. Do not force-push, merge, or deploy unless authorized. Document the actual deployment path before changing it.

## GitHub work accounting
- Record work under the relevant issue as it proceeds: changes, related fixes, verification, limitations, and next steps.
- Fix small related defects within the current issue when appropriate and document them. Create a linked issue for independent or deferred work; avoid duplicates.
- If work pauses, leave the issue open and state what remains and what blocks it. Use Blocked when an external dependency prevents progress.
- Close only when acceptance criteria are met and verification evidence is recorded. Implementation alone is not a pass for manual accessibility or production behavior.
- Cross-repository work gets a linked handoff in its owning repository when access exists; otherwise provide the proposed issue and explicitly report that it has not been created.
- Suggested board states: Backlog, Ready, In Progress, Verification, Blocked, Done. Done requires verified closure, not just a commit.

## Accessibility requirements
- Target WCAG 2.2 Level AA. Use native semantic HTML before ARIA; preserve names, roles, states, labels, landmarks, and meaningful reading order.
- Verify affected keyboard paths, visible focus, focus order, skip links, mobile navigation, zoom/reflow, contrast, forms and errors, and screen-reader behavior.
- Use automated checks as supporting evidence, never as proof of conformance. Record page, environment, date, steps, observed result, expected result, criterion, severity, and retest status.
- Report untested NVDA/VoiceOver and browser checks as unverified. Do not claim certification, complete conformance, or legal protection from a scan or partial review.

## Content and search requirements
- Explain the buyer's problem, service scope, deliverables, exclusions, and next action before introducing POCC, WEAR, VPAT/ACR, or other report names.
- Keep prices, package scope, credentials, client outcomes, testimonials, and regulatory statements grounded in approved/current evidence. Flag unresolved business decisions; do not invent them.
- Preserve published URLs and case-sensitive paths. Before a URL change, inventory inbound/internal links, select the canonical destination, and verify a redirect supported by the actual host. Do not assume plugins or server redirects work on GitHub Pages.
- Maintain one authoritative title/description/canonical path through existing metadata tooling. Keep sitemap entries limited to intended indexable URLs; distinguish expected exclusions from indexing defects.
- Prefer improving existing relevant content over producing a large new publishing backlog. Link educational pages to a useful service and inquiry route.

## Verification and handoff
- Edit source, not `_site/`. It contains tracked generated files: do not mass-delete or regenerate them until deployment ownership is established.
- Use the pinned Ruby version and existing bundle. Run `bundle exec jekyll build` to an isolated temporary destination, plus focused HTML/link/accessibility checks appropriate to the change. Do not upgrade dependencies incidentally.
- Validate rendered output, not only Liquid source. Keep source links, fragments, asset paths, forms, mobile navigation, and important existing content working.
- Distinguish source inspection, automated rendered checks, manual browser tests, assistive-technology tests, and production verification in reports.
- If tools or credentials are unavailable, record the blocked check and exact next action. Never label it passed.
