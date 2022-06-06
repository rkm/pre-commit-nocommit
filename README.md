# pre-commit-nocommit

pre-commit hook to prevent nocommit comments being committed.

## As a pre-commit hook

See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions

Sample `.pre-commit-config.yaml`:

```yaml
- repo: https://github.com/rkm/pre-commit-nocommit
  rev: "" # autoupdate this
  hooks:
      - id: nocommit
      nocommit
      exclude: |
          (?x)^(
            .pre-commit-config.yaml
          )
```
