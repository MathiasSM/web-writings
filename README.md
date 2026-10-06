# Post frontmatter

Posts live in `data/posts/<group>/` (`blog`, `escritos`). This README is outside
those globs, so Hakyll does not process it.

| Key | Required | Meaning |
| --- | --- | --- |
| `title` | yes | Post title. |
| `date` | yes | Published date (`YYYY-MM-DD`); used for ordering. |
| `path` | yes | Output URL, e.g. `/blog/my-post` (the route comes from here). |
| `description` | no | Short summary: post lists and `<meta name="description">`. |
| `lastModifiedAt` | no | Shows a "last updated" line and the sitemap `lastmod`. |
| `language` | no | `en` (default), `es` or `jp`; sets the page language. |
| `TOC` | no | `true` to show a table of contents. |
| `hideDescription` | no | `true` to hide the description on the post page. |
| `type` | no | Kind of post (currently only `escrito`). |
| `project` | no | Project name the post relates to (e.g. `Apolo`). |
