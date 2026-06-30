# Catalog Schema

`catalog.js` is the single source of truth for the GitHub Pages homepage.

Add one object per useful item:

```js
{
  id: "short-stable-id",
  title: "Human readable title",
  href: "items/topic-name/file.html",
  kind: "page",
  area: "concept",
  status: "ready",
  updated: "2026-06-30",
  owner: "Jacky",
  featured: false,
  summary: "One sentence explaining why this item exists.",
  tags: ["tag one", "tag two"]
}
```

Accepted `kind` values:

- `page`
- `file`
- `notebook`

Current `area` values:

- `concept`
- `interview`
- `architecture`
- `validation`
- `evidence`

Use `status: "draft"` when a page is not polished yet. Use `status: "archive"` for older material you want to keep but no longer feature.
