# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an MCP (Model Context Protocol) server for generating UUIDs. The project is in early development stage and uses Python 3.13 with uv as the package manager.

## Development Commands

### Package Management (using uv)
```bash
# Install dependencies
uv pip install -e .

# Add a dependency
uv add <package-name>

# Add dev dependency
uv add --dev <package-name>

# Run the main script
uv run python main.py

# Activate virtual environment
source .venv/bin/activate  # On Unix/macOS
```

## Code Architecture

### Current Structure
- `main.py` - Entry point (currently a placeholder)
- `pyproject.toml` - Project configuration
- No MCP server implementation yet
- No UUID generation logic implemented

### Required Implementation
1. **MCP Server Setup**: Need to add MCP SDK dependencies and implement server handlers
2. **UUID Generation**: Implement UUID v4 generation using Python's `uuid` module
3. **Protocol Handlers**: Create handlers for MCP requests/responses

### Missing Development Tools
- No test framework configured
- No linting/formatting tools set up
- No CI/CD pipeline

When implementing features, consider adding:
- pytest for testing
- ruff for linting and formatting
- mypy for type checking