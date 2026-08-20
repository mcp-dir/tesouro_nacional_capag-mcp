# Instalação rápida

Tesouro Nacional: Capacidade de Pagamento (CAPAG) é um servidor MCP remoto hospedado em `https://api.mcp.ai/p_tesouro_nacional_capag`. Você não baixa nem roda nada localmente — só aponta seu cliente pra essa URL.

A auth acontece em runtime: clientes com **OAuth 2.1** (Claude Desktop, Cursor, VS Code recentes) abrem o browser na 1ª chamada (magic-link). Clientes sem OAuth recebem a tool `authenticate` — abra `https://app.mcp.ai/agent-auth`, faça login, copie o JWT e cole no chat.

---

## Claude (Web e Desktop)

[➕ Abrir no Claude e conectar](https://claude.ai/new?modal=add-custom-connector#settings/customize-connectors)

Manual: [claude.ai/customize/connectors](https://claude.ai/customize/connectors?surface=cowork) → **+** → **Adicionar conector personalizado** → `Tesouro Nacional: Capacidade de Pagamento (CAPAG)` / `https://api.mcp.ai/p_tesouro_nacional_capag`.

Config file (legado): `~/Library/Application Support/Claude/claude_desktop_config.json` (macOS) ou `%APPDATA%\Claude\claude_desktop_config.json` (Windows):

```json
{ "mcpServers": { "tesouro_nacional_capag": { "type": "http", "url": "https://api.mcp.ai/p_tesouro_nacional_capag" } } }
```

## Cursor

[➕ Instalar no Cursor](cursor://anysphere.cursor-deeplink/mcp/install?name=tesouro_nacional_capag&config=eyJ1cmwiOiJodHRwczovL2FwaS5tY3AuYWkvcF90ZXNvdXJvX25hY2lvbmFsX2NhcGFnIn0=)

`.cursor/mcp.json`:
```json
{ "mcpServers": { "tesouro_nacional_capag": { "url": "https://api.mcp.ai/p_tesouro_nacional_capag" } } }
```

## VS Code (Copilot Chat)

[➕ Instalar no VS Code](vscode:mcp/install?name=tesouro_nacional_capag&config=%7B%22type%22%3A%22http%22%2C%22url%22%3A%22https%3A%2F%2Fapi.mcp.ai%2Fp_tesouro_nacional_capag%22%7D)

`.vscode/mcp.json`:
```json
{ "servers": { "tesouro_nacional_capag": { "type": "http", "url": "https://api.mcp.ai/p_tesouro_nacional_capag" } } }
```

## Outros clientes MCP

Qualquer cliente com **MCP over HTTP**. URL fixa:

```
https://api.mcp.ai/p_tesouro_nacional_capag
```

Dúvidas? [tesouro_nacional_capag@mcp.ai](mailto:tesouro_nacional_capag@mcp.ai)
