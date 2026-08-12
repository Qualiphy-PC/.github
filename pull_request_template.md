## What

<!-- pr:what -->
<!-- One or two sentences. -->

## Why

<!-- pr:why -->
<!-- Fixes #123 / JIRA-456 -->

## How

<!-- pr:how -->

## Testing

<!-- pr:testing -->

- [ ] `npm run lint` passes
- [ ] `npm test` passes
- [ ] Ran locally and exercised the change

## Database

<!-- pr:database -->
<!-- DELETE THIS SECTION if the PR has no schema changes. -->

**Migration file:**

**Backward compatible?** <!-- Old code must keep working against the new
     schema during the deploy window. If not, describe the expand → backfill
     → contract sequence and how far apart each step ships. -->

**Rollback:** <!-- down migration, or why there isn't one -->

**Lock risk:** <!-- rows affected, expected duration, hot table? -->

## Infra

<!-- pr:infra -->
<!-- DELETE THIS SECTION if the PR has no infra or config changes. -->

**What changes:** <!-- resource or config, env: dev | staging | prod -->

**Applied manually?** <!-- If you changed something in the console or CLI
     that isn't in this diff, say exactly what and where. This is the only
     record of it. -->

**New env vars or secrets:** <!-- names only, never values. Where they're set. -->

**Rollback:** <!-- how to undo, including the manual parts -->

## Cross-repo

<!-- pr:cross_repo -->
<!-- DELETE THIS SECTION if this PR ships independently. -->

**Depends on:** <!-- link PRs -->

**Deploy order:**

**Feature flagged?**

## Risk & rollback

<!-- pr:risk -->

## Checklist

- [ ] Docs/README updated if behavior changed
- [ ] No secrets, keys, or credentials in the diff
- [ ] Breaking API changes called out above
- [ ] New deps justified (size, license, maintenance)
