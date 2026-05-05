# FORRT — Framework for Open and Reproducible Research Training

[forrt.org](https://forrt.org) · forrtproject@gmail.com

FORRT is a global, volunteer-run initiative working to advance open and
reproducible research practices in higher education. This page is a
**work-in-progress map of the GitHub organisation** — what lives here,
who maintains what, and how things are named. PRs welcome.

---

## Teams

| Team | Remit |
| --- | --- |
| [Operations Committee](https://github.com/orgs/forrtproject/teams/operations-committee) | Cross-cutting coordination across FORRT projects |
| [FORRT Engineering](https://github.com/orgs/forrtproject/teams/forrt-engineering) | Development and infrastructure across FORRT tools |
| [Team Replications](https://github.com/orgs/forrtproject/teams/team-replications) | Replication-focused projects (FReD, FLoRA, RJF, …) |
| [Team Website](https://github.com/orgs/forrtproject/teams/team-website) | [forrt.org](https://forrt.org) maintenance |
| [Team AWoP](https://github.com/orgs/forrtproject/teams/team-awop) | Academic Wheel of Privilege |

Most projects also have their own informal working groups that aren't
modelled as GitHub teams. If you want to get involved, the
[forrt.org get-involved page](https://forrt.org/getinvolved/) is the
best starting point.

---

## Repository clusters

Repos are loosely grouped by project family. Names below are not exhaustive —
see the full [repository list](https://github.com/orgs/forrtproject/repositories).

### Replications — FReD (FORRT Replication Database)

A curated database of replication attempts plus the tooling around it.

- [`fred`](https://github.com/forrtproject/fred) — the R package
- [`fred-data`](https://github.com/forrtproject/fred-data) — the underlying dataset and ingest pipeline
- [`fred-apps`](https://github.com/forrtproject/fred-apps) — JS apps using FReD / FLoRA
- [`fred-explorer`](https://github.com/forrtproject/fred-explorer) — Shiny explorer
- [`fred-litsearch`](https://github.com/forrtproject/fred-litsearch) — reproducible literature search pipeline
- [`fred-repl-extractor`](https://github.com/forrtproject/fred-repl-extractor) — extract replication metadata from articles
- [`fred-preprint-processor`](https://github.com/forrtproject/fred-preprint-processor) — extract references and replications from preprints

### Replications — FLoRA (Library of Replication Attempts)

A complementary, broader library of replication attempts and tooling that
surfaces it in researchers' workflows.

- [`flora-extractor`](https://github.com/forrtproject/flora-extractor) — extraction pipeline
- [`flora-explorer`](https://github.com/forrtproject/flora-explorer) — dashboard
- [`flora-replication-atlas`](https://github.com/forrtproject/flora-replication-atlas) — landing pages per original DOI
- [`flora-zotero`](https://github.com/forrtproject/flora-zotero) — Zotero plugin (privacy-first local matching)
- [`flora-chromium`](https://github.com/forrtproject/flora-chromium) — browser extension
- [`flora-preprint-notifier`](https://github.com/forrtproject/flora-preprint-notifier) — notify authors of potentially-missing replications
- [`flora-preprint-notifier-analysis`](https://github.com/forrtproject/flora-preprint-notifier-analysis) — trial analysis
- [`flora-pubpeer`](https://github.com/forrtproject/flora-pubpeer) — PubPeer integration
- [`plugin-notification-dummy`](https://github.com/forrtproject/plugin-notification-dummy) — test page for the plugin install-banner conditional-hide logic

### Replications — other

- [`replicatethis`](https://github.com/forrtproject/replicatethis) — moderated nomination of findings to replicate
- [`rjf`](https://github.com/forrtproject/rjf) — Replication Journal Federation
- [`journalranking`](https://github.com/forrtproject/journalranking) — rank journals by replication rate
- [`marco`](https://github.com/forrtproject/marco) — Making Replications Count
- [`replication-handbook`](https://github.com/forrtproject/replication-handbook) — Quarto book
- [`love-replications-week`](https://github.com/forrtproject/love-replications-week) — annual outreach event

### Website & public-facing

- [`forrtproject.github.io`](https://github.com/forrtproject/forrtproject.github.io) — main website
- [`webpage-staging`](https://github.com/forrtproject/webpage-staging) — staging renders for site PRs
- [`lighthouse`](https://github.com/forrtproject/lighthouse), [`lighthouse-v1`](https://github.com/forrtproject/lighthouse-v1) — Lighthouse newsletter / portal
- [`forrt-templates`](https://github.com/forrtproject/forrt-templates) — branded templates for FORRT outputs
- [`cv`](https://github.com/forrtproject/cv) — source for the FORRT CV; published PDF is auto-pushed to the site

### Educational resources

- [`open-research-course`](https://github.com/forrtproject/open-research-course)
- [`open-social-psychology`](https://github.com/forrtproject/open-social-psychology)
- [`handbook`](https://github.com/forrtproject/handbook)
- [`transform-to-open-science-book`](https://github.com/forrtproject/transform-to-open-science-book)
- [`best-practices-psychology`](https://github.com/forrtproject/best-practices-psychology)
- [`glossary-research`](https://github.com/forrtproject/glossary-research)
- [`re-searchterms`](https://github.com/forrtproject/re-searchterms) — explore variation in open-science terminology

### Community mapping

- [`map-community`](https://github.com/forrtproject/map-community) — FORRT community map
- [`mapping-open-science-organizations`](https://github.com/forrtproject/mapping-open-science-organizations)

### Games & outreach

- [`open-research-games-portal`](https://github.com/forrtproject/open-research-games-portal)
- [`tenure-run`](https://github.com/forrtproject/tenure-run)

### Archived / historical

- [`tops-archive`](https://github.com/forrtproject/tops-archive) — Transform to Open Science project, snapshot March 2025
- [`fredAnnotator`](https://github.com/forrtproject/fredAnnotator) — superseded annotation tool (archived)

---

## Naming conventions

All repos use **kebab-case** (lowercase, hyphen-separated). Project-family
prefixes group related work:

| Prefix | Used for |
| --- | --- |
| `fred-*` | FReD (FORRT Replication Database) ecosystem |
| `flora-*` | FLoRA (Library of Replication Attempts) ecosystem |
| `forrt-*` | Org-level shared assets (templates etc.) |
| `*-archive` | Snapshotted, no-longer-active projects |

Two exceptions keep non-kebab names because GitHub requires them:
[`.github`](https://github.com/forrtproject/.github) (this repo — must be
exactly `.github` to act as the org profile) and
[`forrtproject.github.io`](https://github.com/forrtproject/forrtproject.github.io)
(must match the org name to serve at that path).

Brand names in prose and READMEs use mixed case (`FReD`, `FLoRA`); the
*repository* names are always lowercase.

When starting a new repo, prefer:

1. The relevant project-family prefix if one applies (`fred-`, `flora-`, …).
2. kebab-case otherwise.
3. A short [description and topic tags](https://github.blog/2017-01-31-introducing-topics/) so it surfaces in the repo list.

---

## Contributing

- New to FORRT? Start at [forrt.org/getinvolved](https://forrt.org/getinvolved/).
- Found something out of date on this page? Open a PR against
  [`forrtproject/.github`](https://github.com/forrtproject/.github) — this
  README is rendered on the org profile.
- For project-specific contributions, see the README of the relevant repo.
