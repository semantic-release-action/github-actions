# semantic-release-action/github-actions

[![Build Status]](https://github.com/semantic-release-action/github-actions/actions/workflows/host_release.yml)

[build status]: https://github.com/semantic-release-action/github-actions/actions/workflows/host_release.yml/badge.svg?branch=master&event=push

This is a GitHub Action that releases your GitHub Action using [semantic-release].

[semantic-release]: https://github.com/semantic-release/semantic-release

## What's in it for me?

This action encapsulates a semantic-release installation and configuration, so your repository only has to focus on the business logic of your GitHub Action.

The default configuration will:

- maintain and commit a CHANGELOG.md file
- create GitHub releases
- maintain semantic version tags as [GitHub recommends]

[github recommends]: https://docs.github.com/en/actions/creating-actions/releasing-and-maintaining-actions#example-developer-process

This allows users of your action to invoke it with any of:

- `my/foo-bar-deluxe@v1`
- `my/foo-bar-deluxe@v1.2`
- `my/foo-bar-deluxe@v1.2.3`

## Use

To use this repository's default semantic-release configuration, create a workflow like:

```yaml
---
name: Release

on:
  push:
    branches:
      - master
      - next
      - next-major
      - beta
      - alpha
      - "[0-9]+.[0-9]+.x"
      - "[0-9]+.x"

jobs:
  release:
    uses: semantic-release-action/github-actions/.github/workflows/release.yml@v5
```

If your repository does not specify a semantic-release configuration, this action will provide its own.
If your repository does specify a semantic-release configuration, that configuration will be used.

## Inputs

|       Input Parameter        | Default | Description                                                                                    |
| :--------------------------: | :-----: | ---------------------------------------------------------------------------------------------- |
| disable-semantic-release-git | `false` | Disable [@semantic-release/git] in your release flow. [Details](#disable-semantic-release-git) |

[@semantic-release/git]: https://github.com/semantic-release/git

#### disable-semantic-release-git

Runtime option controlling the use of [@semantic-release/git].
Set to `false` to prevent semantic-release from pushing artifacts to your repository.
This may be required with certain repository settings, for example when requiring signed commits.
