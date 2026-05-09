# Contributing to UnfoldCMS

Thanks for your interest in contributing.

This repository is a **read-only mirror** of the core UnfoldCMS codebase. The actual development happens in a private repository, and we publish synchronized snapshots here on each release. This means:

- ✅ Issues are read and triaged
- ✅ Discussions are welcome
- ✅ Patches submitted as diffs in Issues/Discussions are reviewed and may be incorporated upstream
- ❌ Pull requests are **not accepted directly** on this mirror — they cannot be merged because the source of truth is upstream

This isn't a slight on contributors — it's a constraint of the source-available license. The same model is used by Sentry, Mattermost, GitLab Enterprise, and other source-available projects.

---

## How to report a bug

1. Search [existing issues](https://github.com/hpakdaman/unfoldcms/issues) to make sure it's not already filed
2. [Open a new issue](https://github.com/hpakdaman/unfoldcms/issues/new) with:
   - **Version** of UnfoldCMS you're running (find it in `composer.json` or the admin "About" page)
   - **PHP version** and **Laravel version**
   - **Database** (MySQL/MariaDB/SQLite + version)
   - **Steps to reproduce** — be specific, include URLs or admin paths
   - **Expected behavior**
   - **Actual behavior**
   - **Logs** if relevant (`storage/logs/laravel.log` — redact sensitive data)
   - **Screenshots** if it's a UI bug

The faster we can reproduce, the faster we can fix.

## How to suggest a feature

[Start a Discussion](https://github.com/hpakdaman/unfoldcms/discussions). Explain:

- What problem you're trying to solve
- What you've tried so far
- What "done" looks like for you

We treat Discussions seriously — most roadmap items started as Discussions.

## How to submit a patch

Since we can't accept PRs on the mirror, the patch flow is:

1. **Find or open an Issue** describing the bug or improvement
2. **Comment on the Issue** with your proposed change as a code diff (paste the patch directly, or link to a fork)
3. **Wait for review** — we aim to respond within 5 business days
4. If accepted, we'll incorporate the patch upstream and credit you in the release notes

For larger changes (more than ~50 lines), open a Discussion first to align on the approach before writing code.

## Code style

If you're submitting a patch, follow the existing code style:

- **PHP:** Laravel Pint (Laravel's opinionated wrapper around PHP CS Fixer). Run `vendor/bin/pint` if you're working in a fork.
- **TypeScript:** ESLint + Prettier. Run `pnpm run lint` and `pnpm run types`.
- **Commit messages:** Imperative mood, short subject line, optional body explaining "why" (not "what").

## What kinds of contributions we love

- **Bug reports with reproduction cases.** The single most valuable contribution.
- **Documentation improvements.** Typos, clarifications, missing examples — all welcome.
- **Translations.** UnfoldCMS supports multi-language; translation contributions for the admin UI are highly valued.
- **Performance fixes.** Identified slow queries, N+1 issues, large bundle sizes.
- **Security disclosures.** See below.

## What we can't accept

- **Cosmetic refactors with no behavior change.** Style preferences vary; we keep the codebase consistent rather than churning.
- **Architectural rewrites without prior alignment.** Open a Discussion first.
- **Plugins or extensions for specific use cases.** UnfoldCMS uses Laravel service providers for extension; we don't ship a plugin marketplace.
- **License changes.** UnfoldCMS is source-available, not open-source. We won't relicense.

## Security disclosures

**Don't open a public Issue for security vulnerabilities.** Email security details to:

```
security@unfoldcms.com
```

We'll acknowledge within 48 hours and work on a fix. Responsible disclosures are credited in release notes (with the reporter's permission).

## Code of conduct

Be kind, be specific, be patient. Reviews and triage take time — we're a small team. Disagreements are fine; rudeness isn't.

By participating in Issues, Discussions, or any other space connected to this project, you agree to behave professionally and respectfully toward other contributors.

---

Thanks for helping make UnfoldCMS better.
