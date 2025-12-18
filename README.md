ontrack-github-actions-cli-library
==================================

Library of actions for Yontrack CLI in GitHub.

# Usage

For any given action you want to use in your workflow:

```yaml
uses: nemerosa/ontrack-github-actions-cli-library/the-action@version
with:
  some-input: 'hello'
```

For the list of available actions, see [below](#actions). The list of versions is available in the [tags](tags) of the repository.

# Actions

## Setup

* [`ontrack-cli-workflow-build`](ontrack-cli-workflow-build/README.md) - linking a workflow to an existing build in Yontrack

