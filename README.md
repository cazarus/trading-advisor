# Trading Advisor

> ⚠️ **Currently in active development. Code will be published as modules are completed.**

A conversational AI trading advisor agent built on a RAG (Retrieval-Augmented Generation) architecture. Uses *Day Trading 101* by David Borman as the core knowledge base, supplemented by real-time market data feeds and broker integrations.

## Concept

The system operates as a dialogue-driven advisor — you describe your position, risk tolerance, or a market scenario, and the agent retrieves relevant strategy context from the knowledge base, cross-references live data, and surfaces actionable insights grounded in established day trading methodology rather than hallucinated generalities.

## Planned Architecture

```
User Query
    │
    ▼
[RAG Retrieval Layer]  ←──  Day Trading 101 knowledge base (chunked + embedded)
    │
    ▼
[Market Data Layer]  ←──  Real-time price feeds (Alpaca / Polygon.io / yfinance)
    │
    ▼
[AI Reasoning Layer]  ←──  Claude / local LLM
    │
    ▼
[Broker Integration]  ←──  Alpaca paper trading → live
    │
    ▼
Advisory Output + Execution Proposal
```

## Planned Features

- **RAG knowledge base** — Borman's Day Trading 101 chunked, embedded, and queryable
- **Real-time data** — Price, volume, and options flow via market API
- **Conversational interface** — Ask questions, get grounded, sourced answers
- **Position analysis** — Input your current holdings and get risk/exit context
- **Broker integration** — Alpaca API for paper trading and eventual live execution
- **Multi-agent layer** — Separate analysis and execution agents with human approval gate

## Tech Stack (Planned)

- Python, LangChain or custom RAG pipeline
- Vector DB: Chroma or Qdrant
- Market data: Alpaca Markets API, Polygon.io
- LLM: Claude API + local Ollama fallback
- Broker: Alpaca paper → live

## Status

- [x] Architecture designed
- [x] Knowledge base source identified
- [ ] Document ingestion and embedding pipeline
- [ ] RAG retrieval layer
- [ ] Market data integration
- [ ] Conversational interface
- [ ] Broker API connection
- [ ] Paper trading validation

## License

MIT
