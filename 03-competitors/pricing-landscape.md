# Pricing Landscape: AI-Native AUTOSAR BSW Delivery
*Skill: sk-competitors | Generated: 2026-10-24*

**Scope:** What Tier 1s and OEMs pay today for AUTOSAR Classic BSW configuration and integration, cybersecurity BSW integration (HSM, SecOC, secure boot, crypto stack), and ASPICE / ISO 21434 work products, and where an AI-native, Cairo-based provider can position its price.

**Read this first (evidence quality).**
- No engineering service provider (ESP) publishes rates. No AUTOSAR stack vendor publishes licence prices. No TARA tool vendor in scope publishes prices.
- Location rates below come from generic software-outsourcing rate tables (Hauer, Devico, SecondTalent, Trio, freelancermap), not automotive procurement benchmarks.
- The research budget ran out before licence, TARA-tool, ASPICE-assessment and per-ECU effort figures could be checked. Every such figure is marked **[Estimate - unverified]** and is a hypothesis to test in discovery calls. **Do not put these numbers in a pitch deck as facts.**
- Labels: **[Data]** sourced, **[Estimate]** calculated with stated assumptions, **[Assumption]** unverified belief, **[Opinion]** analyst judgment. Data older than 12 months (before 2025-10-24) is flagged **(>12 mo)**.

---

## 1. Market Pricing Overview

| Item | Finding | Label / confidence |
|---|---|---|
| **Dominant value metric** | Engineer time: hourly or daily rate, FTE-month, or dedicated-centre capacity. The market leader is moving to **fixed price per work package**. KPIT was 65.4% fixed price in FY26 and 68.3% in Q4 FY26 (59.6% a year earlier), with more than 80% of new deals fixed price. | [Data, KPIT via Multibagg, May 2026] High for KPIT, Medium for the rest of the market |
| **Price range (senior AUTOSAR engineer-hour, fully loaded)** | About USD 25/h (India, Egypt offshore) to about EUR 130/h (German onsite ESP). Roughly a 4-5x spread. | [Data + Estimate] Medium |
| **Median** | About USD 45-60/h for a blended global delivery mix | [Estimate] Low-Medium |
| **Free tier** | None. Pilots and proofs of concept are sometimes discounted or free in ESP sales. VxLabs sells a fixed-scope 6-8 week "TARA-First Pilot". | [Opinion] / [Data, vxlabs.ai] |
| **Standard discounts** | Volume and ODC (offshore development centre) commitments; up-front annual productivity give-backs of 5-10% (Gartner); Jefferies estimates 10-15% of AI productivity already shared with clients in application services. | [Data, Outlook Business, 17 Sep 2025 (>12 mo)] |
| **Buyer expectation** | Engineering buyers expect bill rates to stay flat or fall (Everest 2024 (>12 mo)). Buyers will seek "faster timelines, and outcome-based pricing" (Bain survey, n=280, published Apr 2026). | [Data] |

### 1.1 Rates by delivery location (senior embedded / AUTOSAR)

| Location | Senior rate | Who delivers from here | Source / label |
|---|---|---|---|
| Germany, freelance | EUR 85-95/h (AUTOSAR listing EUR 85/h; FuSa avg EUR 95/h) | Freelancers via GULP, Hays | [Data, freelancermap, Feb 2026] |
| Germany, ESP agency (fully loaded) | EUR 85-130/h (about EUR 700-1,000/day) | Bertrandt, Akkodis, EDAG, IAV, Vector/ETAS/EB services | [Data, Hauer Apr 2026 USD 100-140] + [Estimate] |
| Poland / Czechia | USD 55-95/h; architects USD 120+ | Capgemini Katowice, Luxoft PL, mid-size nearshore | [Data, Hauer, Devico Dec 2025, SecondTalent] |
| Romania | USD 45-75/h | Luxoft RO, Continental/Bosch captives | [Data, Hauer, Devico] |
| Ukraine / Serbia | USD 35-70/h / USD 55-85/h | Intellias (now also Cairo), Luxoft | [Data, Hauer, Devico, Bestarion (single source)] |
| India, agency | USD 25-45/h; architects USD 45-75/h. Often sold at about USD 4-7k per FTE-month | KPIT, Tata Elxsi, LTTS, HCLTech | [Data, Hauer] |
| India, tier-1 ESP blended realisation | About USD 29/h (onsite + offshore mix) | KPIT | [Estimate: FY25 USD 691M / ~13k staff / ~1,800 billable h] |
| **Egypt** | List rate USD 42-60/h (US-facing staff augmentation); automotive offshore probably **USD 25-40/h** | Avelabs/Arrow, Valeo captive, Siemens EDA, Intellias Cairo, Swift Act | [Data, Trio Apr 2026, single source] / [Estimate - unverified] for automotive |
| Morocco / Tunisia | About USD 29 / 25.5/h blended | Nearshore to FR/DE | [Data, weak: closed site, snippet only] |
| Vietnam | USD 22-40/h agency; USD 40-95/h specialist freelance | FPT and others | [Data, Hauer, SecondTalent] |
| Mexico | USD 50-90/h | Capgemini Querétaro, US-facing nearshore | [Data, Hauer, Trio, SecondTalent] |

**Automotive premium:** the sources are generic software tables. Automotive embedded skills (AUTOSAR, ASPICE, ISO 26262/21434) probably carry a +15-40% premium over these rates. [Assumption, borrowed from Hauer and Devico niche-skill uplifts]

**Data conflict:** SecondTalent puts German senior embedded engineers at USD 61-94/h, below freelancermap and Hauer. Trust freelancermap (first-party marketplace data) and Hauer for Germany. [Opinion]

### 1.2 What one ECU costs today (the comparison buyers will actually make)

| Scope | Effort | Germany (~EUR 14-21k/PM) | Eastern Europe (~EUR 7-12k/PM) | India / Egypt (~EUR 3.6-6.5k/PM) | Label |
|---|---|---|---|---|---|
| New ECU: BSW config + integration (MCAL, COM, Mem, Diag, NM, OS, RTE), first time on a platform | 12-36 PM | EUR 0.16-0.75M | EUR 0.09-0.43M | EUR 0.04-0.23M | [Estimate - unverified, medium-low] |
| + cybersecurity BSW (Crypto/CSM/CryIf/SecOC/KeyM, secure boot, HSM) | +3-9 PM | +EUR 0.04-0.19M | +EUR 0.02-0.11M | +EUR 0.01-0.06M | [Estimate - unverified, low] |
| + ASPICE work products (SWE.1-6, SUP.8-10, MAN.3) | +15-30% of engineering effort | **not** included in the totals below; add 15-30% | | | [Estimate - unverified, low] |
| **Total, new ECU incl. security (excl. ASPICE overhead)** | **15-45 PM** | **EUR 0.2-0.95M** | **EUR 0.1-0.55M** | **EUR 0.05-0.3M** | [Estimate] |
| Derivative / carry-over ECU | 3-10 PM | EUR 0.04-0.21M | EUR 0.02-0.12M | EUR 0.01-0.07M | [Estimate - unverified] |
| TARA + cybersecurity concept, one ECU (consulting) | n/a | EUR 30-150k | | | [Estimate - unverified, low] |
| Tool-assisted TARA, "representative project" | about 56 h (vs about 400 h in spreadsheets) | about EUR 6k of labour at German rates | | about EUR 2k | [Data, Aumovio case study via Ansys/Synopsys, vendor-sourced, ~Jan 2026] + [Estimate] |
| Formal ASPICE assessment (intacs, 2 assessors) | about 1 week on site | EUR 25-60k | | | [Estimate - unverified, low] |

> **Verification correction (V1, 2026-10-24).** The raw file (A2 §5) and the first version of this table used per-person-month costs of about EUR 110k (Germany), EUR 60k (Eastern Europe) and EUR 25-35k (India/Egypt), while stating the basis as "about 160 h × hourly rate from section 1". That basis gives about EUR 13.6-20.8k/PM for Germany (EUR 85-130/h), EUR 7.2-12k/PM for Eastern Europe (EUR 45-75/h) and EUR 3.6-6.5k/PM for India/Egypt (USD 25-45/h; A2 itself says "about USD 4-7k per FTE-month"). The earlier totals (EUR 1.7-5M Germany, EUR 0.9-2.7M Eastern Europe, EUR 0.4-1.6M offshore) were overstated by roughly 5-8x. The figures above are recomputed from the stated basis; effort ranges (PM) are unchanged and still unverified. See `verification-report.md`.

**[Opinion] The key point (corrected):** at market hourly rates, one integrated ECU baseline including security costs roughly EUR 0.05-0.3M offshore and EUR 0.2-0.95M in Germany, before ASPICE overhead. No published benchmark exists for these effort numbers; the founders' own project history is the source a buyer would trust most. **Document your own past-project effort data now. It is the most credible benchmark you will have.**

---

## 2. Commercial-Model Comparison

| Model | How it is priced | Who uses it | Prevalence / trend | Who carries risk | Label |
|---|---|---|---|---|---|
| **T&M / staff augmentation** (Dienstvertrag, Arbeitnehmerüberlassung) | EUR/h or day rate, monthly invoice | German ESPs, freelancers, all Indian ESPs for capacity, Akkodis | Historically dominant; KPIT still 40-50% T&M as recently as FY25 | Buyer | [Data] |
| **FTE / ODC (managed capacity, dedicated centre)** | Per FTE-month, blended team rate, annual volume commitments | Indian ESPs, Luxoft, Egyptian vendors. Tata Elxsi EUR 50M (Apr 2025 (>12 mo)) and LTTS EUR 50M (Mar 2025 (>12 mo)) deals both include a dedicated centre | Common for multi-year SDV programmes | Shared | [Data] |
| **Fixed-price work package** (Werkvertrag) | Per milestone or deliverable | KPIT (65-68% of revenue); others unknown | Rising fast. German labour-hire law (AÜG 2017) pushes offshore work toward outcome-defined Werkvertrag | Vendor | [Data] |
| **Outcome-based** | Tied to KPIs (cost reduction, defects, cycle time) | KPIT is converting large T&M accounts; Q1 FY27 headline "engaging clients on 30-40% cost reduction" (context unverified); TechM, TCS, Coforge in IT | Emerging | Vendor | [Data, headline only for the 30-40%] |
| **Per-ECU productised price list** | Fixed fee per ECU configuration or integration, published | **Nobody publishes one.** Stack vendors sell "integration packages" on quote | Rare, opaque | Vendor | [Opinion] |
| **Stack licence + services bundle** | Module-set licence per project, configurator seats, volume or runtime royalties, plus vendor integration days | Vector (quote per module set; predefined packages with updates "without lead time and additional costs"), EB (upfront or volume-based; global concept licences), ETAS ("greatly reduced runtime license costs", which confirms per-unit royalties exist) | Universal for the stack layer | Buyer (licence), shared (services) | [Data, models only]; amounts DATA GAP. Hearsay: full BSW + security stack for one ECU project = low-to-mid six figures EUR [Estimate - unverified, low] |
| **AI feature subscription in the stack tool** | Vector DaVinci AI requires an "AI-enabled" licence plus Embedded Hub account; customer supplies its own LLM endpoint; **subscription-only from July 2027** | Vector | New (2026); EB's "integration-as-code" is described as groundwork for "future AI-assisted configuration" | Buyer | [Data, Vector help pages 2026]; price DATA GAP |
| **TARA / cybersecurity tool licence** | Named or floating seat per year, or enterprise platform | itemis SECURE, Ansys/Synopsys medini, Cybellum, C2A EVSec, VxLabs ThreatZ (also on AWS Marketplace), Saphira, Ketryx | Common | Buyer | Model [Data]; amounts below are [Estimate - unverified, low] |

### 2.1 AI TARA / compliance tool pricing (what is known)

| Tool | Pricing model | Indicative price | AI claim | Label |
|---|---|---|---|---|
| itemis SECURE | Seat licence (assumed) | about EUR 10-30k per seat per year | "up to 80%" TARA effort reduction | Price [Estimate - unverified, low]; claim [Data, snippet] |
| Ansys/Synopsys medini analyze | Seat licence + consulting | similar seat range | Aumovio case: 400 h to 56 h | Price [Estimate - unverified, low]; case [Data, vendor] |
| Cybellum (LG) | Enterprise platform | about USD 100k+/yr at OEM scale | None found | [Estimate - unverified, low] |
| VxLabs ThreatZ | Platform + fixed-scope 6-8 week TARA-First Pilot; AWS Marketplace listing | DATA GAP | "up to 85%" faster than spreadsheets | [Data, vendor claim] |
| C2A EVSec / AutoSynth | Platform | DATA GAP | TARA "75% faster" | [Data, vendor claim] |
| Saphira AI | SaaS (assumed) | DATA GAP | "~70% less hands-on documentation effort" | [Data, vendor claim] |
| Ketryx | SaaS compliance platform | DATA GAP | "Cuts documentation time by 90%" | [Data, vendor claim; no automotive logos] |
| Open source (AutoTARA GitHub, AutoSecGPT) | Free | EUR 0 | n/a | [Data] |

**[Opinion] Implication:** TARA and 21434 documentation is being priced as software (a seat or platform fee) with claimed 70-90% effort cuts. A labour-priced "21434 work products" offer with no implementation attached will be benchmarked against a tool-assisted TARA of about 56 hours. That is a price war the founders should not enter. Bundle the documentation with on-target implementation.

---

## 3. Value Metric Analysis

| Competitor | Value metric | Why it works / doesn't | Impact as the buyer scales |
|---|---|---|---|
| **KPIT** | Fixed price per work package; outcome-based for large accounts | Works for KPIT: AI productivity becomes margin ("productivity gains ... support margin expansion" [Data, Q1 FY27]). Buyer sees a fixed number but not the saving. | Cost grows per programme, not per head. Buyer cannot see whether AI savings were passed through. |
| **Tata Elxsi** | T&M + dedicated centres; fixed-price share not retrieved | Familiar, low-risk for procurement. Conflicts with any "half the cost" promise because revenue is tied to billed effort. | Linear with headcount. |
| **LTTS, Luxoft, Capgemini, HCLTech** | T&M, FTE/ODC, framework agreements | Proven, easy to buy; nearshore (PL, RO, MX) for proximity. | Linear with headcount. |
| **Akkodis, Bertrandt** | Staff augmentation day rates | Fast to staff; exposed to AI deflation and AÜG legal risk in Germany. | Linear; most exposed to rate pressure. |
| **Vector / EB / ETAS (services)** | Licence (per module set, seat, unit royalty) + integration days + AI subscription (Vector, from Jul 2027) | Strongest metric in the market: services pull through licences, and the licence creates the switching cost. | Cost grows with ECU count, production volume (royalties) and seats. |
| **AI TARA tools** | Seat or platform per year | Predictable; buyer still needs engineers to use it and to implement controls. | Grows with seats and programmes. |
| **Avelabs/Arrow, Egyptian ESPs** | T&M / FTE (assumed) | Cairo cost; Arrow can bundle with chip sales. | Linear with headcount. [Assumption] |
| **Tier 1 in-house + AI tools** | Salaries + tool seats (Copilot/Devin/Vector AI subscription) | Sunk cost, no procurement cycle, IP stays inside. | Fixed cost; hard to flex for peaks. |
| **Founders (proposed)** | **Fixed price per ECU scope (new / derivative), evidence included** | Matches the deliverable the buyer actually wants; fits Werkvertrag; makes AI savings visible. Risk: estimation error falls on a 2-person firm. | Grows per ECU and per variant, not per head. Enables a variant subscription. |

---

## 4. Pricing Psychology in Use

| Tactic | Used by | How | Label |
|---|---|---|---|
| **Opacity / quote-only** | Every ESP and every stack vendor | No public prices; licensing "can be discussed in parallel to ECU development" (Vector). Keeps comparison hard and favours incumbents. | [Data] |
| **Percentage anchoring** | Luxoft/DXC AMBER ("up to 50% faster", "30% lower cost"); EB ("up to 50% savings via licensing", "up to 30% lower BSW cost when migrating"); Neusoft (30-50%); TARA tools (70-90%) | Vague "up to" claims with no method. Buyers now discount them. Surveyed/reported AI gains are 10-19% (Capgemini survey Oct 2026; Bain 2025). | [Data, vendor claims] |
| **Bundling** | Vector, EB, ETAS | Licence + first-line support + integration days. Makes vendor services look "free" or low-risk next to a third party. | [Data, model] |
| **Low-risk pilot / land-and-expand** | VxLabs (6-8 week TARA-First Pilot); ESPs (discounted PoCs) | Fixed-scope pilot to get on the account, then expand. | [Data] / [Opinion] |
| **Productivity give-back commitments** | Indian IT / ER&D broadly | Commit up front to 5-10% annual cost reductions. | [Data, Gartner via Outlook Business, Sep 2025 (>12 mo)] |
| **Subscription lock-in** | Vector (AI subscription-only from July 2027); EB global concept licences | Moves AI value into recurring licence revenue. | [Data] |
| **Volume / capacity commitment** | Indian ESPs, ODC deals | Lower blended rate in exchange for multi-year headcount commitment. | [Data] |
| **Analyst badges as price justification** | Capgemini, HCLTech, Akkodis, LTTS (Everest, ISG, Zinnov "Leader") | Supports premium and procurement comfort. | [Data] |

---

## 5. Price Positioning Map

Y-axis: effective price per integrated, evidenced ECU baseline (relative, not absolute). X-axis: depth of BSW + security integration and assurance (on-target verification, assessor-ready evidence, accountability). Positions are **[Opinion]**, based on the raw profiles.

```
 PRICE (per evidenced ECU)
  High |  [German ESPs:              [Vector services]   [ETAS/ESCRYPT
       |   Bertrandt, Akkodis,                          services]
       |   freelancers]
       |                                 [Capgemini Eng.]
       |         [Luxoft]                 [Elektrobit services]
   Mid |                  [LTTS]
       |                       [Tata Elxsi]     [KPIT fixed-price]
       |    [AI TARA tools:            [Avelabs/Arrow]
       |     seat licence,
       |     docs only]      [Tier 1 in-house + Copilot/Vector AI]
   Low |  [Open-source TARA]                          * TARGET:
       |                                                founders' fixed-price,
       |                                                cross-vendor, on-target
       |                                                security BSW + evidence
       +------------------------------------------------------------------>
         Docs / capacity only      Integration labour      Verified on target +
                                                           assessor-ready evidence
                         DEPTH / ASSURANCE
```

**Reading the map [Opinion]:**
- The bottom-right corner (low price, high assurance) is empty. Everyone with deep assurance (Vector, ETAS/ESCRYPT, KPIT) is mid-to-high price. Everyone cheap (AI TARA tools, open source, in-house plus Copilot) stops at documents or lacks accountable evidence.
- KPIT and Avelabs/Arrow are the nearest neighbours to the target. KPIT has the depth and is moving down in price through fixed price and AI. Avelabs has the price and the skills but no visible AI or evidence product.
- **The target position is only credible with proof** (published accuracy metrics, a passed assessment, a named reference). Without it, the founders plot at bottom-left, next to the tools.

---

## 6. Switching Cost Matrix

Rating H/M/L = how hard it is for a buyer to move work **from** this competitor **to** the founders. "Supplier qualification" = the founders' own burden to get onto the buyer's approved list in place of this competitor.

| Competitor | Technical | Contractual | Relationship | Supplier qualification (founders' gap) | Overall | Where to attack |
|---|---|---|---|---|---|---|
| **Vector (services + AI)** | **H**: configuration lives in DaVinci; BSWMD, validators and generators are Vector's; AI agents run inside the tool | **H**: multi-year licence and maintenance; AI subscription from Jul 2027 | **H**: "call Vector" default for MICROSAR security | **H**: Vector is already listed; founders need TISAX, ASPICE evidence, CEEP | **Very high** | Do not displace. Work on the customer's Vector licence as a certified partner; take cross-vendor and HSM-firmware glue work. |
| **Elektrobit** | H (tresos; MCAL plugins often unavoidable) | H (global concept licences) | M-H | H | **High** | Mixed-stack projects (EB MCAL inside Vector/ETAS BSW). |
| **ETAS / ESCRYPT** | H for CycurHSM firmware itself; M for integration around it | H | H (Bosch captive; ESCRYPT brand) | H | **High** | Integration of CycurHSM into non-ETAS BSW; cost. |
| **KPIT** | M (knowledge in people; handover cost) | **H** (MSAs, multi-year fixed-price programmes lock scope) | H (BMW, Honda, Renault; T25 = ~82-88% of revenue) | H | **High** on running programmes, **Medium** on new ECU starts | New ECU starts and derivatives outside a running KPIT programme; small and mid-size Tier 1s below KPIT's deal threshold. |
| **Tata Elxsi** | M | H (multi-year centres, e.g. EUR 50M deal) | M-H | H | **High / Medium** | Security BSW scope that DevStudio.ai does not cover. |
| **LTTS** | M | H (EUR 50M centre deal, NA MSAs) | M | H | **Medium-High** | NA Tier 1s needing Classic security BSW (LTTS messaging is ADAS-centric). |
| **Luxoft (DXC)** | M | M (framework agreements) | M | M-H | **Medium** | BSW security work at accounts where Luxoft is cockpit-focused. **Check Waled's Luxoft non-solicitation clause first.** |
| **Avelabs / Arrow** | M | M | M-H (Munich, Detroit front offices; Arrow chip relationships) | H (founders unlisted) | **Medium-High** | AI-measured fixed price; but **non-solicitation clauses may bar the founders from Avelabs' customers.** Legal review first. |
| **German ESPs / freelancers** | L-M | M (framework) / L (freelancers) | H (proximity, language) / L-M | M (via subcontracting, the prime carries the listing) | **Medium / Low** | Easiest displacement; also the best **subcontracting** channel (Bertrandt is moving work to low-cost countries). |
| **AI TARA tools** (ThreatZ, C2A, medini, itemis) | M (TARA models, knowledge graph) | M (annual seats) | L-M | L (founders are not replacing the tool) | **Medium** | Do not replace the tool. Consume its TARA output and implement the controls. |
| **Tier 1 in-house (+ AI agents)** | L technically | n/a | **Very H** politically (internal teams defend headcount) | n/a | **High** | Overflow, peaks, rescues, and skills the team lacks (HSM/secure boot). Never pitch "replace your team". |

Sources: pricing-intelligence §6, competitor-profiles, gtm-analysis §3, tech-stack-analysis §1. All ratings [Opinion].

**Founders' own new switching friction [Opinion]:** buyers will ask about IP and data residency for LLM use on OEM code, GDPR third-country transfer to Egypt (Egypt has no EU adequacy decision [Assumption]), liability caps, insurance and continuity of a two-person firm. Incumbents do not face these questions. Price must compensate for this added perceived risk, or a guarantee must neutralise it.

---

## 7. Pricing Whitespace

**One line:** No one sells a **published, fixed-price, per-ECU cybersecurity BSW integration package** (HSM, SecOC, secure boot, crypto stack on named MCUs, across Vector/ETAS/EB stacks), **verified on target, with assessor-ready ASPICE/21434 evidence included and published accuracy metrics**. ESPs sell hours or bespoke fixed-price programmes; stack vendors sell licences, single-stack services and AI subscriptions; TARA tools sell seats that stop at documents. [Opinion, based on absence across all 9 raw files]

Specific open spaces, ranked by fit with niche I and wedge H [Opinion]:

1. **Per-ECU security integration package with a public price band.** No one publishes. Transparency helps in procurement-led buying and makes the AI saving visible.
2. **Evidence-inclusive pricing with a guarantee.** The price includes the ASPICE/21434 work-product set for the scope, with "assessment findings on our scope fixed at our cost". Incumbents bill documentation as extra effort.
3. **Productivity pass-through, committed up front.** For example, each derivative ECU priced 20% below the previous one. This answers the Bain/Everest buyer expectation that incumbents (KPIT) are deliberately not meeting.
4. **Derivative / variant subscription.** A recurring fee per ECU variant for re-configuration when the stack, MCAL, keys or requirements change. Turns projects into recurring revenue, which investors value (AI-native services above 3x revenue vs 1-2x for traditional services [Data, Livingstone 2026, partly Assumption]).
5. **Overflow capacity for captives at fixed price.** Avoids the political cost of "replacing" internal teams.
6. **Agent-enablement packs** (skills + MCP integrations + training) for Tier 1s that want to DIY with Vector's MCP and Claude Code/Copilot. Prices the DIY threat instead of fighting it.

**Not whitespace:** "AI-native" (KPIT, Tata Elxsi, PopcornSAR, Neusoft, AVIN, SRM Tech all claim it); fixed price as such (KPIT 65.4% in FY26, 68.3% in Q4 FY26); AI TARA documents (at least 6 commercial tools plus open source); "AI configures BSW" (Vector DaVinci 6.4/6.5, AutoC).

---

## 8. Recommendations for the Founders

> **PRICES TO BE SET IN OFFER (Phase 5) AND MONEY (Phase 7).** Founder decision, 2026-10-24: every price hypothesis below is a placeholder. It will be re-derived from the founders' own effort data (person-months per ECU for BSW integration, cybersecurity and ASPICE work), and the "half the cost" baseline will be stated explicitly.

### 8.1 State the baseline for "half the cost" (mandatory)

"Half the cost" is ambiguous and a buyer's first question will be "half of what?". Procurement will benchmark against India. [Opinion]

| Baseline | Is "half" credible? | What it requires | Verdict |
|---|---|---|---|
| German onsite ESP / freelancers (EUR 85-130/h) | Trivially. Romania already achieves it with no AI. | Nothing AI-specific | **True but meaningless.** Do not lead with it. |
| Eastern European nearshore (USD 45-95/h) | Plausible | About 1.2-1.6x productivity at Cairo cost | Credible for German Tier 1s with nearshore suppliers. [Estimate] |
| Indian / Egyptian offshore T&M (USD 25-45/h) | Hard | **About 2.5-3x productivity** at Cairo cost levels, net of human checkpoint time, tooling and LLM cost | **Unproven. No public evidence for this on security BSW.** Surveyed/reported AI gains are 10-19%. [Estimate + Data] |
| Buyer's own last comparable ECU (internal cost or past ESP invoice) | Depends | A measured pilot | **The only baseline a buyer cannot dispute.** |

**Recommended phrasing [Opinion]:**
- Headline: *"ASPICE-ready AUTOSAR security integration at a fixed price per ECU, at or below what you pay an offshore team on time-and-materials, delivered in half the calendar time."*
- Proof line (after a pilot): *"On [reference ECU], we delivered [scope] in [X] weeks for EUR [Y], [Z]% below the customer's previous cost for the same scope, with zero ASPICE findings on our work products."*
- If "half the cost" stays in the pitch, always attach the baseline: *"half the cost of a German or nearshore ESP for the same ECU scope"* or *"half your last comparable project's cost, measured in a paid pilot"*. Never say "half the cost" unqualified to a buyer who uses Indian ESPs.
- Lead with **time** (calendar weeks to an integrated, evidenced baseline), which is easier to prove than cost against India, and is what release-crunch buyers feel. [Opinion]

### 8.2 If competing on price
- Do **not** compete on hourly rate. Egypt's automotive offshore rate (about USD 25-40/h) is roughly India's. A rate war against KPIT, Avelabs and Valeo's captive is lost on scale. [Opinion]
- Price per ECU scope instead. Working hypotheses to test in 10-15 discovery calls [Estimate - unverified, derived from §1.2]:
  - **Security BSW package (wedge H), one ECU, one MCU family** (Crypto/CSM/CryIf/KeyM, SecOC, secure boot, HSM integration, 21434 work products for that scope): **EUR 60-150k**. Original logic: "3-9 PM at India/Egypt loaded cost = EUR 75-315k; a price at about half of that is the 'half the cost vs offshore' claim made concrete." **V1 correction:** at the corrected India/Egypt cost (EUR 3.6-6.5k/PM) 3-9 PM is about EUR 11-60k, and at German cost about EUR 40-190k. EUR 60-150k is therefore at or above offshore T&M cost and roughly at German cost, not half of offshore. **Founders must re-derive this hypothesis.**
  - **Derivative security package:** **EUR 25-60k**.
  - **Full new-ECU BSW + security baseline (niche I):** **EUR 250-600k**; derivative **EUR 80-200k** (A2's hypothesis). A2 said this "lands at or below India T&M equivalent". **V1 correction:** with the corrected §1.2 figures it does not. India/Egypt T&M for 15-45 PM is about EUR 0.05-0.3M and Germany about EUR 0.2-0.95M, so EUR 250-600k sits above offshore cost and inside the German range. **Founders must re-derive this hypothesis.**
  - Every number above must be checked against the founders' own past-project effort before use.
- Margin check: at these prices a 2.5-3x productivity gain is needed to keep healthy gross margin against Cairo salaries. If the pilot shows only 1.3-1.5x, the price floor moves up toward the India T&M band, and the value story must shift to speed and evidence. [Estimate]

### 8.3 If competing on value
- Sell **assurance, not hours**: on-target verification (secure boot works, SecOC MACs verified on the bus, keys provisioned), cross-vendor glue, and work products an assessor accepts. These are what KPIT, Tata Elxsi and the TARA tools do not visibly offer for security BSW. [Opinion]
- **Publish accuracy metrics** from an internal benchmark (50-100 BSW and security configuration tasks with deterministic acceptance checks). No competitor publishes any. [Opinion, from tech-stack-analysis §6.3]
- Attach a guarantee (fix ASPICE/21434 findings on our scope free; fixed delivery date or price reduction). This turns the founders' biggest weakness (unknown two-person firm) into a risk-transfer argument. [Opinion]

### 8.4 If competing on model
- **Fixed price per ECU with visible pass-through:** publish a price band and commit up front that each derivative is cheaper. This directly contrasts with KPIT's "AI goes to margin". [Opinion]
- **Variant subscription** after the first ECU, for recurring revenue and a better valuation story when raising. [Opinion]
- **Subcontract first.** Sell the same fixed-price package to cost-pressured primes (Bertrandt, mid-size German ESPs, possibly eInfochips). They carry TISAX and supplier listing for 6-18 months while the founders build evidence. Accept lower margin and less visibility as the price of speed. [Opinion, from gtm-analysis]
- **Do not sell the stack or AI tooling.** Work on the customer's Vector/ETAS/EB licences (including Vector's AI subscription if the customer owns it). Confirm third-party and AI-use licence terms before quoting (Gate 0). [Opinion]

### 8.5 What to validate before setting a price
1. Founders' own effort history for 3-5 past security BSW integrations (hours by module, defects, calendar time).
2. What 5+ Tier 1 buyers paid for their last security integration, and through which model.
3. Vector/ETAS/EB terms on third-party and AI use of customer licences; price of Vector's AI subscription.
4. Whether buyers will accept a Cairo provider's AI-assisted work products (assessor and infosec view).
5. TARA tool seat prices (itemis, medini, ThreatZ) to size what the documentation half is worth.

---

## Data Gaps
*Collected from the evidence-quality notes and DATA GAP cells above (added by V1). Root cause: the shared web-search budget ran out and cut every research agent short.*
- No ESP publishes rates; location rates come from generic software rate tables, not automotive procurement data.
- Vector, EB and ETAS licence prices, Vector's AI subscription price, and third-party / AI-use licence terms.
- TARA-tool prices (itemis, medini, ThreatZ, C2A, Saphira, Ketryx, Cybellum).
- Real BSW effort per ECU (person-months); every §1.2 effort figure is unverified.
- Egypt automotive billing rates (one generic source; Payscale implausible).
- Tata Elxsi, LTTS, Luxoft and Avelabs fixed-price shares; ETAS cybersecurity service pricing.
- Willingness to pay for a per-ECU security package (no buyer interviews yet).

## Red Flags
- **"Half the cost" is meaningless or unproven depending on baseline.** Against German rates it needs no AI; against Indian/Egyptian offshore rates it needs about 2.5-3x productivity, while surveyed/reported AI gains are 10-19%. Purchasing will benchmark against India. [Estimate + Data]
- **KPIT already sells AI-infused, fixed-price, cost-reduction delivery** (68.3% fixed price in Q4 FY26, 65.4% for FY26; >80% of new deals; "30-40% cost reduction" engagements, headline unverified) to the same buyers. "AI + fixed price" is not whitespace; only transparent per-ECU packaging, pass-through and security depth may be. [Data + Opinion]
- **Almost every licence, tool, per-ECU and assessment figure here is unverified.** A pricing model built on them without the founders' own effort data and buyer interviews could be wrong by 2x either way. [Data quality] V1 found the per-ECU cost table had already been overstated about 5-8x by an arithmetic error (corrected in §1.2); the EUR 60-150k and EUR 250-600k price hypotheses have not yet been re-derived.
- **Fixed price shifts estimation risk to a two-person firm.** One badly scoped ECU with unfamiliar HSM firmware could consume months of runway. [Opinion]

## Yellow Flags
- Vector's AI subscription (from July 2027) may become a line item the buyer weighs against a service fee: "why pay you if DaVinci's agent does it?". Watch the subscription price. [Data + Opinion]
- AI TARA tools claim 70-90% effort cuts and open-source alternatives exist; the documentation half of the wedge is deflating fast. [Data]
- Incumbents under revenue pressure (KPIT Q1 FY27 -0.6% USD; Tata Elxsi profit declines 2025; Bertrandt -18% revenue) may cut rates aggressively to defend accounts. [Data]
- Egypt rate data is thin and contradictory (Payscale salary floor implausibly low vs Trio list rates); Valeo's ~2,200 Cairo engineers set talent prices. [Data]
- Supplier-qualification costs (TISAX, ISO 27001-aligned ISMS, insurance) and the 6-18 month gap before direct Tier 1 revenue are not priced into any of the above. [Estimate]
- Several sources are older than 12 months (Everest 2024, Jefferies/Gartner Sep 2025, Tata Elxsi and LTTS EUR 50M deals Apr/Mar 2025, ST/ARCCORE 2018).

## Sources
Raw files (all 2026-10-24): `raw/pricing-intelligence.md` (A2), `raw/competitor-profiles.md` (A1), `raw/adjacent-competitors.md` (A3), `raw/tech-stack-analysis.md` (C3), `raw/gtm-analysis.md` (C1), `raw/strategic-signals.md` (C2), `raw/review-mining.md` (B1), `raw/social-sentiment.md` (B3), `raw/forum-mining.md` (B2); `02-niches.md`.

Key underlying sources (as cited in raw files):
- freelancermap, Ingenieur Stundensatz 2026 (9 Feb 2026): https://www.freelancermap.de/blog/?p=68600 ; AUTOSAR listing: https://www.freelancermap.de/projekt/embedded-developer-autosar-euro85-p-h
- Hauer, Nearshore rates 2026 (Apr 2026): https://www.hauerpower.com/en/insights-posts/nearshore-software-development-rates-2026
- Devico, Eastern Europe rates (23 Dec 2025): https://devico.io/blog/software-development-rates-in-eastern-europe-2025-breakdown-by-country
- SecondTalent, embedded engineer cost (Sep 2026): https://www.secondtalent.com/cost-to-hire/embedded-software-engineer/
- Trio, nearshore rates (21 Apr 2026): https://trio.dev/nearshore-software-development-rates/
- Multibagg, KPIT Q4 FY26 (6 May 2026): https://www.multibagg.ai/market-pulse/articles/kpit-q4-93399
- CompoundingAI, KPIT Q1 FY27 call headline (Jul 2026): https://compoundingai.in/market-news/kpittech-q1-fy27-earnings-call
- Outlook Business, AI and outcome-based deals (17 Sep 2025, >12 mo): https://www.outlookbusiness.com/in-depth/ai-pushes-it-services-to-outcome-based-deals-as-clients-demand-results
- Everest Group engineering services CXO brochure (2024, >12 mo): https://www2.everestgrp.com/Libraries/reports/Products/EGR-2024-75-R-6311/MarketingBrochure
- Vector licensing / AI assistant: https://help.vector.com/DaVinci-Package-Manager/current/en/Help/html/custom_package_vs_package_based_delivery.html ; https://help.vector.com/davinci-configurator-classic/en/latest/user-manual/ui-client/views/ai-agent-view.html
- Elektrobit licensing / HL Mando: https://elektrobit.com/?p=27049 ; https://www.elektrobit.com/?p=46314
- ETAS RTA runtime licences: https://www.electronicspecifier.com/?p=135666
- Aumovio TARA case study (vendor, ~Jan 2026): https://ansys.synopsys.com/resource-center/case-study/aumovio
- VxLabs/ThreatZ: https://vxlabs.ai/ ; C2A: https://c2a-sec.com/evsec/ ; Saphira: https://www.saphira.ai/blog/aiaccelerated-iso-21434-cybersecurity-for-automotive-semiconductors ; Ketryx: https://www.ketryx.com/industries/automotive
- Capgemini Research Institute agentic AI survey (12 Oct 2026): https://www.capgemini.com/news/press-releases/68-of-automotive-organizations-use-or-pilot-agentic-ai-for-product-development-but-only-5-report-mature-ai-governance-2/
- Bain, GenAI in software development 2025: https://www.bain.com/insights/from-pilots-to-payoff-generative-ai-in-software-development-technology-report-2025/
- Livingstone 2026 IT services update: https://livingstonepartners.com/wp-content/uploads/2026/08/Livingstone-2026-IT-Services-Market-Update.pdf
- AÜG / sham works contracts: https://www.roedl.com/insights/vorsicht-bei-scheinwerkvertraegen/
