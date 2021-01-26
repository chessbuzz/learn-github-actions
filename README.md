# learn-github-actions
learn-github-actions

## Workflows

* Live in .github/workflows
* are written in YAML
```YAML
name: learn-github-actions
on: [push]
jobs:
  check-bats-version:
    steps:
      -uses: actions/checkout@v2
      -uses: actions/setup-node@v1
      -run: npm install -g bats
      -run: bats -v
 ```
