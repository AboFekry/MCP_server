# MCP Server Demo

A small Python project that demonstrates a Model Context Protocol (MCP) server using `FastMCP`.

## What this project does

This server exposes two simple tools for clients to call:

- `sum_two_numbers_tool` — adds two integers
- `subtract_two_numbers_tool` — subtracts two integers

It is a minimal example for learning how MCP servers are created and tested.

## Project files

- `mcp_server.py` — MCP server implementation
- `requirements.txt` — Python dependencies
- `MCP_explanation.md` — explanation and notes about MCP concepts

## Requirements

- Python 3.10+
- pip

## Setup

```powershell
cd "D:\MY __ career\mcp_server"
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

## Run the server

```powershell
python .\mcp_server.py
```

## Run with MCP Inspector

```powershell
npx @modelcontextprotocol/inspector python .\mcp_server.py
```

This is useful for testing the exposed MCP tools from a browser-based inspector.

## Example tool behavior

- `sum_two_numbers_tool(4, 6)` → returns: `The sum of 4 and 6 is 10 (Calculated by MCP server).`
- `subtract_two_numbers_tool(10, 3)` → returns a demo subtraction result from the current implementation.

## Notes

This is a beginner-friendly sample project meant to show the basics of building an MCP tool server. It can be extended with more useful tools, validation, or real business logic.
