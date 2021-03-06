---
layout: default
title: Documentation Setup
---

# How the Docs are created & how to create more pages

The setup is fairly simple since `Jekyll` will take care of creating a
website from provided `markdown` files given a `_config.yml` file. So,
every page in the directory `docs` automatically is included.
Subdirectories of `docs` will automatically create subpages.

The detailed description of the theme and how to organize content for
`jekyll` pages is shown in the docs for [Just the
docs](`https://just-the-docs.github.io/just-the-docs`).

At a bare minimum each page has the following header:

```markdown
---
layout: default
title: <title>
---
```

Followed by normal markdown syntax. As far as I know, cross referencing
is not really supported (feel free to add explanation if it is).

For simplicity do not use the `nav_order: <int>` directive. So, no

```markdown
---
layout: default
title: <title>
`nav_order: <int>`
---
```

That way, the docs except the `Homepage` are sorted in alphabetical order.

If you want to create a subdirectory structure, please visit
[`just-the-docs`
Documentation](https://just-the-docs.github.io/just-the-docs/docs/navigation-structure)
on navigation structure. Because the markdown headers need to know
what's a parent and what not. To sort your `subdirectory` docs in a
specific order, please refer to the navigation structure documenation
as well.

The documentation are automatically built once new adds are merged
with or pushed to the `main` branch.  Note that it takes a sec to
update.

Note on images, the images have to be in a separate folder called `assets`.  For reference, see `docs/vscode/remotecodeediting.md` for usage in the text and `docs/assets/vscode/<images>` for a location example.


Happy docs writing!

