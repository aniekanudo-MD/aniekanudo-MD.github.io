---
title: "Langgraph Agent Mcp"
repo: "aniekanudo-MD/langgraph-agent-mcp"
category: "AI & Agents"
description: "This repo implements agentic ai with langgraph and MCP module for Google Analytics 4"
excerpt: "An intelligent AI agent built with LangGraph and Model Context Protocol (MCP) that connects to Google Analytics 4 (GA4) to retrieve, analyze, and summarize website performance data. The agent provides business intelligence insights through conversational queries and can be integrated with Claude..."
thumbnail: "/default-thumbnail.svg"
githubUrl: "https://github.com/aniekanudo-MD/langgraph-agent-mcp"
stars: 0
language: "Python"
featured: true
priority: 3
tags: []
techStack:
  - "Python"
  - "LangGraph"
  - "MCP"
  - "Gemini"
  - "OpenAI"
  - "Google Analytics 4 API"
status: "Complete"
liveDemo: ""
features:
  - "**GA4 Report Retrieval**: Fetch standard reports with custom metrics, dimensions, and timeframes"
  - "**Real-Time Analytics**: Access live GA4 data for immediate insights"
  - "**Comparative Analysis**: Compare metrics across two time periods with detailed reports"
  - "**Ranked Reports**: Retrieve and rank data based on specified metrics"
  - "**Account Management**: List all GA4 properties and accounts accessible to the user"
  - "**Multi-Model Support**: Compatible with both Gemini and OpenAI models"
  - "**MCP Integration**: Works as an MCP server with Claude Desktop, MCP Inspector, or standalone client"
---

# Langgraph Agent Mcp

# LangGraph Agent for Google Analytics 4
**Category:** AI & Agents  
**Tech Stack:** Python, LangGraph, MCP, Gemini, OpenAI, Google Analytics 4 API  
**Status:** Complete  
**Thumbnail:** assets/thumbnail.png
## Overview
An intelligent AI agent built with LangGraph and Model Context Protocol (MCP) that connects to Google Analytics 4 (GA4) to retrieve, analyze, and summarize website performance data. The agent provides business intelligence insights through conversational queries and can be integrated with Claude Desktop, MCP Inspector, or run standalone.
## Features
- **GA4 Report Retrieval**: Fetch standard reports with custom metrics, dimensions, and timeframes
- **Real-Time Analytics**: Access live GA4 data for immediate insights
- **Comparative Analysis**: Compare metrics across two time periods with detailed reports
- **Ranked Reports**: Retrieve and rank data based on specified metrics
- **Account Management**: List all GA4 properties and accounts accessible to the user
- **Multi-Model Support**: Compatible with both Gemini and OpenAI models
- **MCP Integration**: Works as an MCP server with Claude Desktop, MCP Inspector, or standalone client
## Tools
| Tool | Description |
|------|-------------|
| `get_report` | Retrieve GA4 report with metrics, dimensions, and timeframe |
| `get_realtime_report` | Access real-time GA4 analytics data |
| `compare_report_metrics` | Compare metrics across two periods |
| `get_report_with_order` | Retrieve ranked reports based on specified metrics |
| `list_all_properties` | List all GA4 properties for the current user |
| `list_all_accounts` | Retrieve GA4 account information |
## Architecture
```
langgraph-agent-mcp/
├── src/
│   ├── gemini_client.py          # Gemini model client
│   ├── openai_client.py          # OpenAI model client
│   ├── gemini_server_sample.py   # MCP server implementation (sample)
│   ├── gemini_utilities/
│   │   ├── gem_server_connect.py # Server connection handler
│   │   ├── response_encoder.py   # Response formatting
│   │   ├── server_connect.py     # Connection management
│   │   └── system_input.py       # System prompts and inputs
│   ├── openai_utilities/
│   │   ├── open_server_connect.py
│   │   └── system_input.py
│   ├── logfolder/                # Structured logging
│   └── tool_sample/
│       ├── run_realtime_report.py
│       └── tabulated.py          # Data table formatting
├── main.py                       # Entry point
├── pyproject.toml                # Dependencies
└── .python-version               # Python version spec
```
## Getting Started
### Prerequisites
- Python 3.10+
- [uv](https://docs.astral.sh/uv/) for dependency management
- Google Cloud account with GA4 access
- OpenAI API key or Google Gemini API key
### Installation
```bash
# Clone the repository
git clone https://github.com/aniekanudo-MD/langgraph-agent-mcp.git
cd langgraph-agent-mcp
# Create virtual environment
uv venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
# Install dependencies
uv sync
```

Configuration
```
1. 
Set up Google credentials:
- 
Configure your Google account for GA4 API access
- 
Download the JSON credentials file
- 
Rename it to credentials.json
2. 
Create environment file:
# Create .env in the src/ folder
touch src/.env
Add to src/.env:
GOOGLE_APPLICATION_CREDENTIALS="C:\\Users\\path\\to\\credentials.json"
GEMINI_API_KEY="your-gemini-api-key"
# OR for OpenAI:
OPENAI_API_KEY="your-openai-api-key"
Running the Agent
Option 1: MCP Inspector (Development)
uv run mcp dev src/gemini_server_sample.py
Option 2: Standalone Client
# Run with Gemini
uv run mcp src/gemini_client.py
# Run with OpenAI
uv run mcp src/openai_client.py
Option 3: Claude Desktop Integration
# Install the MCP server
uv run mcp install src/gemini_server_sample.py
```
Then configure Claude Desktop:
```
1. 
Open Claude Desktop → Settings → Developer → Edit Config
2. 
Add the server configuration:
{
  "mcpServers": {
    "Google Analytics 4": {
      "command": "uv",
      "args": [
        "run", "--with", "mcp[cli]", "mcp", "run",
        "C:\\Users\\path\\to\\langgraph-agent-mcp\\src\\gemini_server_sample.py"
      ],
      "env": {
        "VIRTUAL_ENV": "C:\\Users\\path\\to\\langgraph-agent-mcp\\.venv",
        "PATH": "C:\\Users\\path\\to\\langgraph-agent-mcp\\.venv\\Scripts;${PATH}",
        "GOOGLE_APPLICATION_CREDENTIALS": "C:\\Users\\path\\to\\credentials.json"
      }
    }
  }
}
3. 
Restart Claude Desktop
4. 
Ask Claude: "Get my GA4 traffic report for last week"
```
Sample Queries
```
- 
"Show me pageviews and sessions for the last 30 days"
- 
"Compare this month's traffic to last month"
- 
"What are my top performing pages?"
- 
"List all my GA4 properties"
- 
"Get real-time active users right now"
```
## Tech Stack
```
Component	Technology
Agent Framework	LangGraph
Protocol	Model Context Protocol (MCP)
LLM Providers	Google Gemini, OpenAI
Data Source	Google Analytics 4 API
Language	Python 3.10+
Package Manager	uv
```
Limitations
-
```
This repository contains a sample server implementation
- 
The full production server with all features is available on request
- 
Contact for access to the complete implementation
```
Contact
- 
Email: [Aniekan Udo @gmail.com](mailto:aniekanetimudo+reachout@gmail.com)
 
LinkedIn: [Aniekan Udo @LinkedIn](https://www.linkedin.com/in/aniekan-etim-udo)

License
-
MIT
