# OMNISCIENCE X

### A collective intelligence engine. Not a language model. Something different.

One HTML file. No API key. No server. No cost. Just open it.

---

I kept asking myself why every AI company is trying to build a better chatbot. More parameters. More training data. More compute. And none of them can tell you *why* they said what they said.

So I tried the opposite. What if instead of predicting the next word, you actually mapped knowledge as a graph — concepts connected by real relationships — and then reasoned through it step by step, showing everything?

That's what this is.

**Omniscience X** pulls knowledge from ConceptNet (34 million facts) and Wikipedia in real time, builds a reasoning graph, chains causation across multiple hops, finds contradictions, scores confidence, discovers analogies across domains, and shows you every single step of how it got to its answer.

It's rough. The NLU is regex-based and breaks on complex sentences. The graph viz slows down past 500 nodes. It's a prototype, not a product.

But the core idea works. And I think it matters.

---

## Just Try It

1. Download `omniscience-x.html`
2. Open in your browser
3. Ask it something

No install. No signup. No API key. Nothing.

Try:
- `what is photosynthesis`
- `compare dogs and cats`
- `why do humans dream`
- `what if the internet disappeared`
- `connect music and mathematics`

---

## What It Actually Does

**Learns from the web in real time.** Ask about something it doesn't know and it goes to ConceptNet and Wikipedia, pulls structured facts, adds them to the graph, reasons over them. You watch the knowledge appear.

**Learns from you.** Say "stress increases cortisol" or "dogs are mammals" and it creates graph edges, auto-deduces implications, generates hypotheses from the structure.

**Chains causation.** Ask "why is inflation rising" and it walks the graph: money supply up → spending up → demand up → prices up → inflation. Every link has a confidence percentage. Every step is visible.

**Handles contradictions properly.** Teach it "nuclear energy is safe" then "nuclear energy is dangerous." It doesn't pick a side. It keeps both, flags the contradiction, shows source counts. You see the disagreement instead of a fake consensus.

**Runs counterfactuals.** Ask "what if the sun disappeared" and it traces every causal chain forward from the sun, inverts each one, shows the cascade with confidence scores.

**Finds analogies.** The engine looks for concepts that share graph structure but not meaning — cross-domain parallels that nobody explicitly taught it.

**Three views:**
- **Dialogue** — chat with it, reasoning chains shown inline
- **Knowledge Graph** — force-directed visualisation of everything it knows, updating live
- **Reasoning Trace** — every cognitive step for every response, fully transparent

---

## How It Works (Short Version)

Every concept is a node with a 32-dimensional embedding. Connections are typed — is_a, causes, increases, decreases, prevents, enables, etc. — and weighted by confidence.

When you ask something, it parses intent, activates relevant concepts, spreads activation through the graph, finds multi-hop paths, runs deduction and abduction, checks for analogies, and builds a response where every claim traces back to a specific graph traversal.

Confidence propagates through chains and degrades at each hop. A→B at 90% then B→C at 80% gives 72% for the full chain. Contested edges halve confidence automatically.

Web enrichment hits ConceptNet and Wikipedia APIs (both free, no key). Facts come back as structured relationships that slot into the graph with source tags.

Everything saves to browser storage. Close the tab, come back, your graph is still there.

---

## Two Versions

`omniscience.html` — base engine. You teach it everything. No web calls.

`omniscience-x.html` — full version. Learns from you AND pulls from ConceptNet + Wikipedia live.

Both have the knowledge graph, multi-hop reasoning, contradiction detection, confidence scoring, analogies, counterfactuals, and memory.

---

## Why I Think This Matters

Every AI right now is a black box. You ask, you get an answer, no idea how it got there. If it's wrong you can't tell. If it's uncertain it doesn't say. If experts disagree it picks a side and acts confident.

Fine for writing emails. Not fine for medical decisions, legal questions, policy analysis, or anything where being wrong actually matters.

This is the opposite approach. Every claim has a confidence score. Every connection has a source. Every contradiction is visible. Every reasoning step is shown. You can audit every response and challenge any link.

It won't write you a poem. Won't have a warm conversation. But it'll show you exactly why it thinks what it thinks and be honest about what it doesn't know.

I think there's room for both approaches and the transparent one is massively underbuilt.

---

## What's Missing (Honestly)

It's a browser prototype. One HTML file. Works for one person. To work at scale it needs:

- A graph database (Neo4j) replacing the JavaScript arrays in memory
- A server so multiple people share one graph
- Real-time sync so you see other people's contributions
- Better NLU (the regex parser is the weakest part by far)
- User auth and trust scoring
- Graph viz that doesn't choke past 500 nodes

None of that is research. It's engineering. Every function in the HTML maps directly to a backend operation.

---

## Looking for a Backend Engineer

I built the engine. I need someone to build the platform underneath it.

If you know Node.js and Neo4j and you want to work on something that isn't another CRUD app — read the code, read the [vision doc](VISION.md), and [open an issue](../../issues) if it clicks.

Not looking for a contractor. Looking for someone who sees where this goes and wants to help get it there.

---

## Contributing

PRs welcome. Big priorities:

1. **NLU** — the intent parser is regex. Anything smarter helps massively.
2. **More knowledge sources** — Wikidata, DBpedia, anything structured and free
3. **Graph viz performance** — WebGL, spatial indexing, neighbourhood rendering
4. **Mobile** — works but needs touch controls on the graph
5. **Import/export** — share graphs as JSON
6. **The backend** — the big one

See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

---

## License

MIT. Do what you want with it.

---

## FAQ

**Is this AI?**
Depends what you mean. No neural network. Doesn't predict text. It reasons over a knowledge graph — traverses relationships, chains causation, propagates confidence. Closer to expert systems than to GPT, but with live web learning and modern graph structure.

**Can it replace ChatGPT?**
No. Different tool, different job. ChatGPT generates text fluently. This shows structured reasoning transparently. Use ChatGPT for conversation, use this for understanding *why*.

**Why one HTML file?**
To prove the concept without needing money, a team, or infrastructure. If the idea is good, the rest follows.

**Where does my data go?**
Stays in your browser. Nothing sent anywhere except read-only queries to ConceptNet and Wikipedia public APIs. Your graph is local.

---

*February 2026*
