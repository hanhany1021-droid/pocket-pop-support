# Contributing

Read `docs/PROJECT_CONTEXT.md` before changing policy language, support routes, hosting, or repository visibility.

## Change rules

- Keep the site static and dependency-free unless a documented decision changes that boundary.
- Never add the private Pocket Pop source, credentials, reviewer details, user records, analytics, or local build artifacts.
- Verify privacy claims against the current app before publishing them.
- Update `docs/PROJECT_CONTEXT.md` for durable scope or boundary changes, `docs/ROADMAP.md` for priorities, and append to `docs/DECISIONS.md` for consequential choices.

## Validation

- Open each HTML page and follow every internal link.
- Confirm the GitHub Pages URLs load without authentication.
- Check responsive readability at narrow and desktop widths.
- Run `git diff --check` and review the exact staged files.
- Check added files for credentials or private artifacts before committing.
