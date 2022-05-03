# Geek.Zone Reusable Workflows
Our home for GitHub Actions [reusable workflows](https://docs.github.com/en/actions/using-workflows/reusing-workflows).
If you find the need to use a workflow in more than one repo, move it here and call it.

## Why?
This helps to keep our codebase dry.

## Workflows
### Tweet
To tweet a message, call the `tweet` workflow.

This should be used whenever an action is taken that was previously manually executed.

```yml
jobs:
  rw-tweet:
    uses: geekzonehq/reusable-workflows/.github/workflows/tweet.yml@main
    with:
      message: "change me!"

```