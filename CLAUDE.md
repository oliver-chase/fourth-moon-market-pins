> Framework rules (voice, practice, gates and skill placement) load on their own from
> `~/.claude/CLAUDE.md`, which links into OliverCode. To read a file in OliverCode, resolve its
> path with `dirname "$(readlink ~/.claude/CLAUDE.md)"`. This file holds only what is specific
> to this repo.

# fourth-moon-market-pins — Agent rules

Read before working here:
- `README.md`: this repo is the public mirror of the shop's finished pin images and guide pages, served as a static site
- `docs/repo-structure-contract.md`: the folders and the contract exceptions
- `docs/backlog-config.json`: this repo has no board of its own. It points at the shop repo, fourth-moon-market, so `#N` in a commit names a shop story

Run `bash scripts/validate.sh` before every commit. It is this repo's canonical validation.

Rules:
- The originals live in the shop repo. Change an image or page there, then copy the finished file here
- Everything here is public: no drafts, no shop data, no account identifiers
- An owner request that changes files is filed as a story with Gherkin criteria under an epic before work starts, per the `backlog` skill. A small change, as RULES.md "The backlog" defines it, needs no story and cites the open epic's number in its commit. There is no QA phase and no pull request: the builder makes a quick pass, runs validation, then commits, pushes and merges at the end of the work without being asked, and a different agent QAs only when the owner requests it
