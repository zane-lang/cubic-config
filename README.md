# cubic-config

This repository holds the organization-wide configuration for the
[cubic](https://cubic.dev) AI code reviewer. cubic applies `cubic.yaml` to
every `zane-lang` repository that has no `cubic.yaml` of its own, and reads
the file from the default branch only.

The settings keep reviews inside the free plan's monthly reviewed-line limit:
cubic reviews each pull request once when it opens, skips drafts, and leaves
tests, fixtures, vendored sources, lockfiles and images out of the review.
See [cubic's configuration reference](https://docs.cubic.dev/configure/cubic-yaml)
for every key.
