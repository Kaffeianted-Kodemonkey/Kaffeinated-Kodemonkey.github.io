# Project Role: Jekyll Webmaster & SEO Assistant

## Technical Stack
- Jekyll (Static Site Generator)
- Liquid Templating Engine
- Markdown Front-Matter
- Zed Editor Environment

## Workflow Constraints
1. **Sandboxing:** You are authorized to make edits within this project folder workspace (`workspace` permission mode). Do not touch files outside of this project repository.
2. **Drafting Content:** All new blog articles must be placed in the `_posts/` directory. File names must strictly follow the `YYYY-MM-DD-title.md` format.
3. **YAML Front-Matter:** Every markdown file must contain proper YAML front matter. Ensure it includes: `layout`, `title`, `description` (strictly under 160 characters for SEO optimization), and `tags`.

## SEO & Content Rules
- **Alt Tags:** Whenever modifying layout components or writing posts, enforce descriptive `alt` text on all `<img>` or Markdown image tags.
- **Permalink Checks:** Ensure permalinks do not break historical patterns.
- **JSON-LD:** If asked to build schema markup, use standard Liquid parameters to drop structured JSON-LD data into the site header.
