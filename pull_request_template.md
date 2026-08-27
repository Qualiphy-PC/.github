## What

<!-- pr:what -->
<!-- One or two sentences. -->

## Ticket

<!-- pr:ticket -->

## Sensitive scope

<!-- pr:scope -->
<!-- DELETE THIS SECTION if none apply. If any apply, the PR TITLE must say so
     too — a title that under-reports scope is grounds to request changes. -->

- [ ] Changes **authorization** (who can see or do what)
- [ ] Changes a **money path** (charges, refunds, prices, COGS, payouts)
- [ ] Changes **endpoint semantics** or a response shape others consume
- [ ] Changes **schema** (fill in the Database section below)

## Why

<!-- pr:why -->

## How

<!-- pr:how -->

## Testing

<!-- pr:testing -->
<!-- The question a reviewer asks: WHICH TEST FAILS if this PR's new behavior
     regresses? "The old suite still passes" is not an answer. -->

- [ ] `npm run lint` passes
- [ ] `npm test` passes
- [ ] Ran locally and exercised the change
- [ ] **New behavior has new tests** — happy path AND failure cases (name them above)
- [ ] **Bug fix?** The regression test fails on the code before this PR and passes
      after — run it at the merge base and at the head, note both results above

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

## Touch points

<!-- pr:touch_points -->
<!-- DELETE THIS SECTION if the PR changes no contract surface: endpoints,
     shared tables, response keys, events/webhooks, shared packages. -->

**What surface changes:** <!-- endpoint / table+column / response key / event -->

**Who consumes it:** <!-- callers across the estate — grep the sibling repos and
     check qualiphy-platform/docs/service-dependencies.md — plus external API
     clients where relevant. Say what you checked, not just what you believe. -->

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
