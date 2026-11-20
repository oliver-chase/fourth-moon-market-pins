# Repo structure contract

Status: Active

## Canonical contract sources

1. `OliverCode/docs/RULES.md` ("Project structure")
2. `OliverCode/docs/CONTRACT.md`

## Profile

This repo is a data-only mirror. Its backlog is the shop repo's GitHub Project, named in
`docs/backlog-config.json`, so its stories live in the fourth-moon-market repo.

## Required structure

1. Root docs:
- `README.md`
- `CLAUDE.md`
- `docs/repo-structure-contract.md`
2. Backlog:
- `docs/backlog-config.json` — the shop repo's Project, which tracks this mirror's work
3. Published content:
- `pins/` — finished pin images the Pinterest bulk sheets link to
- `guide/` — the public guide pages
- `resources/` — the free resource pages
- `robots.txt` and `sitemap.xml` — crawl rules and the page list

## Branches

This repo works on `main`. If it needs a development or staging branch, name it here with
what moves through it.

## Enforcement

1. `bash scripts/validate.sh`, which also runs `npm run validate` when the repo has one

## Learning loop

The shop repo owns the loop for every pin: it records each pin's date and reason, reads the results and decides. This mirror only serves the files.

## Contract exceptions

- learning: a data-only mirror; the shop repo owns the loop. Expires 2027-02-01
- board: the mirror's work is tracked on the shop repo's Project, which docs/backlog-config.json names. Expires 2027-02-01
- tests: the only code is the fleet's own gate scripts, which OliverCode tests. Expires 2027-02-01
- docs: the README states the mirror's purpose, and the GitHub About text waits for the owner. Expires 2027-02-01
