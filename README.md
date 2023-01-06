# semantic-release for your GitHub Action

**semantic-release-for-your-github-action** is a GitHub Action that releases your GitHub Action with [semantic-release].

[semantic-release]: https://github.com/semantic-release/semantic-release

## What's in it for me?

This action encapsulates a semantic-release installation and configuration, so your repository only has to focus on the business-logic of your GitHub Action.

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

# Only allow one release workflow to execute at a time, since each release
# workflow uses shared resources (git tags)
concurrency:
  group: ${{ github.workflow }}

jobs:
  release:
    name: Release
    runs-on: ubuntu-latest

    steps:
      - uses: EricCrosson/semantic-release-your-github-action@v2
```

If your repository does not specify a semantic-release configuration, this action will provide its own.
If your repository does specify a semantic-release configuration, that configuration will be used.

## Inputs

There are no inputs to this action.
