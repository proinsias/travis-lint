# travis-lint

Lint `.travis.yml` files.

[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
[![GitHub Actions](https://github.com/proinsias/travis-lint/workflows/Actions/badge.svg)](https://github.com/proinsias/travis-lint/actions/workflows/actions.yml)

Supports being used as a [pre-commit.com](https://pre-commit.com) hook.
Add this to your `.pre-commit-config.yaml`:

```yaml
-   repo: https://github.com/proinsias/travis-lint/
    rev: v1.0.0  # Use the ref you want to point at
    hooks:
      - id: travis-lint
```

This is taken from travis-ci/travis.rb#307 which has been left to languish on the vine by the `travis.rb` maintainers.
