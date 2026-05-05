# FORRT — Framework for Open and Reproducible Research Training

[forrt.org](https://forrt.org) · [@FORRTproject](https://twitter.com/FORRTproject) · forrtproject@gmail.com

FORRT is a global, volunteer-run initiative working to advance open and
reproducible research practices in higher education. This page is a
**work-in-progress map of the GitHub organisation** — what lives here,
who maintains what, and how things are (loosely) named. PRs welcome.

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

- [`FReD`](https://github.com/forrtproject/FReD) — the R package
- [`FReD-data`](https://github.com/forrtproject/FReD-data) — the underlying dataset and ingest pipeline
- [`FReD-apps`](https://github.com/forrtproject/FReD-apps) — JS apps using FReD / FLoRA
- [`fred_explorer`](https://github.com/forrtproject/fred_explorer) — Shiny explorer
- [`fred_litsearch`](https://github.com/forrtproject/fred_litsearch) — reproducible literature search pipeline
- [`fred_repl_extractor`](https://github.com/forrtproject/fred_repl_extractor) — extract replication metadata from articles
- [`fred_preprint_processor`](https://github.com/forrtproject/fred_preprint_processor) — extract references and replications from preprints

### Replications — FLoRA (Library of Replication Attempts)

A complementary, broader library of replication attempts and tooling that
surfaces it in researchers' workflows.

- [`flora-extractor`](https://github.com/forrtproject/flora-extractor) — extraction pipeline
- [`flora-explorer`](https://github.com/forrtproject/flora-explorer) — dashboard
- [`flora-replication-atlas`](https://github.com/forrtproject/flora-replication-atlas) — landing pages per original DOI
- [`flora_zotero`](https://github.com/forrtproject/flora_zotero) — Zotero plugin (privacy-first local matching)
- [`flora_chromium`](https://github.com/forrtproject/flora_chromium) — browser extension
- [`flora_preprint_notifier`](https://github.com/forrtproject/flora_preprint_notifier) — notify authors of potentially-missing replications
- [`flora_preprint_notifier_analysis`](https://github.com/forrtproject/flora_preprint_notifier_analysis) — trial analysis
- [`flora-pubpeer`](https://github.com/forrtproject/flora-pubpeer) — PubPeer integration

### Replications — other

- [`replicatethis`](https://github.com/forrtproject/replicatethis) — moderated nomination of findings to replicate
- [`rjf`](https://github.com/forrtproject/rjf) — Replication Journal Federation
- [`journalranking`](https://github.com/forrtproject/journalranking) — rank journals by replication rate
- [`marco`](https://github.com/forrtproject/marco) — Making Replications Count
- [`replication_handbook`](https://github.com/forrtproject/replication_handbook) — Quarto book
- [`LoveReplicationsWeek`](https://github.com/forrtproject/LoveReplicationsWeek) — annual outreach event

### Website & public-facing

- [`forrtproject.github.io`](https://github.com/forrtproject/forrtproject.github.io) — main website
- [`webpage-staging`](https://github.com/forrtproject/webpage-staging) — staging renders for site PRs
- [`lighthouse`](https://github.com/forrtproject/lighthouse), [`lighthouse-v1`](https://github.com/forrtproject/lighthouse-v1) — Lighthouse newsletter / portal
- [`forrt-templates`](https://github.com/forrtproject/forrt-templates) — branded templates for FORRT outputs

### Educational resources

- [`open-research-course`](https://github.com/forrtproject/open-research-course)
- [`open-social-psychology`](https://github.com/forrtproject/open-social-psychology)
- [`handbook`](https://github.com/forrtproject/handbook)
- [`Transform-to-Open-Science-Book`](https://github.com/forrtproject/Transform-to-Open-Science-Book)
- [`best-practices-psychology`](https://github.com/forrtproject/best-practices-psychology)
- [`glossary-research`](https://github.com/forrtproject/glossary-research)
- [`re-searchterms`](https://github.com/forrtproject/re-searchterms) — explore variation in open-science terminology

### Community mapping

- [`Map_Community`](https://github.com/forrtproject/Map_Community) — FORRT community map
- [`mapping-open-science-organizations`](https://github.com/forrtproject/mapping-open-science-organizations)

### Games & outreach

- [`Open-Research-Games-Portal`](https://github.com/forrtproject/Open-Research-Games-Portal)
- [`TenureRun`](https://github.com/forrtproject/TenureRun)

### Archived / historical

- [`TOPS-archive`](https://github.com/forrtproject/TOPS-archive) — Transform to Open Science project, snapshot March 2025
- [`fredAnnotator`](https://github.com/forrtproject/fredAnnotator) — superseded annotation tool

---

## Naming conventions

There is no single enforced convention yet — the table below describes what
*is*, not what *should be*. Suggestions for consolidating are welcome.

| Prefix / pattern | Used for |
| --- | --- |
| `FReD*` / `fred_*` | FReD ecosystem (mixed case; `FReD` core, `fred_*` snake_case for tooling) |
| `flora-*` / `flora_*` | FLoRA ecosystem (kebab- and snake-case both appear) |
| `forrt-*` | Org-level assets (templates etc.) |
| `*-archive` | Snapshotted, no-longer-active projects |
| kebab-case | Default for new general-purpose repos |

When starting a new repo, prefer:

1. **Project-family prefix** if it belongs to one (`fred_`, `flora_`, …) — match the existing case style of that family.
2. **kebab-case** otherwise.
3. A short [description and topic tags](https://github.blog/2017-01-31-introducing-topics/) so it surfaces in the repo list.

---

## Contributing

- New to FORRT? Start at [forrt.org/getinvolved](https://forrt.org/getinvolved/).
- Found something out of date on this page? Open a PR against
  [`forrtproject/.github`](https://github.com/forrtproject/.github) — this
  README is rendered on the org profile.
- For project-specific contributions, see the README of the relevant repo.
