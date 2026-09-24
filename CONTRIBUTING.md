# Contributing to homebrew-tap

The casks in this repository are generated. Each pgEdge CLI release
runs GoReleaser in [pgEdge/pgedge-cli](https://github.com/pgEdge/pgedge-cli),
which writes `Casks/pgedge.rb` and commits it here. A hand edit to a
generated cask is overwritten by the next release, so change the
`homebrew_casks` section of `.goreleaser.yaml` in pgedge-cli instead.

## Pull Request Guidelines

- One logical change per PR
- Follow conventional commit style for your PR title
  (`feat:`, `fix:`, `docs:`, `chore:`, etc.)
- Run `brew style pgedge/tap` and `brew audit --cask --tap pgedge/tap`
  before submitting; CI runs both

## Reporting Issues

- Report a problem with installing or upgrading through Homebrew here,
  using the [bug report template](.github/ISSUE_TEMPLATE/bug_report.md)
- Report a bug in the `pgedge` command itself in
  [pgEdge/pgedge-cli](https://github.com/pgEdge/pgedge-cli/issues)
