# Trading Advisor

A browser-based AI trading advisor dashboard — the "Day Trader's Second Brain." Built as a single-file HTML app with a dark terminal aesthetic, Chart.js visualizations, and a conversational interface grounded in day trading methodology.

Open `trading-agent.html` directly in any browser. No server, no install, no dependencies beyond what loads from CDN.

## Features

- **Conversational advisor interface** — Ask questions about setups, risk, entries, exits and get structured responses grounded in day trading strategy
- **Live chart panel** — Chart.js price visualization with configurable timeframes
- **Sidebar navigation** — Organized sections for watchlist, positions, analysis, and strategy reference
- **Dark terminal theme** — Green/red accent on near-black, built for extended screen time
- **Knowledge base integration** — Responses reference Day Trading 101 (Borman) methodology rather than generic AI output
- **Self-contained** — Single HTML file, runs entirely in browser

## Usage

```bash
# Just open it
start trading-agent.html        # Windows
open trading-agent.html         # macOS
xdg-open trading-agent.html     # Linux
```

Or drag it into any browser window.

## Tech Stack

- Vanilla HTML / CSS / JavaScript
- Chart.js 3.9.1 (CDN)
- CSS custom properties for theming
- No framework, no build step

## Planned Enhancements

- [ ] RAG pipeline connecting to live knowledge base (LangChain + Chroma)
- [ ] Real-time market data feed (Alpaca / Polygon.io API)
- [ ] Broker integration for paper trading (Alpaca)
- [ ] Local LLM backend option (Ollama) for offline use
- [ ] Multi-agent layer — separate analysis and execution agents

## License

MIT
