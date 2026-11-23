# gb-testfixture

A long-lived test source for git-backup. Commits made here are test data for a
long-lived backup: take a backup, push a commit, take another backup, check the
new one downloads and restores.

## Forks

A test cycle may have **one** private fork of this repository.

- The fork carries the release under test in its name, so the fork says which
  wave it belongs to.
- Before anything is forked, every old private fork of this repository is
  deleted. No fork outlives the release it was made for.
- When a new release needs a new fork, any fork for an obsolete release is
  deleted in the same act.
- Supersession runs per kind: an official release supersedes official releases,
  and a speculative release supersedes speculative releases. A speculative build
  never supersedes an official release, and an official release is never treated
  as superseded by a speculative build.

## What it is not

It is not product code, and nothing here ships. Real work lives in
gitbackup-cloud/gitbackup.cloud.
