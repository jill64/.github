<!----- BEGIN GHOST DOCS HEADER ----->

# .github

<!----- BEGIN GHOST DOCS BADGES -----><a href="https://github.com/jill64/.github/actions/workflows/publish-pages.yml"><img src="https://github.com/jill64/.github/actions/workflows/publish-pages.yml/badge.svg" alt="publish-pages.yml" /></a> <a href="https://github.com/jill64/.github/actions/workflows/run-vitest.yml"><img src="https://github.com/jill64/.github/actions/workflows/run-vitest.yml/badge.svg" alt="run-vitest.yml" /></a><!----- END GHOST DOCS BADGES ----->

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
