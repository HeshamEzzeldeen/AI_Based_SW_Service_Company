# Market Category Analysis: AI-native AUTOSAR BSW / Secure ECU delivery (Agent B1)
*Generated: 2026-10-25*
Status: COMPLETE. Rounds 1-4 done. 20 of 25 web calls used (19 searches + 1 fetch).

*Inputs: `_agent-brief.md`; `03-competitors.md`; `03-competitors/competitive-matrix.md`; Phase 3 raw files (review-mining, competitor-profiles, strategic-signals, pricing-intelligence) for analyst and sizing facts already found. Wave 1 is running in parallel, so competitive alternatives come from Phase 3. Labels: [Data] / [Estimate] / [Opinion], with confidence H/M/L. Raw search notes with URLs are in the appendix.*

---

## How Competitors Frame Themselves

| Competitor | Self-described category | Tagline / framing | Analyst / directory category |
|---|---|---|---|
| KPIT | "Software integration partner" to mobility | "Largest Independent Software and System Integration Partner to the Mobility Ecosystem"; at CES 2026 it launched a "Mobility Agentic AI suite" for SW development, testing and integration [Data, M-H] | ER&D / mobility software; not on Everest's public SDV list [Data, M] |
| Tata Elxsi | ER&D / design-led technology services; "SDV" partner | DevStudio.ai: "multi-agent, ASPICE-aligned GenAI platform" (Mar 2026) [Data, H] | Gartner Peer Insights: "R&D Outsourcing Services" [Data, H] |
| LTTS | "Global leader in AI, digital and ER&D consulting" (Jan 2026) | Investor deck: "shift to outcome-based, risk-sharing models" (Aug 2026) [Data, H] | Everest SDV Engineering Services PEAK 2025 (listed); HFS ER&D assessments [Data, H] |
| Capgemini Engineering, Akkodis, Luxoft, Bertrandt | Global ER&D / "SDV engineering" | "Leader" badges: Everest SDV PEAK, ISG Digital Engineering, Zinnov Zones Automotive ER&D [Data, H, Phase 3] | Same analyst frames |
| Vector / Elektrobit / ETAS | Software products (stack, tools) plus services | Vector: AI assistant and agentic EcuC-as-Code; EB: SecOC + EB zentur HSM firmware; ETAS: CycurHSM (NIST CAVP) [Data, H] | Analysts do not cover them as services firms |
| AI-TARA tools (ThreatZ, C2A, Ketryx, Saphira, AutoTARA, VxLabs) | "AI-powered automotive cybersecurity and embedded software platforms" (VxLabs) [Data, Phase 3] | 70-90% TARA time savings (unaudited) | Software / compliance tooling; no G2/Capterra category found |
| Security consultancies (SwRI, UL, VVDN, FESCARO) | "Automotive cybersecurity engineering / consulting" | FESCARO (Infineon partner page): "all-in-one" consulting + TARA + **HSM solution + engineering + testing** [Data, M] | None |

**What this shows [Opinion, M-H]:**
- Every large ESP frames itself under the broad ER&D / SDV umbrella and uses analyst "Leader" badges as proof.
- "Agentic AI" is already incumbent vocabulary in automotive (KPIT suite, Tata Elxsi DevStudio.ai, HCLTech "Agentic AI for ADAS"), so "AI-native ESP" will not stand out.
- Nobody frames itself as "security BSW integration" or "Secure ECU integration" services. That work sits inside stack vendors' product-plus-services offers, with FESCARO the nearest services-led exception. FESCARO is a NEW competitor not covered in Phase 3; Wave 1 should profile it.
- G2/Capterra are irrelevant here: no category exists for ESPs. The only directory category found is Gartner Peer Insights "R&D Outsourcing Services".

## How analysts frame the space
- **Zinnov:** "Zinnov Zones ER&D" and "Automotive ER&D" ratings (about 60 providers rated). Last public sizing: automotive ER&D spend of ~USD 158B (2019, FLAG: 6+ years old) [Data, L for currency].
- **Everest Group:** "SDV Engineering Services PEAK Matrix 2025" (28 providers) and "Software Product Engineering Services PEAK 2026". In the 2026 report, buyers want partners that "industrialize AI across the SDLC" with "measurable outcomes on cost, speed, and innovation". Everest also publishes on the "shift from effort to value" in engineering services [Data, M; TCS-licensed copy, Apr 2026].
- **ISG:** "Digital Engineering" quadrants [Data, H, Phase 3].
- **HFS:** coined and trademarked "Services-as-Software" (2024). It forecasts a "$1.5 trillion+ SaS market" by 2035, while traditional technology services shrink at −3 to −5% CAGR [Estimate by HFS, M]. In its 2026 survey, 54% of services are bought on effort; buyers prefer "base fee + outcome kicker" (56%) [Data, M; n=101-605]. HFS also runs "Agentic Services Horizons 2026" and assesses ER&D providers. DATA GAP: HFS has not applied SaS specifically to ER&D in public material.
- **The analysts' lens rewards scale, footprint, CoEs and IP accelerators** [Data, Phase 3]. No analyst has a security-BSW or ECU-integration subcategory [Data: absence, M].

## How buyers search and issue RFQs
- **Not via search engines or review sites.** Tier 1s source ER&D through preferred-supplier panels and framework agreements (Akkodis, Bertrandt), then issue private work-package RFQs on supplier portals. No public RFQ documents were found [Data: absence, M]. DATA GAP: the actual RFQ structure (RFI → RFQ → nomination) at named Tier 1s; fill with 3-5 discovery calls with purchasing.
- **In Germany, BSW integration is bought as a "Werkvertrag" (contract for a defined work result) or as freelancer/ANÜ (temporary agency staffing) capacity.** Real postings scope the work as "Integration, Configuration and Test of generic SW modules ... hardware-independent parts of AUTOSAR Basic SW" (freelancermap, Bayern) and require MICROSAR/Vector experience [Data, M]. A Werkvertrag maps naturally onto a fixed-price package.
- **Buyer vocabulary (job posts and freelance projects):** "AUTOSAR BSW integration", "AUTOSAR config & integration", "Classic AUTOSAR with Crypto Service Manager" (Harman), "AUTOSAR Cybersecurity Lead", "HSM firmware", "secure boot", "SecOC", "TARA", "R155/R156" [Data, M].
- **"Secure ECU" is a vendor/marketing term,** not a sourcing line item [Opinion, M]. A buyer would recognise it, but the RFQ will name the modules (Csm/CryIf/SecOC/KeyM/HSM).

---

## Candidate Categories

### Category 1: Automotive Engineering R&D (ER&D) services / ESP
- **Type:** Existing (head-to-head).
- **Buyer expectations:** scale and ramp-up capacity; TISAX; ASPICE CL2/3 track record; a place on the supplier panel; OEM references; T&M or FTE pricing increasingly moving to fixed price; end-to-end SDV coverage; global or nearshore delivery; now also "AI productivity".
- **Current leaders:** KPIT, Tata Elxsi, LTTS, Capgemini Engineering, Akkodis, Luxoft, Bertrandt, HCLTech, Tata Technologies [Data, H].
- **Competitive density:** High (about 12 global/Indian ESPs and 28 in Everest's SDV matrix, plus local benches).
- **Growth:** Growing long-term, cyclical short-term.
  - IMARC: USD 150.7B (2025) to USD 503B (2034), 14.3% CAGR [Data, L-M; broad definition, syndicated].
  - Everest: total automotive engineering spend USD 240-260B, of which USD 75-80B is SDV [Data, M, Feb 2026].
  - BCG/NASSCOM: about USD 500B auto ER&D by 2030, 8-9% CAGR (spend, not outsourced) [Data, M, 2024; FLAG: >12 months].
  - Short term: KPIT puts the 2025 global decline at 24-25%; Bertrandt −18% [Data, H, Phase 3].
  - The definitions differ widely, so use the figures only as order-of-magnitude.
- **Pros:** the category is instantly understood, and procurement already has a sourcing process and budget line for it.
- **Cons:**
  - The founders are Missing on every table stake (qualification, references, scale).
  - KPIT already sells AI + fixed price.
  - The frame invites a rate-card comparison with India (USD 25-45/h).
  - Investors value it at services multiples.
- **Dunford fit:** **No.** The frame hides all six strengths. "Cross-vendor", "on-target verified" and "evidence included" are what every ESP claims, and the founders look like a two-person ESP with no references.

### Category 2: AUTOSAR Classic BSW integration services
- **Type:** Subcategory of ER&D.
- **Buyer expectations:** deep MICROSAR / EB tresos / ETAS RTA-CAR knowledge, MCAL experience, fast bring-up, a working build on target, and engineers who can sit in the customer's toolchain.
- **Current leaders:**
  - The stack vendors' own engineering services (Vector, EB, ETAS).
  - KPIT (Qorix).
  - Avelabs/Arrow (Cairo).
  - Many freelancers and mid-size ESPs.
- **Competitive density:** Medium-High.
- **Growth:** Stable to growing, but the work is being automated.
  - DATA GAP: no integration-services sizing exists.
  - Syndicated AUTOSAR market figures (mostly licences/tools) range from USD 3.5B (2026, 18.4% CAGR; basic software ~24%, ~USD 0.7B, NextMSC) to USD 6.8-7.9B (8.5-9.4%, Marketintelo) [Data, L; reports disagree >2x].
  - Vector DaVinci 6.4/6.5 AI configuration is commoditising the core task [Data, H].
- **Pros:**
  - It is the Gold niche's natural frame and the founders' core skill.
  - Buyers know exactly what to compare it to.
- **Cons:**
  - "AI configures BSW" has a moat of under one year (Vector).
  - Head-on with Avelabs, the founders' former employer, at the same Cairo cost (non-solicit risk).
  - Security, evidence and metrics stay invisible.
- **Dunford fit:** **Partial.** It shows the BSW expertise but not the security wedge, the evidence, or why AI matters. Good as the expansion frame (year 2+), weak as the entry frame.

### Category 3: Secure ECU integration (automotive cybersecurity implementation: security BSW + HSM + secure boot, with ISO 21434 evidence)
- **Type:** Subcategory. It is a narrow "big fish, small pond" inside automotive cybersecurity, at the point where cybersecurity meets BSW integration.
- **Buyer expectations:**
  - A working, on-target crypto stack (Csm/CryIf/Crypto driver, SecOC, KeyM).
  - HSM firmware integration and secure boot.
  - Key provisioning flow.
  - Traceability to TARA cybersecurity goals and the matching 21434 / ASPICE work products.
  - Experience across MCU families (AURIX, TRAVEO, S32K).
- **Current leaders:**
  - Stack vendors bundling product + services: ETAS/ESCRYPT (CycurHSM), EB (zentur + SecOC), Vector (vHSM).
  - FESCARO (Korea; Infineon partner; all-in-one, including HSM engineering).
  - wolfSSL (wolfHSM, open source).
  - Consultancies that stop at paper (SwRI, UL, VVDN).
  - ESPs offering it as one capability among many (KPIT, Capgemini, Avelabs) [Data, M].
- **Competitive density:** Low-Medium for *cross-vendor, fixed-price implementation services*. That exact offer was found at no one, though FESCARO comes closest and must be checked [Data + Opinion, M].
- **Growth:** Growing and regulation-forced.
  - Automotive cybersecurity overall is USD 3.9-6.9B in 2026, growing 15-20% a year (MarketsandMarkets USD 6.88B to 18.86B by 2033, 15.5%; Roots 17.4%; TBRC 20.1%; Persistence 17.2%) [Data, M on direction, L on level].
  - Software is ~52% of the market; DATA GAP: no implementation-services split.
  - Drivers: R155/R156 mandatory for all new EU vehicles since Jul 2024; China GB 44495 since Jan 2026; KPIT names cybersecurity among budgets reopening in 2026 [Data, H].
- **Pros:**
  - All six strengths become the natural comparison points:
    - Security BSW is the category itself.
    - Cross-vendor stands out against stack vendors that only support their own stack.
    - On-target verified stands out against TARA tools and consultants that stop at paper.
    - Evidence included means a 21434/ASPICE work product comes with the integration.
    - Fixed price per MCU family works because the scope is bounded and repeatable.
    - Published accuracy metrics have no competitor that publishes any.
  - A compliance deadline creates urgency.
  - The scope is small enough to win as a two-person team through ESP subcontracting.
  - It is a specialist frame, which lowers the "Cairo vs India rate" comparison.
- **Cons:**
  - The pond is small. Assume single-digit EUR millions of addressable services per year for a start-up [Estimate, L; no services sizing].
  - Stack vendors are the default trusted supplier for their own HSM stacks.
  - "Cybersecurity" may make buyers expect IDS/VSOC products (Upstream, VicOne) unless the name says "integration".
  - Assessor acceptance of AI-generated evidence is unvalidated.
  - AI capability on security BSW is unproven.
- **Dunford fit:** **Yes, strongly.** It is the only frame where each differentiator answers a question the buyer already asks ("Who can make SecOC + HSM + secure boot work on our mixed stack, with the 21434 evidence, by SOP?"). AI becomes the *reason* the fixed price and metrics are possible, not the headline.

### Category 4: AI-native / "agentic" engineering services ("Services-as-Software")
- **Type:** New / emerging. The category exists for investors and analysts (HFS SaS, Sequoia "Services: The New Software" / autopilots, Mar 2026; General Catalyst's USD 1.5B AI-enabled-services roll-up fund; the May 2026 Anthropic + Blackstone + H&F + Goldman AI-native services firm). There is no automotive buyer category [Data, M].
- **Buyer expectations:** outcome-based pricing (HFS: 56% prefer base fee + outcome kicker); faster cycle time; transparency on AI use and its control; and, in automotive, ISO 26262-8 tool confidence, intacs "is AI use controlled?", and data sovereignty.
- **Current leaders:**
  - In automotive the vocabulary is already claimed by incumbents: KPIT (Mobility Agentic AI suite, CES 2026), Tata Elxsi (DevStudio.ai), Luxoft (AMBER), HCLTech.
  - Embedded-AI platforms frame themselves as software, not services: Code Metal (Series B, Feb 2026), CraftifAI (USD 3M seed), H2LooP (USD 2M) [Data, M].
- **Competitive density:** Medium in automotive, and growing fast; High in investor attention.
- **Growth:** Growing (narrative). HFS forecasts USD 1.5T+ by 2035 [Estimate, HFS; L as a sizing]. There is no automotive-specific sizing (DATA GAP).
- **Pros:**
  - The best story for fundraising.
  - It justifies outcome pricing and published metrics.
  - It invites an investor to read the business as non-linear revenue.
- **Cons:**
  - Tier 1 buyers do not buy against this label. It adds risk in a safety- and assessor-governed process.
  - Incumbents with 13k staff use the same words.
  - It sets up a direct fight with Vector's productised AI.
  - "AI-native ESP" was flagged in Phase 3 as already sold [Data, H].
- **Dunford fit:** **No as a buyer-facing category; yes as the business-model narrative for investors.** It describes *how* the founders deliver, not *what the buyer is buying*.

### Category 5: Compliance evidence / ASPICE & ISO 21434 work products (vs AI-TARA tools)
- **Type:** Existing (head-to-head with tools and consultancies).
- **Buyer expectations:**
  - Templates and tooling.
  - TARA in a recognised method/tool (ThreatZ, ystem, etc.).
  - Assessor-recognised consultants (UL, SwRI, TÜV, ESCRYPT).
  - Pricing per seat or per day.
  - 70-90% time savings claimed by AI tools.
- **Current leaders:**
  - AI-TARA and compliance tools: ThreatZ, C2A, Saphira, Ketryx (>USD 55M), AutoTARA, VxLabs (Giza).
  - Consultancies: UL, SwRI, VVDN, SGS/TÜV [Data, M].
- **Competitive density:** High, and commoditising (6+ AI products) [Data, H, Phase 3].
- **Growth:** Growing with R155/GB 44495, but price per document is falling [Opinion, M].
- **Pros:** urgent, budgeted demand, and it uses Waled's ASPICE skills.
- **Cons:**
  - It frames the founders as "paperwork".
  - It puts them against cheap software (EUR 10-30k per seat).
  - It hides the on-target integration skill, which is the scarce part.
  - VxLabs competes from the same city.
- **Dunford fit:** **No as the lead category.** "Evidence included" is much stronger as a *differentiator inside Category 3* ("the integration ships with its evidence") than as a category of its own.

---

## Category Comparison

| Category | Type | Leaders | Density | Size / growth (indicative) | Your Fit | Risk |
|---|---|---|---|---|---|---|
| 1. Automotive ER&D services / ESP | Existing | KPIT, Tata Elxsi, LTTS, Capgemini, Akkodis | High | USD 150B+ outsourced, 8-14% CAGR, cyclical dip in 2025 | Weak | H |
| 2. AUTOSAR BSW integration services | Subcategory | Vector/EB/ETAS services, KPIT, Avelabs | Med-High | Not sized (AUTOSAR SW USD 3.5-7.9B) | Moderate | M-H (Vector AI) |
| 3. **Secure ECU integration** (security BSW + HSM + secure boot + 21434 evidence) | Subcategory | ETAS/ESCRYPT, EB, Vector (product-led); FESCARO | Low-Med | Within USD 3.9-6.9B auto cyber, 15-20% CAGR, regulation-forced | **Strong** | M (small pond, unproven AI, FESCARO) |
| 4. AI-native / agentic engineering services ("Services-as-Software") | New / emerging | KPIT, Tata Elxsi (auto); Code Metal etc. (platforms) | Medium, rising | HFS USD 1.5T+ by 2035 (all industries) | Weak for buyers / Strong for investors | H (buyer scepticism, assessors) |
| 5. Compliance evidence (ASPICE / 21434 work products) | Existing | AI-TARA tools, UL, SwRI | High | Inside auto cyber; price per document falling | Weak | H (commoditised) |

---

## Category choice and fundraising (services vs software multiples)
- **Legacy IT/ER&D services trade at about 1-4x sales.** HFS (Jun 2026) gives an IT-services average of ~1.5x price-to-sales (TCS 3.7x, Accenture 1.8x, Capgemini 0.7x) [Data, M]. Indian ER&D trades higher: KPIT EV/sales ~2.5-4.5x (2026, compressed after −36% YTD); Tata Elxsi ~7.5-8.8x [Data, L-M; MarketScreener/TipRanks snapshots, dates unclear]. Phase 3: services-shaped pitches get 1-3x revenue [Opinion, M].
- **Software and AI-native companies trade much higher, with conditions.** Public SaaS median EV/revenue is 3.4-6.7x (conflicting 2026 figures); private AI software median ~3.9x (multiples.vc); "AI-core" SaaS ~12.5x; HFS's "AI-native" ~46x is skewed by frontier labs [Data, L; aggregator sources]. Investors now test gross margin, because AI-native firms run at 50-70% gross margin with human-in-the-loop costs, and they test revenue quality [Data, L-M].
- **Implications [Opinion, M]:**
  1. Leading with Category 1 or 2 signals a services multiple. Leading with Category 4 to buyers costs sales. The answer is to **split the frames**: Category 3 for buyers, Category 4 (Services-as-Software for safety- and security-critical embedded software) for investors.
  2. What converts a services multiple into a software-like one is evidence of **non-linear delivery**: a fixed-price package per MCU family that is reused across customers, rising gross margin per package, the share of work products produced by agents, and the published benchmark / verification-and-evidence harness as owned IP. The Secure ECU package is the most productisable unit, so Category 3 also helps the investor story.
  3. General Catalyst's roll-up thesis (buy services firms, add an AI platform, lift margins) shows investors will fund AI-enabled services. They expect proof of margin expansion, not just an AI claim.
  4. Corporate VCs (Bosch, ZF, Qualcomm, BMW iVentures) and chip vendors (Infineon PDH) will understand Category 3 immediately, which shortens the strategic-investor path.

---

## Recommendation
**Position into the subcategory "Secure ECU integration": fixed-price, cross-vendor integration of AUTOSAR security BSW, HSM firmware and secure boot, verified on target and delivered with its ISO 21434 / ASPICE evidence.** Use AI as the *enabler* ("that is why the price is fixed and the accuracy is published"), not as the category.

Why [Opinion, M]:
1. **It is the only frame where all six strengths are obvious and relevant.** In Categories 1, 2 and 5 they look like either generic ESP claims or paperwork.
2. **The pond is defensible today.** Stack vendors are single-stack by design, TARA tools and consultancies stop at paper, and big ESPs bundle security as one line among dozens. Nobody found sells the cross-vendor, fixed-price, evidence-included package. Check FESCARO before claiming "only".
3. **Demand is forced by regulation** (R155/R156, GB 44495), which gives urgency without having to create a category.
4. **It avoids the two biggest threats.** It does not compete head-on with Vector's AI configuration (it rides on it) or with KPIT's scale.
5. **It can be sold through ESP subcontracting.** A bounded Werkvertrag package matches how BSW work is already bought.

**Qualifier wording to test** (in discovery calls and with Wave 1/2 language):
- (a) "Secure ECU integration";
- (b) "AUTOSAR security integration";
- (c) "Cybersecurity BSW integration".

Avoid plain "automotive cybersecurity", which triggers expectations of IDS/VSOC products. Do not lead with "AI-native ESP" or "agentic engineering services": incumbents already own those words.

**Category ladder:**
1. Wedge: Secure ECU integration.
2. Expansion (Gold niche, year 2+): "evidence-included AUTOSAR BSW integration packages" (Category 2, carrying the reputation from the wedge).
3. Investor narrative throughout: "Services-as-Software for safety- and security-critical automotive software", backed by package reuse, gross-margin and benchmark metrics.

**Category creation is not warranted.** The evidence does not support the cost. Buyers already have the vocabulary (SecOC, HSM, secure boot, 21434), so only the *packaging* is new.

## Data Gaps
- **No sizing of BSW-integration or security-implementation services.** All AUTOSAR and cyber figures are syndicated totals that disagree by 2x or more. Fill: a bottom-up estimate (number of new ECU programmes with HSM per year × security-integration person-months × rate), checked in discovery calls.
- **Tier 1 RFQ and sourcing structure** (panel admission, work-package RFQs, Werkvertrag vs ANÜ shares) was not found publicly. Fill: interviews with Tier 1 purchasing and ESP sales.
- **FESCARO's actual scope, regions and pricing** (possible direct competitor in Category 3). Fill: a Wave 1 or Phase 3 follow-up search.
- **Whether buyers use the term "Secure ECU"** (search volume, RFQ language). Fill: discovery calls; LinkedIn/job-post term counts.
- **HFS/Everest applying Services-as-Software to ER&D specifically:** titles only, reports paywalled. Fill: an analyst briefing (HFS and Everest offer start-up briefings).
- **Valuation multiples for AI-enabled engineering-services start-ups** (private comps). Only generic AI/SaaS aggregator figures were found. Fill: PitchBook/Dealroom comps for Code Metal, CraftifAI, and GC roll-up portfolio companies.
- **ER&D market size.** Zinnov's public figures are from 2019 (outdated). The IMARC and Everest definitions differ.

---

## Appendix: raw search notes (rounds 1-3, with URLs)

## Round 1 notes (partial)
- KPIT describes itself as the "Largest Independent Software and System Integration Partner to the Mobility Ecosystem" [Data, M] https://directory.partner.io/kpit-com (undated directory); TI partner page https://www.ti.com/partner/KPIT
- Tata Elxsi: called an "ER&D provider" with a focus on SDV (aggregator) [Data, L] https://www.indiainfoline.com/company/tata-elxsi-ltd/summary ; it has a Gartner Peer Insights listing under "R&D outsourcing services" https://www.gartner.com/reviews/product/tata-elxsi-r-and-d-outsourcing-services
- LTTS: "global leader in AI, digital and ER&D consulting" (press release, Jan 2026) [Data, H] https://www.businesswire.com/news/home/20260127890511/en
- HFS coined "Services-as-Software" (2024, trademarked). In 2026 it ran SaS Awards and a "Buying Services-as-Software" webinar (21 Jul 2026) [Data, H] https://www.hfsresearch.com/wp-content/uploads/pdf/SasAwardsBrochure_2026.pdf ; https://www.hfsresearch.com/wp-content/uploads/pdf/HFS-Webinar-Buying-SaS_21-07-2026.pdf

## Round 1-2 notes (8 searches/fetches used)
- HFS "Buying Services-as-Software" webinar deck (21 Jul 2026, local pdftotext of the fetched PDF) [Data, H for what HFS says; its sizing is an Estimate]:
  - HFS estimates a "$1.5 trillion+ Services-as-Software (SaS) market is emerging" by 2035. In its 2035 projection, global technology services shrink to ~$1T (CAGR −3 to −5%) and software/SaaS reaches ~$1.5T (CAGR 5%).
  - "Billable hours and FTE-based pricing measure effort, not outcomes"; "Service firms profit from inefficiency" (survey of 605 G2000 executives, 2026).
  - Current commercial model: 54% effort/input based, 26% transaction/output, 20% outcome. Preferred models include "Hybrid: base fee + outcome kicker" at 56% (n=101).
  - PSR (price-to-sales, June 2026): IT services average ~1.5x (TCS 3.7, Infosys 2.0-2.1, Accenture 1.8, HCLTech 1.3, Cognizant 1.0, Capgemini 0.7, Wipro 0.5). AI-native average ~46x (Anthropic 35.5x on a funding round).
  - URL: https://www.hfsresearch.com/wp-content/uploads/pdf/HFS-Webinar-Buying-SaS_21-07-2026.pdf
- IMARC (updated Jun 2026): automotive engineering services outsourcing was USD 150.7B in 2025 and is forecast at USD 503.0B by 2034, a 14.33% CAGR; APAC holds 48% [Data from a Tier-2/3 market-research house, L-M, broad definition] https://www.imarcgroup.com/report/en/automotive-engineering-services-outsourcing-market
- Zinnov Automotive ER&D 2019: spend ~$158B (+5% YoY), Europe ~half [Data, >12 months old, FLAG] https://media.zinnov.com/wp-content/uploads/2022/09/zinnov-zones-automotive-e-rd-services-2019-ratings.pdf
- Phase 3: Everest via Akkodis put automotive engineering spend at USD 240-260B, of which USD 75-80B is SDV (Feb 2026). BCG/NASSCOM: auto ER&D ~USD 500B by 2030, 8-9% CAGR (2024).
- Automotive cybersecurity (total, incl. HW/SW/services): MarketsandMarkets USD 6.88B (2026) to 18.86B (2033), 15.5% CAGR; Roots ~USD 6.6B at 17.4%; TBRC ~USD 3.89B at 20.1%; Persistence ~USD 4.05B at 17.2%. Software is ~52% of 2025 share (MarkNtel). DATA GAP: no implementation-services split. https://pipelinepub.com/news/marketsandmarkets-automotive-cybersecurity-market-press-release ; https://www.rootsanalysis.com/automotive-cybersecurity-market
- Investors: General Catalyst set aside $1.5B (late 2023) for AI-enabled services roll-ups (e.g., Titan, $74M, Aug 2025). Sequoia's thesis is "Services: the new software" / "autopilots". 14 funds have published similar theses (LinkedIn, secondary). On 4 May 2026, Anthropic + Blackstone + H&F + Goldman formed an AI-native enterprise services firm, backed by Sequoia, Apollo, GA and GIC [Data, M, secondary snippets]. https://finder.techleap.nl/news/feed/general-catalyst-s-1-5b-ai-services-transformation ; https://the-ai-native-cfo.beehiiv.com/p/the-general-catalyst-behind-15-billion

## Round 2-3 notes (14 calls used)
- AUTOSAR market (syndicated reports; they diverge by more than 2x) [Data, L]: NextMSC USD 3.49B (2026), 18.4% CAGR to 2035, with basic software ~24% (~USD 0.71B, 2025) https://www.nextmsc.com/report/autosar-market-at5395 . Marketintelo Classic Platform USD 6.8B (2025) at 8.5% (another Marketintelo Classic report: USD 2.19B, 4.2%) https://marketintelo.com/report/classic-autosar-market . These are mostly licences/tools, not integration services. DATA GAP: no BSW integration-services sizing.
- Everest Software Product Engineering PEAK 2026 (TCS-licensed copy, Apr 2026): buyers want partners that "industrialize AI across the SDLC" and expect "measurable outcomes on cost, speed and innovation" [Data, M] https://www.tcs.com/content/dam/global-tcs/en/pdfs/who-we-are/news/analyst-reports/everest-group-software-product-engineering-services-peak-matrix-assessment-2026-global.pdf . Everest has published on the "Shift from Effort to Value" in engineering services (title only).
- LTTS NDR deck (17 Aug 2026): "macro pressures accelerating shift to outcome-based, risk-sharing models" [Data, H] https://nsearchives.nseindia.com/corporate/LTTS_17082026162753_LTTSRegulation30NDRAnalyst.pdf
- KPIT at CES 2026: "Mobility Agentic AI suite" for SW development, testing and integration on Microsoft Foundry [Data, H] https://autotechinsight.spglobal.com/news/5285965/ces-2026-kpit-showcases-agentic-ai-solutions-on-microsoft-ai-infrastructure-for-mobility-applications . HCLTech has an "Agentic AI for ADAS" brochure. So "agentic engineering services" is already incumbent vocabulary in automotive.
- How buyers buy (DE): BSW integration is sourced as "Werkvertrag" (service contract) work packages and freelancer/ANÜ projects on freelancermap/GULP, e.g. "Integration of generic SW modules ... hardware-independent parts of AUTOSAR Basic SW"; "Integration, Configuration and Test of generic SW modules" [Data, M] https://www.freelancermap.de/projektboerse/projekte/it/300496-projekt-integration-of-generic-sw-modules-engine-control-bayern.html . No public RFQ documents (Tier 1 RFQs are private, issued via supplier portals). DATA GAP.
- "Secure ECU" / HSM integration: offered as products by EB (SecOC + zentur HSM FW), Vector (vHSM), wolfSSL (wolfHSM, lists AUTOSAR/SecOC integration), and dSPACE (Cybersecurity Integrator, test). Services: small players (AutoSec Innovation, LinkedIn). No analyst category or ranking exists for security BSW implementation services [Data, M] https://www.elektrobit.com/?p=18784 ; https://www.dspace.com/ko/kor/home/products/sw/impsw/cybersecurity-integrator.cfm
- Embedded AI startups (investor comparables): CraftifAI $3M seed (Mar 2026, agentic embedded SW) https://inc42.com/?p=549273 ; H2LooP $2M seed https://inc42.com/buzz/h2loop-secures-2-mn-to-scale-ai-platform-for-embedded-systems/ ; Code Metal Series B (Feb 2026, Salesforce Ventures + Accel; LLM code translation + formal verification; Bosch a customer) https://yespress.io/code-metal.md . All are framed as platforms/software, not services.

## Round 4 notes (calls 15-20)
- Sequoia, "Services: The New Software" (Julien Bek, Mar 2026): AI companies are "copilots" (sell tools) or "autopilots" (sell outcomes). Enterprises spend about $6 on services for every $1 on software. It describes a "wedge" of work with no budget line or incumbent [Data, M; snippets] https://sequoiacap.com/article/services-the-new-software
- AI-startup economics: AI-native gross margin is 50-70% (inference + human-in-the-loop). Investors scrutinise revenue quality. Public software multiples are near decade lows (Sapphire, Dec 2025) [Data, L-M] https://crv.com/content/ai-startup-funding ; https://sapphireventures.com/blog/2026-the-year-ahead/ . SaaS multiples: median 3.4-6.7x public; AI-core 12.5x; private AI SW median 3.9x EV/revenue (aggregators) [Data, L] https://fungies.io/saas-valuation-statistics-2026/
- ER&D listed multiples: KPIT EV/sales 2026 ~4.5x down to ~2.5x after −36% YTD (MarketScreener snapshots); Tata Elxsi EV/sales ~7.5-8.8x (TipRanks/MarketScreener); JM Financial values Tata Elxsi at 25x FY28 EPS (Reduce), Oct 2026 [Data, L-M] https://www.marketscreener.com/quote/stock/KPIT-TECHNOLOGIES-LIMITED-105516357/ ; https://www.tipranks.com/stocks/in:tataelxsi/statistics ; https://www.businesstoday.in/markets/stocks/story/kpit-tech-tata-elxsi-ltts-tata-tech-share-price-targets-for-erd-stocks-top-pick-560067-2026-10-07
- Cyber engineering services providers: SwRI (TARA, 21434 and R155 assessments), UL (TARA workshops, work-product gap analysis), VVDN (21434/R155/R156 alignment), and FESCARO on Infineon's partner page: "all-in-one ... consulting to obtain necessary certifications, TARA, HSM solution, engineering, and testing" [Data, M] https://www.infineon.com/cms/en/partner-network/microcontroller-partners/preferred-design-houses/fescaro/ ; https://ul.com/sites/default/files/2024-10/Automotive_Cyber_Consulting_Sell_Sheet.pdf ; https://swri.org/node/956 . Demand signal: a Swedish consultancy is building a network of senior automotive cyber consultants for OEM/Tier 1 assignments (Sep 2026) https://www.framtid.se/yrke/cybersakerhetschef/lediga-jobb/cyber-instincts-ab/senior-automotive-cybersecurity-engineer
- RISE: R155/R156 mandatory for all new vehicles from Jul 2024 [Data, H] https://ri.se/en/expertise-areas/services/technical-service-for-road-vehicles-cybersecurity
- HSM stacks on AURIX: ETAS CycurHSM (NIST CAVP certified), EB zentur, wolfHSM (GPLv3, TC3xx; v2.0.0 integrates wolfBoot) [Data, H] https://www.embedded.com/?p=4480974 ; https://www.wolfssl.com/wolfhsm-infineon-tc3xx-v2-0-0/ . A follow-up search on FESCARO's own scope returned nothing (DATA GAP).
- No 2026 funding found for AI ASPICE/21434 compliance start-ups beyond Phase 3's list. Autosifu (India, pre-funding) does vehicle pen-testing [Data, L] https://dealroom.co/just-founded/autosifu/
