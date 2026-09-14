# GitHub Info

## Mona's editorial angle

Mona's website focuses on practical GitHub guidance backed by official references from:

- docs.github.com
- github.blog
- github.blog/changelog

## Current homepage themes

- GitHub collaboration basics: repositories, branches, pull requests, and merges.
- GitHub Copilot as an AI coding assistant across the IDE, CLI, and GitHub.
- GitHub Actions as the automation layer behind repository workflows.
- Recent GitHub Blog and Changelog stories worth watching.

## Latest practical updates

- **Refreshed repository pull requests page** (public preview): the PR list page now has better filtering, search, and a compact view, making it easier to triage large PR queues. *(Source: GitHub Changelog)*
- **Block pull requests with exposed secrets from merging**: a new repository ruleset option stops PRs containing detected secrets from being merged, adding a safety net on top of secret scanning. *(Source: GitHub Changelog)*
- **GitHub CLI supports media in issues, PRs, and comments**: `gh` now has an `--attach` option to add inline images and video directly from the command line. *(Source: GitHub Changelog)*
- **Control GitHub Actions cache access with `cache-mode`** (GA): workflows can now set least-privilege cache permissions (read, write, write-only, or none) to help prevent cache-poisoning attacks. *(Source: GitHub Changelog)*
- **Copilot code review can now approve pull requests**: Copilot's automated review can formally approve a PR, not just leave comments, speeding up routine review cycles. *(Source: GitHub Changelog)*
- **Configure cost vs. quality in Copilot's auto model selection**: new efficiency/balance/intelligence tiers let teams trade off cost, quality, and latency for Copilot requests. *(Source: GitHub Changelog)*
- **Awesome Copilot Workflows catalog**: the `github/awesome-copilot` workflows collection includes ready-made agentic workflows such as `daily-issues-report`, `ospo-org-health` (stale issue/PR and contributor reports), and `weekly-comment-sync` (finds and fixes stale code comments via a draft PR) — useful starting points for automating repository maintenance. *(Source: Awesome Copilot Workflows)*
