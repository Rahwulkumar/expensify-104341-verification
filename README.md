# Expensify #104341 verification

This package verifies a local three-file change against Expensify/App commit `f24918318d03b8f83ccb88ce41de278070e70775`. It is preparation for a contribution, with no claimed assignment, proposal acceptance or bounty entitlement. Existing proposals describe overlapping approaches.

The manually triggered workflow checks the exact file hashes, installs the pinned dependencies with the normal patches, and runs full TypeScript checking, the project's lint pipeline on all changed files, formatting, spelling, three regression suites and the staging web build. Checks run sequentially on a standard Ubuntu runner. Individual failures remain visible and fail the final job; continuing after a failed step only collects the remaining results.

The browser artifact supports subsequent testing of the real split/hold/partial-approval flow. A successful build does not establish that the UI flow passes. No account information, browser storage or credentials belong in this repository or its artifacts. The workflow has read-only repository permissions and does not deploy or publish a PR. Artifacts expire after one day.

Upstream source is checked out directly from [Expensify/App](https://github.com/Expensify/App); its [MIT license](LICENSE.md) applies to the patch. This package contains no copied dependency tree or private investigation records.
