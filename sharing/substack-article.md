# What Happens When Everything Breaks at Once: Modeling the Iran War from Resource Constraints

*Most war analysis focuses on who wins on the battlefield. I built a different kind of model — one that starts from physical supply chains and traces what happens when 18 critical resources break simultaneously. The answer surprised me.*

---

The Iran War has a winner. It's not the US. It's not Israel. It's not Iran.

The winner is China. And China didn't fire a single shot.

That's the headline finding from a 76-file geopolitical simulation I built using AI research agents — modeling the war from physical resource constraints upward rather than from political assumptions downward. Instead of asking "who has the better military," the model asks: what happens when helium, bromine, fertilizer, oil, and fourteen other critical inputs stop flowing through the same chokepoint at the same time?

The answers are more concrete — and more unsettling — than anything you'll read in op-ed commentary.

---

## The Supply Chain Nobody Talked About

The Strait of Hormuz was always described as an "oil chokepoint." That's true but incomplete. What the resource-level analysis reveals is that Hormuz is actually a **polycrisis chokepoint** — a single geographic bottleneck for at least six unrelated supply chains that all feed modern civilization.

When Hormuz closed in February 2026, these disruptions hit simultaneously:

**Helium: 33% of global supply went offline.** Qatar's Ras Laffan complex is the world's largest helium source. No helium means no semiconductor fabrication — it's used for wafer cooling and EUV lithography. It also means no MRI machines, no cryogenics research, no space launch infrastructure.

**Fertilizer: One-third of global trade was disrupted.** The Northern Hemisphere was weeks away from spring planting. Crops went into the ground with insufficient nitrogen, phosphate, and potash. By the time you read this, Q3-Q4 yields are already locked in — 1 billion people face food insecurity regardless of whether the war ends tomorrow.

**Polyethylene: 84% of Middle Eastern exports were stranded.** This is the one nobody talks about. Polyethylene is in every plastic package, every food wrapper, every medical device. The food crisis has a packaging crisis stacked on top of it.

**Sulphur: 24-44% of production was affected.** Sulphur doesn't sound important until you realize it's required for copper smelting. Copper is the backbone of the green energy transition. No sulphur = no copper = no solar panels, no EVs, no grid modernization.

**Bromine: 67% of global supply is now in an active war zone.** Israel and Jordan's Dead Sea operations produce two-thirds of the world's bromine. It's used in flame retardants — which are in every circuit board, every chip package, every piece of electronics. There is no substitute that meets fire safety standards.

**LNG: 17% of global supply went offline for 3-5 years.** Qatar's LNG infrastructure isn't coming back quickly. Taiwan has 11 days of LNG reserves. Japan runs ~80% of its oil through Hormuz. The energy security crisis is structural, not temporary.

---

## The Cascade Effect: When Disruptions Compound

Here's where the model gets interesting. Each of these disruptions is significant on its own. But the real story is how they interact.

The semiconductor industry is hit by **three independent input crises simultaneously**: helium (33% offline), bromine (67% at risk), and neon (combinatorial risk from Ukraine war spillover). There's no single-source fix. A chip fab can't just "find alternative helium" when bromine is also gone and neon is constrained. The model shows a **30-50% chip output cut** — not from any factory being bombed, but from three separate supply chains breaking at once.

The food crisis has a similar cascade structure. Fertilizer disruption → crop yields decline → but also polyethylene disruption → food packaging fails → spoilage increases → the same crop yields that are already down deliver less edible food. The model calls this a "spoilage multiplier" — every ton of food that survives the fertilizer shock loses another 15-20% to packaging and logistics failures.

Insurance creates the most counterintuitive cascade. Lloyd's of London withdrew war-risk coverage for Hormuz transit. The immediate effect was a 92% traffic collapse. But the deeper effect is the **$1:$390 trade multiplier** — for every dollar of insurance withdrawn, $390 of trade freezes. Ships aren't being sunk; they're being uninsured. And insurance designations persist for weeks to months after any ceasefire. The economic damage outlasts the shooting.

---

## The Winner: "China Has the Periodic Table"

The US has 11 aircraft carriers. China has none.

But China controls rare earth processing. China refines 99% of the world's gallium and 83% of its germanium. China processes 78% of global cobalt and 65-75% of lithium. China is the only major economy insulated from Hormuz disruption.

When the model runs the scenarios, China emerges as the strategic winner in every outcome except Iranian nuclear breakout (a 10% probability scenario that's catastrophic for everyone). In the most likely scenario — a negotiated wind-down by late 2026 — China achieves:

- First permanent naval presence in the Gulf (55% probability)
- Yuan-denominated oil purchases rising 30-40%
- Mediator position that gives it influence over post-war reconstruction
- Accelerated leverage over Taiwan through demonstrated US munitions depletion

The US won the military war in hours. But the war was never going to be decided by who wins the dogfights. It was decided by who controls the inputs to modern civilization — and China holds more of them than any analysis I've seen acknowledges.

---

## Five Predictions (With Dates)

The model produces specific, falsifiable predictions. Here are the five I'd put money on:

**1. Late April: The Pharma Cliff.** Pharmaceutical buffer stocks exhaust roughly 60 days after Hormuz closure. Antibiotic and metformin shortages begin globally. China controls 70% of India's active pharmaceutical ingredient imports. This one hits in four weeks — the fastest testable prediction in the model.

**2. May-June: First Harvest Damage Visible.** The fertilizer disruption shows up in wheat yield data. The food crisis transitions from "predicted" to "observed." Prices haven't peaked yet, but the supply side is now locked.

**3. July-August: Taiwan's 11-Day Clock.** Summer energy demand peaks. Taiwan's 11-day LNG reserve becomes a live vulnerability. Helium shortage hits TSMC. China doesn't need to invade — "enhanced customs inspections" on tankers achieves coercive leverage. The model puts gray zone escalation at 35-45% probability.

**4. November 3-27: The 24-Day Gauntlet.** US midterms (Nov 3) + China's gallium/germanium export ban resumption (Nov 27) + EU winter gas storage crisis (Dec 1). Three independent pressure peaks in 24 days. This is the maximum leverage moment for China and the maximum stress moment for US decision-making.

**5. 1 → 5 Nuclear States.** Even the best-case scenario leaves Iran with 440.9 kg of 60% enriched uranium as a permanent threshold state. This alone triggers Saudi acquisition via Pakistan (6-24 months). Then Japan (6-12 months — they have 44.4 tonnes of separated plutonium), Turkey (3-7 years), and South Korea (1-2 years). The NPT doesn't survive this war.

---

## The $650 Billion AI Delay

One more prediction that deserves its own section: the AI infrastructure buildout just got delayed by 6-12 months.

Data centers are energy-hungry, chip-dependent, helium-needing facilities. All three inputs are now constrained. The model shows the $650 billion global AI infrastructure buildout hitting a wall from three directions simultaneously.

This isn't about research progress — papers will keep coming. It's about physical infrastructure: the fabs, the data centers, the power plants, the cooling systems. The atoms, not the bits.

The irony: nuclear energy is the only technology both accelerated by this war AND not China-dependent at the reactor level. Data centers are already redirecting to nuclear sites. The AI boom might accidentally accelerate the nuclear renaissance.

---

## How This Model Was Built

The simulation was built using Claude Code as an orchestration layer, deploying parallel research agents — one for each of 18 resources, 18 countries, and 20 cascade pathways. Each agent produced a self-contained deep dive with sourced data from news outlets, think tanks, and government reports dated February-March 2026.

The knowledge architecture uses what I'm calling an "Agentic Brain" — six intelligence layers where each layer cites the one below it, creating a traceable chain from raw data → resource analysis → country incentives → industry impact → cascade modeling → integrated simulation.

All 76 files are open source under CC BY 4.0. You can browse the full analysis, chat with the research via Google NotebookLM, or dig into the source code.

---

## The Bottom Line

Wars are resource disruption events. The side with better weapons doesn't automatically win — the side that remains connected to the inputs of modern civilization does.

Right now, China is more connected than the US to the periodic table, to the processing infrastructure, and to the mediator role that shapes whatever peace emerges.

The US has aircraft carriers. China has the periodic table.

That's not a military problem. It's a systems problem. And systems problems don't get solved by better missiles.

---

**Explore the full analysis:** [coderexpert123.github.io/war-games-2026](https://coderexpert123.github.io/war-games-2026/)

**Chat with the research:** [NotebookLM](https://notebooklm.google.com/notebook/4cf9474f-194d-4607-8953-8ee84a9e66e0)

**Source code:** [GitHub](https://github.com/coderexpert123/war-games-2026)

---

*All claims sourced from major news outlets, think tanks, and government reports dated February-March 2026. This is an open-source research project, not classified intelligence.*
