# Tooling (Phase 0)

Environment: Claude Code cloud container (Linux, no desktop, no Chrome session).

## Agent-Reach install
- `pip install` of the GitHub archive zip: 403 (egress policy).
- Installed from `git clone https://github.com/Panniantong/agent-reach` into `~/.agent-reach-venv` (GitHub source, not PyPI). Version: v1.5.0.

## Dry run (`agent-reach install --env=auto --dry-run`)
```
Environment: Server/VPS (auto-detected)
[dry-run] System dependency check:
  gh CLI: would install via: apt-get install gh / brew install gh
  ✅ Node.js: already installed, skip
[dry-run] Would install mcporter and configure Exa search
Tip: Reddit requires a logged-in session (rdt-cli + cookie).
```
`--system` NOT run (awaiting approval; pointless until network is opened).

## Channel status
| Channel | Backend | Status |
|---|---|---|
| Reddit | OpenCLI impossible here (no Chrome). rdt-cli + cookie possible | Blocked: www.reddit.com, old.reddit.com denied by egress |
| YouTube | yt-dlp | Blocked: www.youtube.com denied. TubeAlfred MCP: 0 credits |
| Web reader | Jina Reader | Blocked: r.jina.ai denied |
| Exa | mcporter | Blocked: mcp.exa.ai denied |
| Built-in WebSearch | Claude server side | Works (titles, URLs, summaries only; not verbatim) |
| Built-in WebFetch | Claude server side | reddit.com and trustpilot.com refused |
