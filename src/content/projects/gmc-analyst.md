---
title: "Gmc Analyst"
repo: "aniekanudo-MD/gmc-analyst"
category: "Fullstack"
description: "A fullstack web application for analyzing Global Management Challenge (GMC) competition data. Parse Excel reports, visualize financial and operational metrics, and simulate decision outcomes"
excerpt: "A fullstack web application for analyzing Global Management Challenge (GMC) competition data. Upload Excel reports, visualize financial and operational metrics across quarters, and simulate decision outcomes to optimize business strategy."
thumbnail: "/default-thumbnail.svg"
githubUrl: "https://github.com/aniekanudo-MD/gmc-analyst"
stars: 0
language: "TypeScript"
featured: true
priority: 1
tags: []
techStack:
  - "Go"
  - "React"
  - "TypeScript"
  - "PostgreSQL"
  - "Gin"
  - "Vite"
  - "Zustand"
status: "Complete"
liveDemo: ""
features:
  - "**Excel Report Parsing**: Upload and parse GMC competition Excel files"
  - "**Financial Dashboards**: Income statement, balance sheet, cash flow analysis"
  - "**Operational Metrics**: Track production, inventory, sales, and market share"
  - "**Competitor Analysis**: Compare performance against rival teams"
  - "**Decision Simulation**: Model impact of strategic choices"
  - "**Quarter Navigation**: Browse historical data across multiple quarters"
---

# Gmc Analyst

# GMC Analyst
**Category:** Fullstack  
**Tech Stack:** Go, React, TypeScript, PostgreSQL, Gin, Vite, Zustand  
**Status:** Complete  
**Thumbnail:** assets/thumbnail.png
## Overview
A fullstack web application for analyzing Global Management Challenge (GMC) competition data. Upload Excel reports, visualize financial and operational metrics across quarters, and simulate decision outcomes to optimize business strategy.
## Features
- **Excel Report Parsing**: Upload and parse GMC competition Excel files
- **Financial Dashboards**: Income statement, balance sheet, cash flow analysis
- **Operational Metrics**: Track production, inventory, sales, and market share
- **Competitor Analysis**: Compare performance against rival teams
- **Decision Simulation**: Model impact of strategic choices
- **Quarter Navigation**: Browse historical data across multiple quarters
## Project Structure
```
gmc-analyst/
├── cmd/api/                      # Go API entry point
├── internal/
│   ├── adapter/
│   │   ├── db/                   # PostgreSQL repositories
│   │   ├── excel/                # Excel parser and extractor
│   │   └── http/                 # HTTP handlers and DTOs
│   ├── config/                   # App configuration
│   ├── domain/                   # Business logic and entities
│   └── simulation/               # Decision simulator
├── web/                          # React frontend (Vite)
│   ├── src/
│   │   ├── api/                  # API client
│   │   ├── components/           # UI components
│   │   ├── pages/                # Dashboard pages
│   │   └── store/                # Zustand state management
│   └── tests/e2e/                # Playwright tests
├── migrations/                   # Database migrations
├── config/                       # Excel cell mappings
└── docs/                         # Architecture docs
```
## Getting Started
### Prerequisites
- Go 1.22+
- Node.js 18+
- PostgreSQL 16+
### Backend Setup
```bash
# Install dependencies
go mod download
# Set environment variables
cp .env.example .env
# Run the backend server (port 3030)
go run ./cmd/api
```
### Frontend Setup
```bash
cd web
npm install
npm run dev  # runs on port 5173
```
### Environment Variables
| Variable | Default | Description |
|----------|---------|-------------|
| `PORT` | `3030` | Backend API port |
| `DATABASE_URL` | - | PostgreSQL connection string |
| `LOG_LEVEL` | `debug` | Logging level |
| `CORS_ORIGIN` | `http://localhost:5173` | Allowed CORS origin |
## Tech Stack
| Layer | Technology |
|-------|-----------|
| **Backend** | Go 1.22+ with Gin framework |
| **Frontend** | React + TypeScript with Vite |
| **Database** | PostgreSQL 16+ |
| **State Management** | Zustand v5.0+ |
| **Testing** | Playwright (E2E), Go tests |
## Contact
- **Email**: [Aniekan Udo @Gmail](mailto:aniekanetimudo+reachout@gmail.com)
- **LinkedIn**: [Aniekan Udo @Linkedin](https://www.linkedin.com/in/aniekan-etim-udo)
## License
MIT
