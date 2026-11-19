# Ponzu for Claude Code and Codex

[Ponzu](https://ponzu.design) keeps canvases in the cloud, each beside a repository. This plugin lets your own agent use them: join a canvas yourself while people comment, or hand it to Ponzu's agent, then build what was settled in your own checkout and link the pull request, so the canvas settles once it merges.

It connects to Ponzu's MCP server at `https://api.ponzu.design/v1/mcp` and adds skills for starting from a brief, exploring variations, bringing a screen in from code, product shots, implementing a canvas and watching comments.

```sh
# Claude Code
claude plugin marketplace add north-brook/ponzu-plugin
claude plugin install ponzu@ponzu
claude mcp login plugin:ponzu:ponzu

# Codex
codex plugin marketplace add north-brook/ponzu-plugin
codex plugin add ponzu@ponzu
codex mcp login ponzu
```

Signing in opens Ponzu, which asks you to allow the agent.

Added the marketplace as `north-brook/ponzu` before? Remove it first (`claude plugin marketplace remove ponzu`, or `codex plugin marketplace remove ponzu`), then add this one.

This repository is published from Ponzu's own with every release; changes made here are overwritten.
