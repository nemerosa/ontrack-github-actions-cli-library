# [`ontrack-cli-workflow-build`](action.yml)

Links the current workflow to an existing build in Yontrack.

It uses the commit associated with the calling workflow to identify the build.

The Yontrack environment is then setup to point to the build and
the [Yontrack CLI](https://github.com/nemerosa/ontrack-cli) is correctly setup & configured.

Example:

```yaml
steps:
  - uses: nemerosa/ontrack-github-actions-cli-library/ontrack-cli-workflow-build@version
    with:
      project: reporting
      yontrack-url: ${{ vars.YONTRACK_URL }}
      yontrack-token: ${{ secrets.YONTRACK_TOKEN }}
      github-token: ${{ secrets.GITHUB_TOKEN }}
```
