<!----- BEGIN GHOST DOCS HEADER ----->

# .github

[![coverage.yml](https://github.com/jill64/.github/actions/workflows/coverage.yml/badge.svg)](https://github.com/jill64/.github/actions/workflows/coverage.yml) [![publish-pages.yml](https://github.com/jill64/.github/actions/workflows/publish-pages.yml/badge.svg)](https://github.com/jill64/.github/actions/workflows/publish-pages.yml) [![run-playwright.yml](https://github.com/jill64/.github/actions/workflows/run-playwright.yml/badge.svg)](https://github.com/jill64/.github/actions/workflows/run-playwright.yml)

Common account settings

<!----- END GHOST DOCS HEADER ----->

## Reusable Workflows

```yml
name: Test

on: push

jobs:
  test:
    uses: jill64/.github/.github/workflows/coverage.yml@main
```
