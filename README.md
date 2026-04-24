# 2026 Iran War: Geopolitical & Resource Cascade Analysis

**99 files. 18 resources. 18 countries. 20 cascade models. 5 probability-weighted scenarios.**

**[Chat with this research](https://notebooklm.google.com/notebook/4cf9474f-194d-4607-8953-8ee84a9e66e0)** | **[Browse the site](https://coderexpert123.github.io/war-games-2026/)**

A bottom-up geopolitical simulation of the 2026 Iran War (US/Israel vs Iran, started Feb 28), built entirely from open-source intelligence. Unlike top-down political punditry, this analysis starts from physical resource constraints — oil flows, mineral supply chains, semiconductor inputs, food systems — and models how disruptions cascade across industries, countries, and each other simultaneously.

Built using Claude as a network of parallel research agents, with each resource, country, and cascade analyzed independently, then integrated into a unified simulation.

## Why This Exists

Most war analysis focuses on military operations and diplomacy. This project asks different questions:

- What happens when **33% of global helium** goes offline and chip fabs can't run?
- What happens when **67% of the world's bromine** (Dead Sea, Israel/Jordan) is in a war zone and every circuit board needs flame retardants?
- What happens when **fertilizer shipments through Hormuz stop** and the Northern Hemisphere has already planted with insufficient inputs?
- What happens when all of these hit **simultaneously**?

The answer: cascades compound in ways that no single-issue analysis captures. That's what this project models.

## Key Findings

**China is the war's strategic winner.** It controls rare earth processing, is insulated from Hormuz disruption, and holds a November 2026 deadline on gallium/germanium exports that gives it maximum leverage over the US mid-war. Every week the war continues, China's relative position strengthens.

**The chip famine is structural, not transient.** Three independent semiconductor inputs — helium (33% offline), bromine (67% at risk), neon (combinatorial risk) — are disrupted simultaneously. Combined with Taiwan's 11-day LNG reserve, chip production faces a 30-50% output cut that no single-source workaround can fix.

**The food crisis is already locked in.** Northern Hemisphere spring planting (March-May 2026) is happening with disrupted fertilizer supply. Even if the war ends tomorrow, Q3-Q4 crop yields will disappoint. 1 billion+ people face food insecurity by late 2026.

**November 2026 is the convergence point.** US midterm elections (Nov 3), China's gallium/germanium export ban deadline (Nov 27), and Europe's winter energy crisis (Dec 1) all collide. This is when maximum political, economic, and strategic pressure peaks simultaneously.

**Insurance outlasts the war.** Lloyd's war-risk designations persist weeks to months after ceasefire. The $1:$390 trade multiplier means insurance disruption freezes far more economic activity than the physical damage alone.

## How It's Structured

The analysis is organized in seven intelligence layers, each building on the one below:

```
Layer 7: COMMUNICATION        Public assets, outreach, distribution to external audiences
Layer 6: BLIND SPOTS          What we don't know and might be wrong about
Layer 5: SIMULATION            Phase-by-phase predictions and scenarios
Layer 4: CASCADES              How disruptions compound across domains  ← the analytical core
Layer 3: INDUSTRIES            Sector-specific impact (chips, food, pharma, defense, auto, energy)
Layer 2: ACTORS                Country-by-country incentive analysis
Layer 1: RESOURCES             Production, prices, trade flows, stockpiles
```

Every claim cites the layer below it. Simulation cites cascades. Cascades cite industries and resources. Resources cite primary sources with dates.

### Start Here

| If you want... | Read this |
|----------------|-----------|
| The integrated prediction | [`simulation/master-simulation.md`](simulation/master-simulation.md) |
| Every actor's position at a glance | [`simulation/incentive-map.md`](simulation/incentive-map.md) |
| Probability-weighted scenarios & opportunities | [`simulation/scenarios-and-opportunities.md`](simulation/scenarios-and-opportunities.md) |
| How cascades compound | [`cascades/combinatorial-matrix.md`](cascades/combinatorial-matrix.md) |
| The November 2026 convergence | [`cascades/november-2026-convergence.md`](cascades/november-2026-convergence.md) |
| What we might be wrong about | [`blind-spots/analysis.md`](blind-spots/analysis.md) |

### Full Coverage

<details>
<summary><strong>18 Resources Analyzed</strong></summary>

Oil & gas, helium, rare earths, fertilizers, munitions, shipping insurance, bromine, sulphur, gallium-germanium, uranium, polyethylene, lithium, cobalt, copper, titanium, neon, construction materials, platinum group metals

[Full resource index](resources/00-resource-index.md)
</details>

<details>
<summary><strong>18 Countries/Regions Analyzed</strong></summary>

United States, Israel, Iran, China, Russia, India, European Union, Gulf States (Saudi/UAE/Qatar/Bahrain/Iraq/Egypt/Jordan), South Korea, Pakistan, North Korea, Japan, Africa, Latin America, Turkey, Central Asia, Southeast Asia, Lebanon/Hezbollah

[Full country index](countries/00-country-index.md)
</details>

<details>
<summary><strong>6 Industries Analyzed</strong></summary>

Semiconductors & AI, defense industrial base, food & agriculture, pharmaceuticals, automotive, energy transition

[Full industry index](industries/00-industry-index.md)
</details>

<details>
<summary><strong>20 Cascade Models</strong></summary>

Combinatorial matrix, November 2026 convergence, water crisis, cyber escalation, insurance systemic risk, migration & remittances, cryptocurrency & alternative finance, space & satellite vulnerability, information warfare, climate compounding, domestic unrest, health & environmental effects, nuclear proliferation, global financial contagion, Yemen/Houthi/Red Sea, maritime chokepoint network, Sunni-Shia dynamics, Ukraine war interaction, China-Taiwan window

[Full cascade index](cascades/00-cascade-index.md)
</details>

## Methodology

- Parallel research agents deployed per resource, per country, and per cascade — not a single narrative thread
- All claims sourced from major news outlets, think tanks, and government reports (Feb-March 2026)
- Analysis built bottom-up from resource constraints, not top-down from political assumptions
- Verified facts distinguished from reasonable inferences distinguished from speculation
- Combinatorial analysis identifying correlated disruption cascades that single-issue analysis misses

### Public Assets & Distribution

For journalists, researchers, and content creators, the following public-facing assets are available:

| Asset | Description | Link |
|--------|-------------|------|
| **Interactive Site** | Browse all analysis, cross-linked by resource/country/industry/ cascade | [coderexpert123.github.io](https://coderexpert123.github.io/war-games-2026/) |
| **NotebookLM Chat** | Chat with the entire research corpus | [NotebookLM](https://notebooklm.google.com/notebook/4cf9474f-194d-4607-8953-8ee84a9e66e0) |
| **HTML Infographic** | Screenshot-ready cascade visualization | [sharing/infographic.html](sharing/infographic.html) |
| **Substack Article** | 1500-word narrative summary | [sharing/substack-article.md](sharing/substack-article.md) |
| **YouTube Script** | 10-minute explainer with visual cues | [sharing/youtube-script.md](sharing/youtube-script.md) |
| **Podcast Script** | 10-minute conversational audio script | [sharing/podcast-script.md](sharing/podcast-script.md) |
| **Press Release** | Formal media announcement | [sharing/press-release.md](sharing/press-release.md) |

All assets are licensed under CC BY 4.0. Feel free to adapt and reuse with attribution.



## How This Was Built

This entire repository was built using [Claude Code](https://claude.com/claude-code) (Anthropic's CLI agent) as an orchestration layer. The process:

1. **Parallel deep dives**: 8+ research agents deployed simultaneously, each investigating a single resource, country, or cascade in depth
2. **Bottom-up integration**: Findings aggregated into cascade models that identify compounding interactions
3. **Simulation synthesis**: All layers combined into probability-weighted scenarios
4. **Continuous updates**: As the war evolved day-by-day, new intelligence was integrated and cascades re-traced

The project's knowledge management uses an "Agentic Brain" architecture — a structured system of intelligence layers, navigational indexes, and dependency tracking that allows AI agents to efficiently navigate and update 76 interconnected files.

## Caveats

- All analysis is based on open-source reporting as of March 24, 2026
- Wars are inherently unpredictable — a single escalation could redirect everything
- This is an analytical framework, not a crystal ball
- Resource data has reporting lags; some figures may be outdated by days or weeks

## License

This work is licensed under [CC BY 4.0](LICENSE). You're free to share and adapt it with attribution.
