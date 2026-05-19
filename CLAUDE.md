# CLAUDE.md - Persistent Context for the RDC Knowledge Base

This file is loaded into Claude's context whenever a session involves this repository. It carries the long-term context that doesn't fit in session-scoped memory.

## Owner

- **Brian Jensen** (`brianjensen-rdc` on GitHub) - Head of People + Operations at Red Door Collaborative
- Sole authoring owner for SOPs and project deliverables in this repo
- Reviewer chain (collaborative, not gatekeeping): Chris Telfer -> Naj Yosof -> Karin Hokanson + Silas Varga -> Devin Richards -> Discipline Leads (Joy, Justine, Nathan)

## Repository Purpose

Personal/organizational knowledge base for Claude-assisted work at RDC. Holds project context, conversation outputs, reference materials, and the canonical RDC design system. Modeled after Joe Garvin's PARA-style knowledge base.

## Structure

- `projects/` - Active client and internal work projects (one folder per project)
- `areas/` - Ongoing responsibilities and recurring contexts
- `resources/` - Reference material, frameworks, prompt libraries, research
- `docs/` - Documentation, guides, and the canonical RDC design system
- `archive/` - Completed projects and historical context
- `meta/` - System notes, conventions, changelog, repository guidelines

## Conventions

- File names: lowercase, hyphenated, descriptive (e.g., `file-taxonomy-implementation-plan.md`)
- Each substantive file opens with a brief header comment indicating creation date and originating session/project
- All HTML deliverables MUST use the design system at `docs/rdc-design-system.html` (Coral, Squid, Wine, Mist; DM Sans typography; the component library)
- Markdown is the default for working documents; HTML is for review/distribution artifacts

## Active Projects (current state)

- **file-taxonomy** - RDC File Taxonomy & Organization SOP. Current phase: foundation/baselining complete, SOP authoring next. See `projects/file-taxonomy/`.

## Design System

`docs/rdc-design-system.html` is the canonical source. Brand colors:
- Coral `#FF4F58` - primary CTA, accents
- Squid `#0D1724` - dark surfaces, authority type
- Wine `#7F0046` - secondary brand
- Mist `#ABDCE0` - accent only (never primary bg)

Typography: DM Sans (web stand-in for Suisse Int'l). Page background `#F7F6F4`.

## Encrypted Document Distribution

Some HTML deliverables in `docs/` are encrypted with StatiCrypt-style password protection so they can be hosted on public GitHub Pages while restricting access. The password is shared via private channels (not committed here).

## How to Update This File

When the project list, conventions, or design system change materially, update this file. Future Claude sessions read this on load.
