# [`ontrack-cli-workflow-build`](action.yml)

Links the current workflow to an existing build in Yontrack.

It uses the commit associated with the calling workflow to identify the build.

The Yontrack environment is then setup to point to the build.

Example:

```yaml
steps:
  - uses: nemerosa/ontrack-github-actions-cli-libraryontrack-cli-workflow-build@version
    with:
      project: reporting
```

Following variables are required:

* YONTRACK_URL - URL of the Yontrack instance

Following secrets are required:

* YONTRACK_TOKEN - Token to access the Yontrack instance
* GITHUB_TOKEN - used to download the latest version of the CLI if its `version` is not specified
