# Blocked sources (2026-10-02)

Container egress policy returned 403 on CONNECT for:
www.reddit.com, old.reddit.com, r.jina.ai, www.youtube.com, suggestqueries.google.com,
www.trustpilot.com, mcp.exa.ai, www.bbb.org, www.google.com, html.duckduckgo.com,
www.contractortalk.com, www.quora.com, cli.github.com, www.bing.com,
github.com archive downloads (git clone works).

Fallbacks tested:
- WebFetch old.reddit.com: refused. WebFetch trustpilot.com: EGRESS_BLOCKED.
- TubeAlfred YouTube MCP: insufficient credits (0).
- Chrome browser tools: not available in a cloud session.
