# gh-deploy

A simple command line utility for creating a GitHub Deployment via the GitHub API.

## Getting Started

Make sure the `GITHUB_OAUTH_TOKEN` environment variable is initialized with a
valid GitHub OAuth token with the `repo_deployment` scope. Run
`gh-deploy --help` for example usage:

```term
$ gh-deploy -h

  gh-deploy [REF] [[FLAGS]]

    Create a GitHub Deployment via the API.

    FLAGS:

      -a,--auto-merge          Auto-merge the default branch into the requested ref if it is behind the default branch
      -c,--required-contexts   A comma seperated list of status contexts verified against commit status checks
      -d,--description         Short description
      -e,--environment         Name for the target deployment environment
      -o,--owner               Owner name
      -p,--payload             JSON payload with extra information about the deployment
      -r,--repo                Repo name
      -t,--task                The named task to execute
      -v,--verbose             Verbose output
      -h,--help                Show this usage
```
