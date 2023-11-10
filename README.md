<!----- BEGIN GHOST DOCS HEADER ----->

# .github

[![curl-test.yml](https://github.com/jill64/.github/actions/workflows/curl-test.yml/badge.svg)](https://github.com/jill64/.github/actions/workflows/curl-test.yml) [![publish-pages.yml](https://github.com/jill64/.github/actions/workflows/publish-pages.yml/badge.svg)](https://github.com/jill64/.github/actions/workflows/publish-pages.yml) [![run-playwright.yml](https://github.com/jill64/.github/actions/workflows/run-playwright.yml/badge.svg)](https://github.com/jill64/.github/actions/workflows/run-playwright.yml) [![run-vitest.yml](https://github.com/jill64/.github/actions/workflows/run-vitest.yml/badge.svg)](https://github.com/jill64/.github/actions/workflows/run-vitest.yml)

🛠️ Common account settings

<!----- END GHOST DOCS HEADER ----->

## Reusable Workflows

```yml
name: CI

on: push

jobs:
  test:
    uses: jill64/.github/.github/workflows/run-vitest.yml@main
  test-e2e:
    uses: jill64/.github/.github/workflows/run-playwright.yml@main
    with:
      pre-test: npm run build
      test-command: npx playwright test
```
