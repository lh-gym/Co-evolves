# Add New Material

This repo is a static GitHub Pages knowledge base. The homepage is generated from `content/catalog.js`, so scaling it means keeping content files and catalog records tidy.

## Fast Path

1. Put the new file in a stable location.
   - One-page HTML that should keep a short URL can stay at repo root.
   - New topic folders should go under `items/topic-name/`.
   - Shared images or downloads can go under `assets/`.
2. Edit `content/catalog.js`.
3. Copy an existing object, paste it at the end of the array, and change:
   - `id`
   - `title`
   - `href`
   - `kind`
   - `area`
   - `updated`
   - `summary`
   - `tags`
4. Commit to `main`.
5. Open `https://lh-gym.github.io/Co-evolves/` after GitHub Pages refreshes.

## Naming Rules

- Use lowercase folder names: `items/sql-validation/`.
- Prefer hyphens over spaces: `audit-evidence-checklist.html`.
- Keep public URLs stable once shared in Notion or a resume.
- Do not add sensitive personal files to this public repo. Use a private repo for private resumes, IDs, contact lists, or client-confidential material.

## Catalog Example

```js
{
  id: "audit-evidence-checklist",
  title: "Audit Evidence Checklist",
  href: "items/audit-evidence/audit-evidence-checklist.html",
  kind: "page",
  area: "validation",
  status: "ready",
  updated: "2026-07-01",
  owner: "Jacky",
  featured: false,
  summary: "A checklist for explaining how validation outputs become audit evidence.",
  tags: ["audit", "dbt", "evidence", "interview"]
}
```

## What To Edit Later

- Add or reorder cards: edit `content/catalog.js`.
- Change homepage layout: edit `index.html`.
- Add a new category label: add records with a new `area`, then optionally add its display label in `index.html`.
