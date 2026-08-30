# R&D & R&R

Brian Herbert's blog, self-hosted at [burningaltar.com](https://burningaltar.com).

Markdown in `content/`. Hugo + [hugo-bearblog](https://github.com/janraasch/hugo-bearblog). GitHub Pages publishes on every push to `main`.

## Local preview

```sh
hugo server
```

## New post

```sh
hugo new content blog/my-slug.md
```

Then edit the file, assign 1–3 tags from the closed vocabulary, commit, and push.

## Tags

Closed set. Use lowercase slugs in frontmatter; the site displays the names below.

| Slug | Name | Use when the post is about |
| --- | --- | --- |
| `ai` | AI | Tools, models, agents, building with them |
| `family` | Family | Household, marriage, parenting, home life |
| `health` | Health | Body, medicine, food, fitness, sleep, mental health |
| `philosophy` | Philosophy | Meaning, ethics, first principles, how to think — not primarily faith |
| `theology` | Theology | God, scripture, church, practice of faith |

Rules:

- Every post gets at least one tag; usually 1–3.
- Tag the subject, not a passing mention.
- Prefer `theology` over `philosophy` when the post is about God or faith.
- Do not reuse a tag slug as a post slug (`/blog/ai/` is the AI filter).
- To add a tag: add it to `params.tagVocab` in `hugo.toml`, create `content/tags/<slug>/_index.md`, and update this table.
