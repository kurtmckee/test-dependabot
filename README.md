Demonstrate Dependabot failing to find new versions of
`github.com/wasilibs/go-shellcheck/cmd/shellcheck`.

The issue demonstrated here is that Dependabot always claims that
whatever version is currently listed is the latest version.

For example, if the version in the `.pre-commit-config.yaml` file is `v0.10.0`,
then Dependabot's logs claim that `v0.10.0` is the latest available version.

However, if the version is `v0.11.1`,
then Dependabot's logs claim that `v0.11.1` is the latest available version.

(At the time of writing, `v0.11.1` is the latest version.)
