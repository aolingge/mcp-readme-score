<p align="center">
  <img src="assets/readme-banner.svg" alt="MCP README Score banner" width="100%">
</p>

<h1 align="center">MCP README Score</h1>

<p align="center">检查 MCP server README 是否写清安装、权限、环境变量、安全边界和示例。</p>

<p align="center"><a href="README.md">English</a> · <a href="#快速开始">快速开始</a> · <a href="#检查项">检查项</a></p>

<p align="center">
  <img alt="Node.js" src="https://img.shields.io/badge/node-%3E%3D18-6366F1">
  <img alt="dependencies" src="https://img.shields.io/badge/dependencies-0-111827">
  <img alt="license" src="https://img.shields.io/badge/license-MIT-2563EB">
</p>

<p align="center">
  <img src="assets/cli-preview.svg" alt="MCP README Score CLI preview" width="88%">
</p>

## 为什么做这个

AI Agent 工具链正在快速增长，但很多仓库缺少能直接放进 CI 或本地预检的小工具。这个项目保持零依赖、命令短、输出清楚，适合被收藏、fork、二次改造。

## 快速开始

```bash
npx github:aolingge/mcp-readme-score --path README.md
```

Generate Markdown:

```bash
npx github:aolingge/mcp-readme-score --path README.md --markdown > report.md
```

Use a score gate:

```bash
npx github:aolingge/mcp-readme-score --path README.md --min-score 80
```

## 检查项

| Check | What it looks for |
| --- | --- |
| install | Shows install instructions. |
| configuration | Shows client configuration. |
| permissions | Explains permissions. |
| security | Mentions security boundary. |

## Output

```text
MCP README Score score: 100/100
PASS  example-check  Useful signal found
FAIL  missing-check  Add the missing guidance
```

## 参与贡献

Good first PRs: add checks, add fixtures, improve docs, or add GitHub Actions examples.

## License

MIT


## Quality Gate

Use this project as a repeatable gate before an AI agent marks work as done:

- [Quality gate guide](docs/quality-gates.md)
- [Copy-ready GitHub Actions example](examples/github-action.yml)

