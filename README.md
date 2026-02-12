# OMNISCIENCE X

### What if a million people taught one AI everything they know — and you could see exactly how it thinks?

---

Not a chatbot. Not a language model. A **collective intelligence engine** that learns from people and the web, reasons through chains of causation, detects contradictions, and shows you every single step.

One HTML file. No API key. No server. No cost.

---

## The Problem Nobody's Solving

Every AI right now is a black box. You ask ChatGPT a question, you get a confident answer, and you have **no idea** if it's true, where it came from, or how certain it actually is. If experts disagree, it picks a side and acts like it's fact. If it's wrong, you can't tell.

That's fine for writing emails. It's dangerous for medical decisions, legal questions, investment analysis, or anything where being wrong has consequences.

## What This Does Instead

Omniscience X takes the opposite approach. It maps knowledge as a **graph** — concepts connected by real relationships (causes, prevents, increases, decreases) — and reasons through it step by step, showing everything.

Ask it a question. It shows you:
- **Every reasoning step** it took to reach the answer
- **Confidence scores** on every single claim
- **Source counts** — how many people independently confirmed each fact
- **Contradictions** — when evidence conflicts, it shows both sides instead of hiding one
- **The full causal chain** — not just "A causes B" but "A causes B which increases C which leads to D" with confidence degrading at each hop

**You can challenge any link in the chain.** If one step is wrong, you can see exactly which one and why.

---

## Why This Gets Exciting At Scale

Right now it's a prototype for one person. But the architecture is built for millions.

### 10,000 Users: Better Than Any Single Expert

Imagine 10,000 people — doctors, engineers, teachers, farmers, mechanics, economists — all teaching it what they know.

Someone asks: **"I have a headache, blurred vision, and neck stiffness"**

The graph returns:
- **Meningitis** — 89% confidence, 3,200 sources (headache + neck stiffness + blurred vision pattern)
- **Migraine with aura** — 74% confidence, 1,800 sources
- **Hypertensive crisis** — 61% confidence, 800 sources

And crucially it shows **why**: headache + neck stiffness + **fever** points to meningitis (2,400 sources). Without fever it points to migraine (1,200 sources). The distinguishing symptom is visible. The confidence is visible.

No single doctor has seen every disease. But 3,200 medical professionals independently teaching symptom-disease connections? That graph knows patterns no individual could hold in their head.

### 100,000 Users: It Discovers Things Nobody Taught It

A doctor teaches: "cortisol suppresses immune function."
An economist teaches: "unemployment increases stress."
A neuroscientist teaches: "stress increases cortisol."
A sociologist teaches: "automation increases unemployment."
An engineer teaches: "AI increases automation."

Nobody teaches the full chain. But the graph connects it:

**AI → automation → unemployment → stress → cortisol → immune suppression → disease**

Seven hops. Five different professions. One emergent insight that **no single expert could see** because nobody works across all five fields. The reasoning engine finds it automatically. Every link independently verified by thousands of people.

That's not artificial intelligence. It's collective intelligence with a reasoning engine underneath.

### 1 Million Users: A Prediction Engine

The causal chains get dense enough to **predict consequences before they happen**.

A government announces interest rate rises. The graph traces every known downstream chain:

Interest rates rise → mortgage costs increase (99%, 500K sources) → house purchases decrease (96%) → construction slows (91%) → construction jobs decrease (88%) → local spending drops (79%)

**Simultaneously:** currency strengthens (86%) → exports become expensive (82%) → manufacturing competitiveness falls (76%)

**Simultaneously:** savings increase (94%) → consumer spending falls (87%) → retail jobs decrease (83%)

Four parallel cascade chains running simultaneously. Each link verified by hundreds of thousands of independent people. Confidence degrading at each hop so you see exactly where prediction becomes speculation.

No economist models all sectors simultaneously. The graph does — because a million people from every sector taught it their piece.

### At Scale: It Finds Leverage Points In Complex Problems

Every big problem — poverty, climate, disease — is a web of causal chains. Most interventions fail because they target the wrong point.

The graph can find **convergence nodes** — places where the most causal chains intersect. The single interventions that cascade through the most downstream effects.

Ask "how do we reduce poverty" and it traces every chain backward. Maybe **female education** appears upstream of: reduced birth rates, improved child nutrition, improved child health, increased economic participation, improved governance. One node upstream of dozens of outcomes. Found not by ideology but by graph topology over billions of verified edges.

### At Billion Scale: It Maps Human Ignorance

Dense clusters show what humanity understands well. **The empty spaces between clusters show what we haven't figured out yet.**

The void between neuroscience and consciousness? That's the hard problem of consciousness — visible, measurable, specific.

The graph could generate a ranked list of the **most important unanswered questions in human knowledge** — the biggest gaps between the densest clusters. That list would be worth more than every research grant ever issued. It would tell researchers exactly where to look.

---

## What Makes This Different From Everything Else

| | ChatGPT / Claude | Google | Wikipedia | **Omniscience X** |
|---|---|---|---|---|
| Shows reasoning | ❌ | ❌ | ❌ | ✅ Every step visible |
| Confidence scores | ❌ | ❌ | ❌ | ✅ Every claim scored |
| Contradictions | Picks one answer | Shows all results | One consensus | ✅ Both sides preserved |
| Source tracing | ❌ | Links only | Citations | ✅ Source count per edge |
| Learns from you | ❌ | ❌ | Edit process | ✅ Real-time |
| Predicts cascades | ❌ | ❌ | ❌ | ✅ Multi-hop forward propagation |
| Runs locally | ❌ | ❌ | ❌ | ✅ One HTML file |
| Cost | $20/month+ | Free | Free | ✅ Free forever |

---

## Try It Right Now

1. Download `omniscience-x.html`
2. Open in your browser (not inside another app — directly in Chrome/Firefox/Safari)
3. Start asking questions

No install. No signup. No API key.

Try:
- `what is photosynthesis`
- `compare dogs and cats`
- `why do humans dream`
- `what if the internet disappeared`
- `connect music and mathematics`

It pulls live from **ConceptNet** (34 million common-sense facts) and **Wikipedia** in real time, builds a reasoning graph, and shows you every step.

---

## Three Views

**Dialogue** — chat with it, see reasoning chains and confidence scores inline

**Knowledge Graph** — live force-directed visualisation of its entire mind, updating in real time. Blue = confirmed. Purple = web-learned. Gold = contested.

**Reasoning Trace** — every cognitive operation visible. Intent → concept extraction → spreading activation → path-finding → deduction → hypothesis → confidence. Nothing hidden.

---

## How It Works

**Knowledge Graph** — concepts as nodes with 32-dimensional embeddings, connected by typed relationships (is_a, causes, prevents, increases, decreases, has, can, part_of, similar_to, is_not) weighted by confidence and source count.

**Web Enrichment** — queries ConceptNet and Wikipedia APIs (free, no key) in real time. Extracts structured facts and integrates them into the graph. You watch it learn.

**Multi-Hop Reasoning** — chains causation up to 6 hops. Confidence degrades at each step. A→B at 90% then B→C at 80% = 72% overall. Contested edges halve confidence.

**Contradiction Detection** — opposite relations tracked (causes/prevents, increases/decreases, is/is_not). Both sides preserved with independent scores. Shows the real disagreement.

**Analogy Engine** — finds cross-domain structural parallels. Heart↔pump, economy↔ecosystem. Emerges from graph topology, not from anyone teaching it.

**Counterfactual Analysis** — "what if X disappeared?" Traces causal chains forward, inverts each, shows the full cascade.

**Episodic Memory** — stores conversations, recalls by relevance, consolidates patterns over time.

---

## What's Missing (Honestly)

It's a prototype. One person, one browser. The NLU breaks on complex sentences. The graph viz slows past 500 nodes.

To become what's described above it needs:
- Graph database (Neo4j) replacing in-memory arrays
- Server for shared multi-user graph
- Real-time sync between users
- Better natural language understanding
- Trust scoring and moderation

All solved problems. The gap is engineering, not research.

---

## Looking for a Backend Engineer

I built the reasoning engine. I need someone to build the platform underneath.

Node.js + Neo4j + WebSocket. The HTML file is the spec — every function tells you what the backend needs to do.

Not looking for a contractor. Looking for someone who reads the [vision doc](VISION.md) and thinks "I need this to exist."

[Open an issue](../../issues) if that's you.

---

## Contributing

PRs welcome. Priorities:

1. **NLU** — replace regex with proper natural language understanding
2. **Response quality** — readable answers backed by visible graph data
3. **More knowledge sources** — Wikidata, DBpedia, anything structured and free
4. **Graph viz** — WebGL rendering, neighbourhood view, performance at scale
5. **Import/export** — share graphs as JSON

See [CONTRIBUTING.md](CONTRIBUTING.md).

---

## The Bet

Transparent reasoning over structured knowledge — where every claim is traceable and every contradiction is visible — is more valuable for serious decisions than fluent text from a black box.

Language models sound human.
Knowledge graphs show truth — and show why.

The world needs both. Only one is a billion-dollar industry. This is a shot at building the other.

---

## License

MIT.

---

*February 2026*
