# Reusable Workflows

汎用的なGitHub Actionsワークフローを再利用可能なワークフローとして保管するリポジトリです。

## 使用方法

```yaml
name: My Workflow
on:
  pull_request:
    branches: [main]

jobs:
  use-reusable-workflow:
    uses: ryoooosk/reusable-workflows/.github/workflows/[ワークフロー名].yml@main
    secrets:
      GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```
