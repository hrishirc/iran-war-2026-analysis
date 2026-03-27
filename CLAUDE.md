# Iran War 2026 Analysis — Project Brain

## What This Project Is
A comprehensive geopolitical and resource-level simulation of the 2026 Iran War (US/Israel vs Iran, started Feb 28 2026). Built from parallel research agents, resource-by-resource deep dives, and combinatorial cascade modeling.

---

## The Brain

### Intelligence Layers

Knowledge is organized bottom-up. Each layer cites the layer below it.

| Layer | Abstraction | Directory | Contents |
|-------|------------|-----------|----------|
| 1. Raw Data | Ground truth | `/resources/` | Production figures, prices, trade flows, stockpile levels. Each resource file is self-contained with sourced data points. |
| 2. Actor Analysis | First synthesis | `/countries/` | Per-country incentive maps: wants, fears, actions, paradoxes. Built from raw resource data + news reporting. |
| 3. Industry Impact | Domain synthesis | `/industries/` | How resource disruptions hit specific sectors (chips, AI, defense, food). Draws from multiple resource files. |
| 4. Cascade Modeling | Cross-domain synthesis | `/cascades/` | How disruptions compound across resources, industries, and countries simultaneously. The analytical core. |
| 5. Integrated Simulation | Prediction | `/simulation/` | Phase-by-phase predictions and scenarios. Built from all layers below. |
| 6. Gaps & Uncertainties | Meta-analysis | `/blind-spots/` | What we don't know, underweighted actors, wrong assumptions, unmodeled dynamics. |
| 7. Communication & Distribution | Audience reach | `/sharing/` | Public-facing assets, journalist outreach, social media templates. Communicates intelligence layers to external audiences. |

**Citation chain**: Simulation cites cascades. Cascades cite industries + resources. Industries cite resources. Countries cite resources + news. Resources cite primary sources (news, think tanks, government data).

### Brain Files

These are navigational indexes. They help you find knowledge, not hold it. Each has a "when to consult" purpose.

| Brain File | When to Consult | Location |
|-----------|-----------------|----------|
| **Resource Index** | Starting any resource-level research; checking what's been covered vs gaps | `resources/00-resource-index.md` |
| **Country Index** | Starting any country analysis; checking actor coverage | `countries/00-country-index.md` |
| **Cascade Index** | Starting any cascade analysis; understanding cross-domain interactions | `cascades/00-cascade-index.md` |
| **Industry Index** | Starting any industry analysis; checking sector coverage | `industries/00-industry-index.md` |
| **Incentive Map** | Quick reference for any actor's wants/fears/position | `simulation/incentive-map.md` |
| **Combinatorial Matrix** | Understanding how a change in one resource cascades to others | `cascades/combinatorial-matrix.md` |
| **Scenarios & Opportunities** | Probability-weighted outcomes, structural shifts, economic opportunities | `simulation/scenarios-and-opportunities.md` |
| **Blind Spots** | Before claiming simulation completeness; planning next research phase | `blind-spots/analysis.md` |
| **Master Simulation** | The current integrated prediction — the "answer" | `simulation/master-simulation.md` |
| **This file (CLAUDE.md)** | Orientation; how the brain works; conventions; priorities | You're here |

### Connections — Dependency Graph

The full dependency graph spans 76 files. This shows the architectural flow, not every individual connection. Consult each index file for detailed relationships.

```
LAYER 1: RESOURCES (19 files)
  resources/00-resource-index.md ◄── navigational index
  18 resource files ──────────────┬──→ LAYER 4: CASCADES
                                  └──→ LAYER 3: INDUSTRIES

LAYER 2: ACTORS (19 files)
  countries/00-country-index.md ◄── navigational index
  18 country/region files ────────┬──→ LAYER 4: CASCADES
                                  └──→ LAYER 5: SIMULATION

LAYER 3: INDUSTRIES (7 files)
  industries/00-industry-index.md ◄── navigational index
  6 industry files ───────────────┬──→ LAYER 4: CASCADES
                                  └──→ LAYER 5: SIMULATION

LAYER 4: CASCADES (20 files)  ◄── THE ANALYTICAL CORE
  cascades/00-cascade-index.md ◄── navigational index
  cascades/combinatorial-matrix.md ◄── master cascade framework
  18 cascade analysis files ──────┬──→ LAYER 5: SIMULATION
                                  └──→ each other (cascades compound)

LAYER 5: SIMULATION (8 files)
  simulation/master-simulation.md ◄── the integrated prediction
  simulation/incentive-map.md ◄── actor decision framework
  simulation/scenarios-and-opportunities.md ◄── probability-weighted outcomes
  simulation/war-termination-framework.md ◄── how it ends
  4 supporting analysis files

LAYER 6: META-ANALYSIS (1 file)
  blind-spots/analysis.md ◄── reads all layers; identifies gaps

LAYER 7: COMMUNICATION & DISTRIBUTION (22 files)
  sharing/00-sharing-guide.md ◄── navigational index
  5 public assets (committed) ──────┐
  17 private strategy files (local) ───┴──→ External audiences: journalists, social media, podcasts, video
```

**Key cascade clusters** (highest-impact cross-domain interactions):
- **November convergence**: rare-earths + china + US + EU + japan + south-korea → november-2026-convergence → master-simulation
- **Food crisis**: fertilizers + polyethylene + food-agriculture + climate → combinatorial-matrix
- **Chip famine**: helium + bromine + neon + semiconductors → combinatorial-matrix
- **Maritime network**: shipping-insurance + yemen-houthi + maritime-chokepoints + insurance-systemic-risk
- **Two-war interaction**: russia + ukraine-interaction + munitions + defense-industrial-base
- **China meta-cascade**: china + rare-earths + gallium-germanium + cobalt + lithium + china-taiwan-window

**Cascade propagation rules:**
- A change to any `/resources/` file may invalidate `/cascades/` and `/simulation/`
- A change to any `/countries/` file may invalidate `/simulation/incentive-map.md`
- New data should propagate: raw data → resource file → affected cascades → simulation update
- **Follow the dominoes**: when you update one file, trace all downstream effects in a single pass

---

## Working Principles

### Research Methodology
- Deploy parallel sub-agents per resource or country for maximum depth
- All claims must be sourced with publication name and date
- Distinguish verified facts from reasonable inferences from speculation
- Update simulation as new data becomes available
- When updating, follow the dominoes: resource → cascade → simulation

### Conventions
- Dates in ISO format or "Month Day, Year"
- All prices in USD unless noted
- Oil production in barrels per day (bpd)
- Minerals in metric tonnes
- Gas in million tonnes per annum (mtpa) for LNG, billion cubic meters (bcm) for pipeline
- Sources at bottom of each file with publication name and date

### When Adding New Content
1. Determine which intelligence layer it belongs to
2. Create or update the appropriate file
3. Update the relevant brain file (index)
4. Trace downstream: does this change any cascade? Does it change the simulation?
5. If it reveals a gap, add to `blind-spots/analysis.md`
6. Log the change below

---

## Priority Research Gaps

**All 8 original priority gaps filled.** All blind spot categories now covered. Research phase complete — next step is simulation rebuild. See `blind-spots/analysis.md` for the full coverage audit.

---

## Change Log

| Date | Change | Files Affected | Why |
|------|--------|---------------|-----|
| 2026-03-23 | Initial brain creation | All 23 files | First comprehensive build from conversation research |
| 2026-03-23 | Full brain architecture | CLAUDE.md | Intelligence layers, brain files, connections, propagation rules |
| 2026-03-23 | Gap fill: conversation content captured | 9 new files | War overview, wild cards, supply exhaustion, Russia/China incentives, bromine, sulphur, gallium-germanium, defense industrial base, food agriculture |
| 2026-03-23 | Scenarios & opportunities document | scenarios-and-opportunities.md | 5 probability-weighted scenarios, structural shifts, 4-tier opportunity framework, key dates calendar |
| 2026-03-24 | South Korea country analysis | countries/south-korea.md, 00-country-index.md, CLAUDE.md, blind-spots/analysis.md | Most resource-exposed developed economy; fills priority gap #1 from blind spots |
| 2026-03-24 | Uranium deep resource analysis | resources/uranium.md, resources/00-resource-index.md, CLAUDE.md | Nuclear breakout dimension, enrichment chokepoints, US import dependency, Iran stockpile analysis |
| 2026-03-24 | Polyethylene deep resource analysis | resources/polyethylene.md, resources/00-resource-index.md, CLAUDE.md | Food packaging cascade; 84% ME exports via Hormuz; 50% global capacity offline; spoilage multiplier on food crisis |
| 2026-03-24 | Water crisis cascade model | cascades/water-crisis-model.md, CLAUDE.md | Desalination as defining humanitarian threat; 4 escalation levels; energy-water nexus; migration cascade; fills priority gap #3 from blind spots |
| 2026-03-24 | November 2026 convergence analysis | cascades/november-2026-convergence.md, CLAUDE.md | Three-pressure convergence: midterms + gallium/germanium deadline + winter energy. Fills priority gap #5. Highest-value analytical gap in project. |
| 2026-03-24 | Cyber escalation scenarios | cascades/cyber-escalation-scenarios.md, CLAUDE.md | Full cyber warfare analysis both directions. 6 scenarios with probabilities. Fills priority gap #2. |
| 2026-03-24 | Pakistan country analysis | countries/pakistan.md | Nuclear-armed Iran neighbor; 170 warheads; Baluchistan border risk; CPEC alternative route; $38.3B remittance exposure; sectarian fragility |
| 2026-03-24 | North Korea country analysis | countries/north-korea.md | DPRK-Iran missile lineage; THAAD/Patriot redeployed from Korea to ME; Kim's optimal provocation window late 2026; $2B+ crypto theft capacity |
| 2026-03-24 | Japan country analysis | countries/japan.md | ~80% oil via Hormuz; 241-254 day SPR; four strategic paradoxes; TSMC Kumamoto; DPRK missile barrages; Sept-Oct SPR crisis point |
| 2026-03-24 | Pharmaceutical supply chains | industries/pharmaceuticals.md | 60-day inflection point (late April); China controls 70% of India's API imports; WHO Dubai hub paralyzed; antibiotics/metformin most exposed |
| 2026-03-24 | Insurance systemic risk cascade | cascades/insurance-systemic-risk.md | $1:$390 trade multiplier; Lloyd's £126B chain of security; PICC state-backed asymmetry for China; correlated losses across 8 insurance lines |
| 2026-03-24 | Migration & remittance cascade | cascades/migration-remittance-cascade.md | 30M foreign nationals in GCC; $115B annual remittances; Nepal 27% GDP exposed; 10-15x scale of 1990-91 Gulf War displacement |
| 2026-03-24 | Final resource batch | lithium.md, cobalt.md, copper.md, titanium.md, neon.md | All 5 remaining indexed resources. Key: lithium indirect-but-compounding; cobalt DRC 55% quota pre-war; copper sulphur transmission; titanium zero US sponge production; neon low direct risk but combinatorial |
| 2026-03-24 | Final industry batch | automotive.md, energy-transition.md | BYD/1973 parallel; green transition paradox quantified; nuclear = only tech both accelerated AND not China-dependent |
| 2026-03-24 | Regional analysis | africa.md, latin-america.md | Africa: 45M additional acute hunger, most harmed least consulted. LatAm: fertilizer time bomb, Q2 phase transition from buffer to contributor |
| 2026-03-24 | Final blind spots batch | 7 new cascade/resource files | Crypto (A7A5 stablecoin $100B+), space/satellite (BeiDou transition, Khayyam), info warfare (145M deepfake views), climate (El Nino 62%), domestic unrest (9 countries), health/environmental (Tehran black rain), construction materials ($350-650B reconstruction) |
| 2026-03-24 | Deep blind spots batch | 10 new files | Nuclear proliferation cascade, global financial contagion, Yemen/Houthi/Red Sea, Turkey, Central Asia, PGMs, ASEAN, war termination, Sunni-Shia, maritime chokepoints |
| 2026-03-24 | Final research files | 3 new files | Lebanon/Hezbollah (ceasefire controlled by Tehran; arsenal -85%), Ukraine interaction (revenue-expenditure inversion; Russia grand bargain offer), China-Taiwan window (coercive leverage > invasion; mediator paradox) |
| 2026-03-26 | Quality assurance pass and simulation rebuild | ~50 files across all layers | Full QA audit with sourced corrections across all intelligence layers. Simulation rebuilt with corrected inputs: Brent peak $119.50, Japan Hormuz ~80% (IEA), Tomahawk ~4,000, Shahed $30-50K (CSIS). Added Methodology & Uncertainty section, China Risks & Constraints analysis, probability methodology notes. GDP estimate: $1.2-1.8T (excl. nuclear tail). See blind-spots/red-team-audit.md for QA methodology. |
| 2026-03-26 | China Hormuz bypass analysis | cascades/china-hormuz-bypass-analysis.md, 00-cascade-index.md, CLAUDE.md | Pipeline-by-pipeline (ESPO, Kazakhstan, Myanmar, Power of Siberia), maritime (Russia Pacific, Brazil, W. Africa, Arctic NSR), SPR (1.2-1.3B bbl), demand management (1.5-3.4M bpd). 3-month: high confidence yes. 6-month: yes with pain. 12-month: possible but transformative. |
| 2026-03-27 | Communication & distribution layer | sharing/ (22 files), CLAUDE.md | Added Layer 7: public-facing assets (infographic.html, substack-article.md, youtube-script.md, podcast-script.md, press-release.md), journalist outreach templates, social media posting guides. 5 public assets committed; 17 strategy files kept local. |
| | | | |

---

## File Inventory (99 files)

### Root
- `README.md` — Public-facing project description
- `CLAUDE.md` — This file. Brain architecture and project instructions.

### `/resources/` (19 files)
- `00-resource-index.md` — Brain file: resource coverage index
- `oil-gas.md` — Oil & natural gas: 20M bpd disruption, prices, pipelines, LNG, reserves
- `helium.md` — 33% global supply offline; semiconductor fabrication dependency
- `rare-earths.md` — Chinese dominance; weapons dependency; gallium/germanium Nov 2026 deadline
- `fertilizers.md` — 1/3 of global trade via Hormuz; food crisis locked in
- `munitions.md` — 5,197 in 96 hours; cost asymmetry; production bottlenecks
- `shipping-insurance.md` — 92% traffic collapse; insurance as weapon; mine warfare
- `bromine.md` — 67% global supply at risk; Israel/Jordan Dead Sea; flame retardants for PCBs/chips
- `sulphur.md` — 24-44% production disrupted, 50% seaborne trade; copper smelting → green transition paradox
- `gallium-germanium.md` — China 99%/83% production; export ban suspension expires Nov 2026; defense/chip dependency
- `uranium.md` — Natanz struck; 440.9 kg 60% HEU stockpile; US 95% import dependency; Russia 46% enrichment dominance
- `polyethylene.md` — 84% ME exports via Hormuz; 50% global capacity offline; food packaging → spoilage cascade
- `lithium.md` — Indirect-but-compounding; China 65-75% refining; no US strategic reserve; green transition paradox
- `cobalt.md` — DRC 55% quota cut pre-war; China 78% refining; F-35 alloy dependency; LFP offset partial
- `copper.md` — Sulphur transmission mechanism; TC/RCs collapsed to $0; coiled spring post-war; green transition bottleneck #1
- `titanium.md` — Zero US sponge production; VSMPO-AVISMA halved; 1-3yr qualification; F-35 25%, F-22 42% titanium
- `neon.md` — Low direct risk; recycling halved demand; combinatorial risk with helium+bromine = 30-50% chip output cut
- `construction-materials.md` — Aluminum/steel/cement; Gulf ~5Mt aluminum; Iran 32Mt steel; reconstruction paradox $350-650B; only China can supply at scale
- `platinum-group-metals.md` — Russia 40% palladium; South Africa 70% platinum; US NDS functionally empty; hydrogen fuel cell bottleneck; sanctions trigger question

### `/countries/` (19 files)
- `00-country-index.md` — Brain file: actor coverage index
- `united-states.md` — Domestic politics, military sustainability, exit strategy
- `israel.md` — Two-front war, 93% support, strategic goals
- `iran.md` — Post-Khamenei leadership, asymmetric tools, internal fragility
- `china.md` — Resource dominance, mediation, SMIC advantage, Nov 2026 leverage
- `russia.md` — Oil windfall, Ukraine exploitation, intelligence sharing
- `india.md` — Energy vulnerability, diaspora risk, zero leverage
- `european-union.md` — Second energy crisis, divided response, autonomy failure
- `gulf-states.md` — Saudi, UAE, Qatar, Bahrain, Iraq, Egypt, Jordan (Turkey moved to own file)
- `south-korea.md` — Triple semiconductor input crisis, energy dependency, defense exports, financial market shock
- `pakistan.md` — 170 nuclear warheads; Baluchistan border; CPEC alternative route; $38.3B remittance exposure; sectarian risk
- `north-korea.md` — DPRK-Iran missile lineage; THAAD redeployed from Korea; Kim's late-2026 provocation window; $2B crypto theft
- `japan.md` — ~80% oil via Hormuz; 254-day SPR; four strategic paradoxes; TSMC Kumamoto; DPRK missile threat
- `africa.md` — 45M additional acute hunger; 90% fertilizer imports; Nigeria oil windfall; Morocco phosphate asset; Dangote refinery; most harmed, least consulted
- `latin-america.md` — Brazil fertilizer paradox; Venezuela sanctions reversal; Argentina lithium/shale boom; Chile copper; Mexico nearshoring; Q2 phase transition risk
- `turkey.md` — NATO 2nd largest military; Bosporus control; Incirlik/B61; Kurdish dimension; Bayraktar exports; Erdogan's balancing act
- `central-asia.md` — Kazakhstan #1 uranium + oil; Turkmenistan gas; INSTC collapse; corridors gatekeeper-controlled; resources captive to China
- `southeast-asia.md` — Singapore shipping hub; Indonesia nickel 50%+; Malaysia semiconductor packaging; Philippines 2.4M Gulf OFWs; China+1 manufacturing shift
- `lebanon-hezbollah.md` — Active second front; arsenal -85%; ceasefire controlled by Tehran; 1M+ displaced; Syria corridor severed; UNIFIL withdrawing

### `/industries/` (7 files)
- `00-industry-index.md` — Brain file: industry coverage index
- `semiconductors-ai.md` — Triple input crisis, memory prices, TSMC vulnerability, data center attacks
- `defense-industrial-base.md` — Munitions burn rate, production ramp, single-point failures, Ukraine competition
- `food-agriculture.md` — Fertilizer shortage, crop yield timeline, water desalination, 1B+ at risk
- `pharmaceuticals.md` — 60-day inflection point; China 70% of India API imports; WHO Dubai hub paralyzed; antibiotics/metformin most exposed
- `automotive.md` — BYD/1973 parallel; 6 simultaneous input constraints; +8-15% vehicle inflation; Japan/Korea critical exposure
- `energy-transition.md` — Green transition paradox quantified; nuclear = only tech accelerated AND not China-dependent; 2-4yr delay, 10-20yr acceleration; copper as binding constraint #1

### `/cascades/` (21 files)
- `00-cascade-index.md` — Brain file: cascade coverage index
- `china-hormuz-bypass-analysis.md` — Pipeline-by-pipeline, maritime, SPR, demand management: can China survive 3/6/12 months without Hormuz?
- `combinatorial-matrix.md` — Brain file: 5 major cascade models, meta-cascade (China)
- `november-2026-convergence.md` — Three-pressure convergence: US midterms (Nov 3) + China gallium/germanium deadline (Nov 27) + EU winter energy crisis (Dec 1)
- `water-crisis-model.md` — Desalination crisis: 100M+ at risk, 4 escalation levels, energy-water death spiral
- `cyber-escalation-scenarios.md` — Cyber warfare both directions: 6 escalation scenarios. GPS spoofing, SCADA, cloud strikes, NotPetya spillover
- `insurance-systemic-risk.md` — Lloyd's £126B chain; $1:$390 trade multiplier; PICC China asymmetry; 8 correlated insurance lines
- `migration-remittance-cascade.md` — 30M GCC foreign nationals; $115B remittances; Nepal/Pakistan most exposed; kafala system
- `cryptocurrency-alternative-finance.md` — Russia A7A5 stablecoin $100B+; DPRK $2B theft; Iran 15M crypto users; mBridge/CIPS de-dollarization; Saudi as key indicator
- `space-satellite-vulnerability.md` — Iran BeiDou transition; Khayyam satellite; GPS spoofing 1,650 vessels; ASAT risks; cable-satellite dual degradation
- `information-warfare.md` — Iran AI deepfakes 145M views; 99% internet blackout; verification collapse → policy paralysis; Iraq War comparison
- `climate-weather-compounding.md` — El Nino 62% by summer; Gulf hurricane on 56% US refining; 50C+ heat-water death spiral; monsoon risk to 800M
- `domestic-unrest-modeling.md` — 9 countries assessed; Lebanon 90-95%; Iraq 70-80%; Bahrain 65-75%; US most unpopular war at launch; Arab Spring comparison
- `health-environmental-effects.md` — Tehran black rain 9-10M exposed; 85 trapped tankers; 2026 Gulf War Syndrome; nuclear contamination; 30-year cancer timeline
- `nuclear-proliferation-cascade.md` — Saudi/Turkey/Egypt/Japan/S.Korea pathways; NPT collapse scenario; 1→5 nuclear states in decade
- `global-financial-contagion.md` — Stagflation; EM sovereign debt cascade; central bank dilemma; 1997-style contagion; IMF capacity limits
- `yemen-houthi-red-sea.md` — Double chokepoint (Hormuz+Bab el-Mandeb); Houthi escalation; Red Sea alternative negated; Saudi Petroline at Yanbu vulnerable
- `maritime-chokepoint-network.md` — Network analysis of all 6 global chokepoints; interdependencies; double/triple closure scenarios; Cape of Good Hope as sole fallback
- `sunni-shia-dynamics.md` — 200-300M Shia globally; Axis of Resistance fragmenting; Iraq as decisive battleground; Karbala narrative; proxy network status
- `ukraine-war-interaction.md` — Two-war feedback loop; revenue-expenditure inversion; munitions competition; Russia grand bargain offer; NATO fracture
- `china-taiwan-window.md` — Coercive leverage > invasion; mediator paradox; gray zone 35-45%; energy quarantine 10-15%; November convergence interaction

### `/simulation/` (8 files)
- `master-simulation.md` — Brain file: 4-phase prediction model, winners/losers
- `incentive-map.md` — Brain file: every actor's wants/fears/actions
- `war-overview.md` — Timeline of key events, day-by-day from Feb 25 to March 23
- `iran-wild-cards.md` — 7 creative asymmetric scenarios Iran could pursue
- `supply-exhaustion-analysis.md` — Can US/Israel deplete Iran's military? Analysis of conventional vs asymmetric
- `russia-china-incentives.md` — Deep analysis of what Russia and China actually want from this war
- `scenarios-and-opportunities.md` — **Brain file**: 5 scenarios with probabilities, structural shifts, economic opportunities matrix, key dates
- `war-termination-framework.md` — Ceasefire mechanics; historical precedents; reconstruction governance ($350-650B); post-war security architecture; frozen conflict risk

### `/blind-spots/` (1 file)
- `analysis.md` — Brain file: 6 categories of unmodeled risks

### `/sharing/` (22 files — 5 public, 17 private/local)
- `00-sharing-guide.md` — Brain file: rollout schedule, platform rules, checklist
- `infographic.html` — Screenshot-ready HTML cascade visualization (public, committed)
- `substack-article.md` — 1500-word narrative article (public, committed)
- `youtube-script.md` — 10-minute explainer script with visual cues (public, committed)
- `podcast-script.md` — 10-minute conversational audio script (public, committed)
- `press-release.md` — Formal press release for media outreach (public, committed)
- `linkedin-carousel.md` — 13-slide LinkedIn carousel content (private)
- `infographic-spec.md` — Canva layout spec (private)
- `journalist-pitch.md` — Email templates by beat (private)
- `journalist-emails-individual.md` — 10 personalized journalist pitches (local only)
- `niche-platforms.md` — Template reuse map for multiple communities (private)
- `event-hooks.md` — Reshare triggers when predictions come true (private)
- `[platform-specific posts]` — Twitter, Reddit, LinkedIn, HN templates (private)

---

## Missing Files (To Be Created)

**All identified research gaps have been filled.** The research phase is complete. Next step: rebuild `simulation/master-simulation.md` and `simulation/incentive-map.md` incorporating all new intelligence.
