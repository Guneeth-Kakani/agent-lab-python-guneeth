🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# 🎯 Soc Ops

## Break the Ice, One Bingo at a Time

**Soc Ops** is a fast-paced, interactive bingo game designed to spark conversations at in-person mixers, team retreats, and social events. Players hunt through the crowd to find people matching quirky questions, marking off 5-in-a-row for an instant win!

Perfect for icebreakers, networking events, and team building—bringing people together through fun, collaborative gameplay.

---

## ✨ How It Works

1. **Get a board** with 25 randomized questions
2. **Find people** around you matching each question
3. **Mark your squares** with a tap
4. **Get 5 in a row** (across, down, diagonals) to win! 🎉

The center square is always a **FREE SPACE**—because everyone needs a freebie.

---

## 🛠️ Tech Stack

Built with modern Python web technologies for a seamless experience:

- **[FastAPI](https://fastapi.tiangolo.com/)** — Lightning-fast web framework
- **[HTMX](https://htmx.org/)** — Interactive UX without reloading
- **[Jinja2](https://jinja.palletsprojects.com/)** — Dynamic templates
- **Python 3.13+** — Modern, clean code
- **Signed Sessions** — Secure, stateless player tracking

---

## 🚀 Quick Start

### Prerequisites
- Python 3.13+
- `uv` package manager

### Installation

```bash
# Clone the repository
git clone https://github.com/copilot-dev-days/agent-lab-python
cd agent-lab-python

# Install dependencies
uv sync

# Run the dev server
uv run uvicorn app.main:app --reload
```

Visit **http://localhost:8000** and start playing!

---

## 🧪 Development

```bash
# Run tests
uv run pytest -v

# Lint code (ruff)
uv run ruff check .

# Format code
uv run ruff format .
```

All **25 tests** pass with full coverage of game logic and API endpoints.

---

## 📚 Learning Lab

This project is also a hands-on workshop for AI-assisted development with GitHub Copilot!

| Part | Topic |
|------|-------|
| [**00**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=00-overview) | Overview & Checklist |
| [**01**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=01-setup) | Setup & Context Engineering |
| [**02**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=02-design) | Design-First Frontend |
| [**03**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=03-quiz-master) | Custom Quiz Master |
| [**04**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=04-multi-agent) | Multi-Agent Development |

📝 Full lab guides are available in [`workshop/`](workshop/) for offline reading.

**New to this workshop?** Start with [Part 00: Overview](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=00-overview).

---

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

---

**Questions? Found a bug?** Check out [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to help!
