# RenderCV

RenderCV is a Python-based CV and résumé engine that transforms YAML input into professional PDF, PNG, Markdown, and HTML documents using Jinja2 templates and Typst.

## Architecture & Codebase Guide

For a comprehensive architecture breakdown, flow diagrams, and module explanations, see:
- [Architecture & Flow Guide](docs/developer_guide/architecture.md)

## Project Structure

```
├── src/
│   └── rendercv/
│       ├── cli/         # CLI commands (render, new, create-theme)
│       ├── schema/      # YAML validation & Pydantic models
│       └── renderer/    # Typst / Markdown / HTML templating & compilers
├── docs/
│   └── developer_guide/
│       └── architecture.md
├── pyproject.toml
└── uv.lock
```

## Quick Start

```bash
# Install dependencies with uv
uv sync

# Render a CV
uv run rendercv render CV.yaml
```
