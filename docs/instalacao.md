# Instalação detalhada

Tesouro Nacional: Capacidade de Pagamento (CAPAG) é um servidor MCP remoto. Aponte seu cliente pra `https://api.mcp.ai/p_tesouro_nacional_capag`. Snippets rápidos: [INSTALL.md](../INSTALL.md).

| Cliente | URL | Auth |
|---|---|---|
| Claude Desktop | `https://api.mcp.ai/p_tesouro_nacional_capag` | OAuth 2.1 ou agent-auth |
| Cursor | `https://api.mcp.ai/p_tesouro_nacional_capag` | OAuth 2.1 ou agent-auth |
| VS Code (Copilot) | `https://api.mcp.ai/p_tesouro_nacional_capag` | OAuth 2.1 ou agent-auth |

A config JSON é a mesma em todos: só a URL, sem headers.

## Desinstalar

Remova o bloco `mcpServers.tesouro_nacional_capag` (ou `servers.tesouro_nacional_capag` no VS Code) do config do cliente e reinicie.
