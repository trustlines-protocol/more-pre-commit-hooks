# Overview

This repository contains some additional
[pre-commit](https://pre-commit.com/) hooks.

## shellcheck

This hook runs the shellcheck program, a linter for shell
scripts. This requires the shellcheck executable to be installed (`apt install
shellcheck`).

## shfmt

This hook runs the shfmt program, an autoformatter for shell scripts. Please
install the shfmt executable from [mvdan/sh](https://github.com/mvdan/sh/releases)

## Usage

To use these hooks, add the following snippet into your
`.pre-commit-config.yaml`:

```yaml
- repo: https://github.com/trustlines-protocol/more-pre-commit-hooks.git
  rev: master
  hooks:
    - id: shfmt
    - id: shellcheck
```
