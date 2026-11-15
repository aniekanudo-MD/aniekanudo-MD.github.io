---
title: "Notetaker Mcp Server"
repo: "aniekanudo-MD/Notetaker-MCP-Server"
category: "MLOps & Tools"
description: "An MCP (Model Context Protocol) server that turns Claude Desktop into your personal note-taking assistant. Add notes, read them back, search through them, and get AI-generated summaries — all through natural conversation. A `notebook.txt` is automatically created when you first run the project."
excerpt: "An MCP (Model Context Protocol) server that turns Claude Desktop into your personal note-taking assistant. Add notes, read them back, search through them, and get AI-generated summaries — all through natural conversation. A `notebook.txt` is automatically created when you first run the project."
thumbnail: "/default-thumbnail.svg"
githubUrl: "https://github.com/aniekanudo-MD/Notetaker-MCP-Server"
stars: 0
language: ""
featured: false
priority: 7
tags: []
techStack:
  - "Python"
  - "MCP"
  - "Claude Desktop"
status: "Complete"
liveDemo: ""
features:
  - "**Add Notes**: Save notes directly from Claude's responses"
  - "**Read All Notes**: View your entire notebook"
  - "**Read Latest**: Quickly access your most recent note"
  - "**Read by Index**: Jump to any specific note"
  - "**AI Summary**: Ask Claude to summarize your notes"
  - "**Search Notes**: Find information across all notes with AI-powered search"
---

# Notetaker Mcp Server

# Notetaker MCP Server
**Category:** MLOps & Tools  
**Tech Stack:** Python, MCP, Claude Desktop  
**Status:** Complete  
**Thumbnail:** assets/thumbnail.png
## Overview
An MCP (Model Context Protocol) server that turns Claude Desktop into your personal note-taking assistant. Add notes, read them back, search through them, and get AI-generated summaries — all through natural conversation. A `notebook.txt` is automatically created when you first run the project.
## Features
- **Add Notes**: Save notes directly from Claude's responses
- **Read All Notes**: View your entire notebook
- **Read Latest**: Quickly access your most recent note
- **Read by Index**: Jump to any specific note
- **AI Summary**: Ask Claude to summarize your notes
- **Search Notes**: Find information across all notes with AI-powered search
## Project Structure
```
Notetaker-MCP-Server/
├── main.py                       # MCP server entry point
├── pyproject.toml                # Python dependencies
├── uv.lock                       # Dependency lock file
├── .python-version               # Python version spec
├── LICENSE                       # MIT License
└── README.md
```
## Quick Start
### Prerequisites
- Python 3.10+
- [uv](https://docs.astral.sh/uv/)
- [Claude Desktop](https://claude.ai/download)
### Setup
```bash
git clone https://github.com/aniekanudo-MD/Notetaker-MCP-Server.git
cd Notetaker-MCP-Server
uv sync
uv run mcp install main.py
```
### Configure Claude Desktop
1. Open Claude Desktop → Settings → Developer → Edit Config
2. Ensure the config matches:
```json
{
  "mcpServers": {
    "Demo": {
      "command": "uv",
      "args": [
        "run",
        "--with",
        "mcp[cli]",
        "mcp",
        "run",
        "C:\\Users\\username\\path\\to\\Notetaker-MCP-Server\\main.py"
      ]
    }
  }
}
```
3. Restart Claude Desktop
### Try It
```
"Write a three line poem on Agriculture and add it to my note"
```
## Available Tools
| Tool | Type | Description |
|------|------|-------------|
| `add_note` | Tool | Add content to your notebook |
| `read_all_notes` | Tool | Read all notes |
| `read_latest_notes` | Tool | Read the most recent note |
| `read_indexed_notes` | Tool | Read note at a specific index |
| `note_summary_prompt` | Prompt | Get AI summary of your notes |
| `search_note_prompt` | Prompt | Search notes for specific info |
## Tech Stack
- **Protocol**: Model Context Protocol (MCP)
- **Client**: Claude Desktop
- **Language**: Python 3.10+
- **Package Manager**: uv
## Contact
- **Email**: [Aniekan Udo @Gmail](mailto:aniekanetimudo+reachout@gmail.com)
- **LinkedIn**: [Aniekan Udo @Linkedin](https://www.linkedin.com/in/aniekan-etim-udo)
## License
MIT
