# Repository Conventions

## File Naming

- All-lowercase, hyphenated, descriptive
- Good: `file-taxonomy-implementation-plan.md`, `q3-marketing-recap.md`
- Avoid: `FileTaxonomyImplementationPlan.md`, `q3 marketing recap.md`, `Doc.md`

Note: this is the **repo convention**, distinct from the SharePoint file convention (which uses PascalCase descriptors and hyphen-separated taxonomic rank). Repo audience is Brian-with-Claude; SharePoint audience is the whole org.

## Header Comments

Each substantive file opens with a brief block indicating:

- **Created:** YYYY-MM-DD
- **Project / Session:** which project or conversation this came out of
- **Author:** Brian, Claude (with Brian), or other
- **Status:** draft / in review / final / archived

Example (top of a Markdown file):

```markdown
<!--
Created: 2026-05-19
Project: file-taxonomy
Author: Brian Jensen (with Claude)
Status: draft v2
-->
```

## Folder Usage

- `projects/<project-name>/` - One folder per active project. Internal structure is project-driven; common pattern is `plan.md`, `baseline.md` or similar, plus a `deliverables/` subfolder for shipped artifacts.
- `areas/` - Standing responsibilities (HR, Ops, account management, etc.). Files document ongoing context that doesn't belong to a discrete project.
- `resources/` - Reference frameworks, prompt libraries, research excerpts. Things you reach for repeatedly.
- `docs/` - Guides, instructional content, and the canonical RDC design system.
- `archive/` - Completed projects move here. Preserves structure.
- `meta/` - This file, the changelog, and any repo-governance artifacts.

## HTML Deliverables

All HTML produced for distribution MUST use the design system at `docs/rdc-design-system.html`:

- Colors: Coral `#FF4F58`, Squid `#0D1724`, Wine `#7F0046`, Mist `#ABDCE0`
- Typography: DM Sans (web), Suisse Int'l (print/design)
- Components: page-header hero with decorative "rd", content cards with colored top bars, pill badges, tinted alert callouts

## Encrypted Distribution

Some HTML files are encrypted (password-gated) and live under `docs/<project>-encrypted/`. Source HTML stays in the project folder; encrypted versions are committed for GitHub Pages serving. Passwords are shared out-of-band.

## Changelog

Update `meta/changelog.md` with each meaningful change. Date-stamped entries, newest at top.
