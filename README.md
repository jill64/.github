<!----- BEGIN GHOST DOCS HEADER ----->

# .github

[![publish-pages.yml](https://github.com/jill64/.github/actions/workflows/publish-pages.yml/badge.svg)](https://github.com/jill64/.github/actions/workflows/publish-pages.yml) [![run-playwright.yml](https://github.com/jill64/.github/actions/workflows/run-playwright.yml/badge.svg)](https://github.com/jill64/.github/actions/workflows/run-playwright.yml) [![run-vitest.yml](https://github.com/jill64/.github/actions/workflows/run-vitest.yml/badge.svg)](https://github.com/jill64/.github/actions/workflows/run-vitest.yml)

Common account settings

<!----- END GHOST DOCS HEADER ----->

## Reusable Workflows

```yml
name: Test

on: push

jobs:
  test:
    uses: jill64/.github/.github/workflows/run-vitest.yml@main
```
