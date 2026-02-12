# Contributing

## Getting Started

The whole project is two HTML files. Download one, open it in a browser, you're running it. No build step, no dependencies, no package.json.

## What Would Help Most

### Better NLU (Biggest Bang for Buck)
The intent parser runs on regex. It catches structured input fine but falls apart on natural language. Swapping in something like [Compromise.js](https://github.com/spencermountain/compromise) or even a basic dependency parser would make a huge difference to the user experience.

### The Backend (The Big One)
Moving from a single-user browser app to a shared multi-user system. See the README for details. Short version: Neo4j for the graph, Node.js API, WebSocket for real-time sync, Supabase for auth. The HTML file is basically the spec — every JavaScript function tells you what the backend needs to do.

### More Knowledge Sources
Currently pulls from ConceptNet and Wikipedia. Other free structured APIs worth adding:
- [Wikidata](https://www.wikidata.org/) — structured entity data
- [DBpedia](https://www.dbpedia.org/) — Wikipedia but as structured data
- Any other open knowledge graph

### Graph Viz Performance
The Canvas 2D force layout gets sluggish past ~500 nodes. Ideas:
- WebGL renderer
- Quadtree for force calculations
- Only show labels on zoom
- Neighbourhood view instead of rendering the entire graph

### Mobile
Technically works on mobile already but the graph view needs pinch-to-zoom and proper touch drag.

### Import/Export
Being able to dump your graph to JSON and load someone else's would let people share knowledge without needing a backend.

## How to Contribute

1. Fork it
2. Branch off (`git checkout -b feature/whatever`)
3. Make changes
4. Test by opening the HTML in a browser
5. PR it

That's it. No CI pipeline. No linting config. Just make the HTML file better.

## Code Layout

Both HTML files are self-contained. Sections are marked with comment headers:

- **Knowledge Graph** — Node/Edge classes, graph operations, spreading activation
- **Web Knowledge** (X version) — ConceptNet + Wikipedia integration
- **Logic Engine** — deduction, forward chaining, abduction
- **Analogy Engine** — cross-domain structure mapping
- **Memory** — episode storage and pattern consolidation
- **NLU** — intent parsing, concept extraction
- **Reasoning Engine** — the orchestrator that ties it all together
- **Graph Viz** — force-directed layout, Canvas rendering
- **UI** — chat, tabs, panels
- **Persistence** — save/load to browser storage

## Questions

Open an issue. Happy to talk through architecture or priorities.
