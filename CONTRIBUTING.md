# Contributing

Use PHP 8.2 or later with mbstring and Composer. Install dependencies with
`composer install`, then run:

```sh
composer qa
```

This runs PHP CS Fixer in dry-run mode, PHPStan, and PHPUnit. Use
`composer cs:fix` to apply formatting. Git provider tests require the `git`
executable. Use temporary fixture directories and repositories for provider
examples and tests; do not expose personal filesystem contents.

For changes to tree operations, test input preservation, path normalization,
metadata, and edge cases such as empty nodes. Update the relevant
[guide](docs/index.md) and changelog for public behavior changes. Keep rendered
tree examples aligned with actual printer output.
