# Soc Ops - Copilot Workspace Instructions

**Soc Ops** is a Social Bingo game built with **FastAPI + Jinja2 + HTMX**. Players find people matching questions to mark 5-in-a-row bingo on a grid.

## ✅ Mandatory Development Checklist

**Before committing, run:**
```bash
uv run ruff check .          # Lint (snake_case, no unused imports)
uv run pytest                # Test (25 tests expected)
uv run uvicorn app.main:app --reload  # Verify dev server starts
```

## Quick Reference

| Command | Purpose |
|---------|---------|
| `uv sync` | Install dependencies (Python 3.13+ via uv) |
| `uv run pytest -v` | Run all tests |
| `uv run ruff check .` | Lint & check code style |
| `uv run uvicorn app.main:app --reload` | Dev server at http://localhost:8000 |

## Architecture

- `main.py` — FastAPI routes & HTMX endpoints
- `game_logic.py` — Board generation & bingo detection
- `game_service.py` — GameSession (signed cookies via itsdangerous)
- `models.py` — Pydantic models (GameState, BingoSquare)
- `templates/` — Jinja2 base, screens, & components
- `static/css/app.css` — Custom utility classes (`.flex`, `.grid`, `.bg-accent`, etc.)

## Key Patterns

**Game Logic**: 5×5 grid, shuffled questions, center is free space, check rows/cols/diagonals  
**State**: Stored server-side in signed cookies, persisted on every change  
**HTMX**: Routes return HTML fragments; buttons use `hx-post`/`hx-get` with `hx-target`  
**Templates**: `base.html` (session mgmt), `start_screen.html`, `game_screen.html`, components  
**Styling**: Custom CSS utilities; avoid generic AI aesthetics (see frontend-design.instructions.md)

## Design Guide

**Theme**: Cinematic theater experience with dramatic lighting, deep reds, and gold accents  
**Typography**: Cinzel (serif) for headings, Orbitron (futuristic) for UI, Source Serif Pro for content  
**Colors**: Theater dark (#0a0a0a), blood red (#8b0000), gold (#fbbf24), cyan (#06b6d4)  
**Effects**: Curtain animations, sweeping spotlights, glow effects, backdrop blur  
**Principles**: Avoid generic AI aesthetics - commit to distinctive, cohesive themes with high-impact animations

## Related Guidance

- [frontend-design.instructions.md](.github/instructions/frontend-design.instructions.md) — Build distinctive UIs, not generic AI
- [css-utilities.instructions.md](.github/instructions/css-utilities.instructions.md) — Available utility classes
- [general.instructions.md](.github/instructions/general.instructions.md) — Use real browser (never Simple Browser)

---

**Last updated**: April 2026

