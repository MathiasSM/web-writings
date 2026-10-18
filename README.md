Content for [mathiassm.dev](https://mathiassm.dev)
================================================================================

This repository contains all/most content used to build my personal website [mathiassm.dev](https://mathiassm.dev). I currently use a static site generator ([MathiaSM/hakyll-site](https://github.com/MathiasSM/hakyll-site)) to build it. It requires some minimal structure and metadata which I'll explain in this readme file.

Structure
--------------------------------------------------------------------------------

- `config`: Build configuration, automation checks and so on. Not content related, but development/deployment related. It may include linter configuration, accessibility checkers, etc.
- `tables`: TSV files that define some data-driven logic in the site generator; i.e. the generation of HTML snippets, lists, or metadata needed for other pages.
- `hobbies.yaml`: A single YAML file listing every hobby, each with `name`, `href`, `icon` and an optional `show` flag (a hobby is shown unless `show: false`). Editors can validate it against `schema/hobbies.schema.json` (see the modeline comment at the top of the file).
- `writings`: Where the written content lives, in the form of markdown files (other markup languages may be used, as long as they can be processed by pandoc). The structure within is ignored by the generator, as all metadata is within yaml frontmatter blocks within each file. This frontmatter is explained later in this document.
- `media`: Where images (icons, photos, etc) live, and where other media files might eventually live. Structure is reflected in the final website. Svg files get some special treatment since they are plain-text files, so that I can inline them into pages/templates/etc.
- `projects`: YAML files, each defining a "project" to showcase; I'll probably eventually turn this into normal written content, even if mostly empty and frontmatter-driven.


Frontmatter in markup files
--------------------------------------------------------------------------------

This documentation should probably live in the site generator...

### Required fields for publication


| Key     | Required | Meaning                                           |
| ---     | ---      | ---                                               |
| `path`  | yes      | Output URL, e.g. `/blog/my-post`                  |
| `title` | yes      | Post title. Used in `h1` and head `title`         |
| `date`  | yes      | Published date (`YYYY-MM-DD`); used for ordering. |

### Common optional fields

| Key               | Meaning                                                                  |
| ---               | ---                                                                      |
| `lastModifiedAt`  | Similar to `date`. Used to show "last updated" info on the site and in the sitemap. |
| `description`     | Short summary: post lists and `<meta name="description">`.               |
| `hideDescription` | `true` to hide the description on the posts list page.                   |
| `language`        | `en` (default), `es` or `jp`; sets the page language (semantic HTML).    |
| `TOC`             | `true` to show a table of contents.                                      |
| `type`            | Kind of post (currently only `escrito`).                                 |
| `project`         | Project name the post relates to. Makes the project link to this post.   |


### Group index pages 

Any file with this set becomes the index file for the given group.

| Key     | Notes                           |
| ---     | ---                             |
| `group` | The name of the group           |
| `index` | For index pages, must be `true` |


