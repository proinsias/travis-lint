# travis-lint

Lint `.travis.yml` files.

[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
[![Cron Jobs](https://github.com/proinsias/travis-lint/workflows/Cron%20Jobs/badge.svg)](https://github.com/proinsias/travis-lint/actions/workflows/cronjobs.yml)
[![Pull Requests & Pushes](https://github.com/proinsias/travis-lint/workflows/Pull%20Requests%20%26%20Pushes/badge.svg)](https://github.com/proinsias/travis-lint/actions/workflows/pull-requests-and-pushes.yml)
[![ShiftLeft Scan](https://github.com/proinsias/travis-lint/workflows/ShiftLeft%20Scan/badge.svg)](https://github.com/proinsias/travis-lint/actions/workflows/shiftleft-analysis.yml)
[![Mergify Status][mergify-status]][mergify]

Supports being used as a [pre-commit.com](https://pre-commit.com) hook.
Add this to your `.pre-commit-config.yaml`:

```yaml
-   repo: https://github.com/proinsias/travis-lint/
    rev: v1.0.0  # Use the ref you want to point at
    hooks:
      - id: travis-lint
```

This is taken from
[travis-ci/travis.rb#307](https://github.com/travis-ci/travis.rb/pull/307)
which has been left to languish on the vine by the `travis.rb` maintainers.

[mergify]: https://mergify.io
[mergify-status]: https://img.shields.io/endpoint.svg?url=https://gh.mergify.io/badges/proinsias/travis-lint&style=flat
