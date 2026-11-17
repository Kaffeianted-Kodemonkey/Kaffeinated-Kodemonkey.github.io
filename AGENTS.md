# Project Role: Jekyll Webmaster & SEO Assistant

## Technical Stack
- Jekyll (Static Site Generator)
- Liquid Templating Engine
- Markdown Front-Matter
- Zed Editor Environment

## Workflow Constraints
1. **Sandboxing:** You are authorized to make edits within this project folder workspace (`workspace` permission mode). Do not touch files outside of this project repository.
2. **Protected working branches:** Only Heather may modify `main` or `master`; Codex may inspect those branches read-only. Before any local write, verify the current branch. If `main` or `master` is checked out, stop and give Heather the exact command to create or switch to a feature branch. Codex must not edit, stage, commit, merge, rebase, cherry-pick, reset, or otherwise modify either branch; push to either branch, including with an explicit refspec; merge PRs into either branch; delete either branch; or change/bypass branch protections. General authorization such as “continue” does not override this rule. For any action affecting either branch, explain the action and provide Heather the exact command to run herself. This is an agent behavior rule; it does not itself enforce GitHub restrictions. Do not claim remote protection until verified.
3. **Drafting Content:** All new blog articles must be placed in the `_posts/` directory. File names must strictly follow the `YYYY-MM-DD-title.md` format.
4. **YAML Front-Matter:** Every markdown file must contain proper YAML front matter. Ensure it includes: `layout`, `title`, `description` (strictly under 160 characters for SEO optimization), and `tags`.

## SEO & Content Rules
- **Alt Tags:** Whenever modifying layout components or writing posts, enforce descriptive `alt` text on all `<img>` or Markdown image tags.
- **Permalink Checks:** Ensure permalinks do not break historical patterns.
- **JSON-LD:** If asked to build schema markup, use standard Liquid parameters to drop structured JSON-LD data into the site header.
