Content for [mathiassm.dev](https://mathiassm.dev)
================================================================================

This repository contains all/most content used to build my personal website [mathiassm.dev](https://mathiassm.dev). I currently use a static site generator ([MathiaSM/hakyll-site](https://github.com/MathiasSM/hakyll-site)) to build it. It requires some minimal structure and metadata which I'll explain in this readme file.

Structure
--------------------------------------------------------------------------------

- `config`: Build configuration, automation checks and so on. Not content related, but development/deployment related. It may include linter configuration, accessibility checkers, etc.
- `data`: Yaml files holding reusable data in pages and templates. Each has their own schema file for LSPs.
- `writings`: Where the written content lives, in the form of markdown files (other markup languages may be used, as long as they can be processed by pandoc). The structure within is ignored by the generator, as all metadata is within yaml frontmatter blocks within each file. This frontmatter is explained later in this document.
- `media`: Where images (icons, photos, etc) live, and where other media files might eventually live. Structure is reflected in the final website. Svg files get some special treatment since they are plain-text files, so that I can inline them into pages/templates/etc.
- `projects`: YAML files, each defining a "project" to showcase; I'll probably eventually turn this into normal written content, even if mostly empty and frontmatter-driven.


Frontmatter in markup files
--------------------------------------------------------------------------------

See <https://github.com/MathiasSM/hakyll-site/blob/master/README.md>.
