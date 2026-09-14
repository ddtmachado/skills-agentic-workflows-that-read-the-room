---
name: update-github-info
description: Keep the GitHub Info website current with practical, source-backed updates.
strict: true

on:
  schedule: daily
  workflow_dispatch:

permissions:
  contents: read
  metadata: read

tools:
  github:
    mode: local
    toolsets: [repos]
  edit: true
  web-fetch: {}

network:
  allowed:
    - defaults
    - github
    - github.blog
    - github.com
    - awesome-copilot.github.com

safe-outputs:
  create-pull-request:
    base-branch: main
    draft: false
    reviewers: [mona]
    allowed-files:
      - site/content/github-info.md
---

Read `notes/mona-notes.md` using the GitHub repository read tools before making any changes.

Fetch and review all of these public sources:

- https://github.blog/latest/
- https://github.blog/changelog/
- https://awesome-copilot.github.com/workflows/

Use the notes and the fetched sources to identify concise, practical updates that help
developers learn GitHub faster. Update only `site/content/github-info.md`, keeping the
content source-backed and mentioning whether each update comes from the GitHub Blog,
GitHub Changelog, or Awesome Copilot Workflows.

When there is a meaningful update, use the `create-pull-request` safe output to open a
pull request against `main` for Mona to review. Do not write directly to `main`, and do
not modify any other file. If there is no meaningful update or the sources are
unavailable, make no file changes and call `noop` with a short reason.
