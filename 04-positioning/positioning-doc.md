# Market Positioning: AI-native AUTOSAR security integration (Cairo)
*Skill: sk-positioning | Generated: 2026-10-25 | Mode: Deep*

*Inputs: raw/alternative-mapping.md (A1), raw/customer-intelligence.md (A2), raw/positioning-perception-audit.md (A3), raw/market-categories.md (B1), raw/trends-timing.md (B2), raw/fescaro-check.md, raw/founder-input.md, and Phase 2-3 files. Labels: [Data] sourced, [Estimate] derived, [Assumption] untested belief, [Opinion] judgement; confidence H/M/L. The company has no name yet, so "[Company]" is a placeholder.*

## Executive Summary
1. [Company] integrates the AUTOSAR security software of an ECU (crypto stack, SecOC, KeyM, HSM firmware, secure boot, secure flashing and diagnostics) on the customer's own Vector or ETAS stack and target MCU, verifies it on the hardware, and delivers the ISO 21434 / ASPICE evidence with it, signed by named senior engineers. The plan is for AI agents to do the bulk of the work under controls built to the questions assessors now ask; that harness (attribute F) is not built yet [Assumption].
2. It is for BSW and cybersecurity managers at mid-size Tier 1s and OEM ECU teams who face an R155 flow-down or GB 44495 evidence deadline and have no spare in-house HSM expert. Today they rent a senior freelancer, queue for the stack vendor's consultants, or let the security scope slip.
3. It wins because no alternative is accountable for the seam between silicon, stack and evidence: stack vendors and HSM vendors cover only their own products, freelancers sell hours, and AI-document tools stop at paper. [Company] sells that seam as a scoped, fixed-price package.

**Overall strength: Moderate.** The rung is open and the founders have shipped this exact work. But the claim rests on two individuals' track records, two proof points (controlled-AI evidence, published accuracy) are not built yet, and the "only" holds on packaging, which a large ESP could copy.

---

## 1. Competitive Alternatives
*What a buyer does today if [Company] does not exist. Ordered by how often the founders will meet each one, not by company size.* Full map: `competitive-alternatives.md`.

### Alternative Landscape
| Alternative | Type | Job match | Where it falls short |
|---|---|---|---|
| Senior security freelancer (GULP, Hays, freelancermap) | Outsource (individual) | Fills the skill gap for 6-12 months | Sells hours, not an outcome; no evidence ownership or process to show an assessor; knowledge leaves at contract end; scarce ("rate on request") [Data, M] |
| Status quo: team works harder / slips | Status quo | Avoids spend and supplier onboarding | The one or two security experts become the critical path; "weeks to untangle" one mismatch [Data, H] |
| Status quo: cut or defer security scope / accept the audit finding | Non-consumption | Protects the SOP date | R155 flow-down and GB 44495 make it contractual; findings hurt supplier rating and sourcing [Data, H/L] |
| Stack vendor services (Vector, ETAS/ESCRYPT, EB) | Direct (vendor) | Security integration on their own stack | Single-stack by design; premium German rates; queues; nobody owns the mixed-vendor seam [Opinion, M] |
| Captive centre (Valeo Cairo, BGSW, AUMOVIO RO/IN) | Internal | Same job at cost, inside the firewall | Booked through SOP; under headcount cuts (AUMOVIO −4,000 R&D, Bosch −13,000) [Data, H]; security experts concentrated at HQ |
| Large ESPs (KPIT, Tata Elxsi, LTTS, Capgemini, DXC/Luxoft) | Direct (ESP) | Whole programmes, increasingly fixed price + AI | Small security packages below deal threshold; AI gains kept as margin; no published AI metrics [Opinion, M; Data, H] |
| Security product vendors with services (FESCARO, Autocrypt, wolfSSL) | Direct (bundled) | Their own HSM firmware + engineering + TARA | Integrate their own products, not the customer's chosen stack; FESCARO is Korea-centric [Data, M] |
| Cairo ESPs (Avelabs, Swift Act, Brightskies) | Direct (ESP) | Low-cost AUTOSAR + 21434 capacity | T&M capacity; no AI story; the founders' former employer (non-solicit) [Data, M] |
| DIY with coding agents + Vector MCP / PAIO | Internal tool | Speeds up the internal team | 10-19% measured gains; no "controlled AI" evidence; security BSW is the least documented area for agents [Data, H] |
| MCU vendor reference software (Infineon, NXP, Renesas) | Adjacent (free) | Security bring-up on the silicon | Reference ≠ production; NDA documents; no evidence for the customer's ECU [Data, M] |
| AI-TARA / compliance tools (ThreatZ/VxLabs, Ketryx, C2A) | Adjacent | 21434 documents faster | Stop at paper; implement nothing [Data, M] |
| Body leasing (Akkodis, Alten, Ferchau, Bertrandt) | Outsource (staffing) | Onsite capacity under frame contracts | German cost; distressed; quality depends on the placed person [Data, M] |

**Insight:** the alternatives the founders will actually displace are the freelancer, the overloaded internal expert and the deferred scope. KPIT and Vector matter for credibility comparisons, not as the usual lost-deal reason [Opinion, M].

> **Confidence:** Medium. The alternative set is well sourced (12 alternatives, A1 + Phase 3), but how often buyers pick each one comes from inference, not buyer interviews.

## 2. Unique Attributes
*Confirmed against the founders' profiles (`raw/founder-input.md`). Only attributes that are true today are used in the positioning. Two more are marked as proof points to build.*

| # | Attribute | Evidence | Unique vs alternatives? | Defensible? | Use in positioning |
|---|---|---|---|---|---|
| A | **Security BSW integrated and verified on target, end to end:** crypto stack (Csm/CryIf), SecOC + FVM + KeyM, HSM integration and HSM updater, secure boot (incl. OTA), secure flashing, secure diagnostics; SWE.2 design of secure logging, storage, debugging | Hesham: 5 security programmes 2021-2026 (target MCU stated for two: AURIX TC3xx and TRAVEO); Vector Certified Embedded Professional AUTOSAR Classic - Security [Data, founder-supplied, H] | Partly. Vendor services and some freelancers have it; ESPs have it in individuals. Unique in combination with B-D | Medium (people-based until codified) | **Yes, core** |
| B | **Works on the customer's stack, across vendors:** delivered on Vector MICROSAR (on Infineon AURIX TC3xx and TRAVEO) and on ETAS RTA with ETAS HSM (on Infineon AURIX, confirmed by Hesham 2026-10-25) | Hesham's projects [Data, H]. Stack vendors are single-stack by design [Data, H]; no ESP homepage claims "stack-agnostic" [Data, M] | **Yes** against vendors and HSM-product sellers. Not against ESPs, which also work on several stacks but don't sell it as a package | Medium. Breadth must grow (EB, NXP HSE, Renesas, TC4x) | **Yes, with honest scope:** "Vector and ETAS stacks on Infineon today" |
| C | **Evidence included:** ASPICE SWE.1-SWE.6 (incl. SWE.2 owned by Waled) and the ISO 21434 work products that trace to the implementation, shipped with the integration | Waled: complete SWE.2 owner; Hesham: SWE.2/SWE.3 security design and ASPICE quality control [Data, H]. Not shown in either profile: SWE.1 or SWE.4-6 ownership, ISO 21434 cybersecurity-case or TARA authorship, ASPICE-CS SEC.1-4 work [founder-input]. Nobody bundles implementation + evidence at a fixed price [Data, M] | **Yes**, as a bundle. TARA tools sell documents; vendors sell implementation | Medium | **Yes, conditional:** ASPICE SWE evidence today; full ISO 21434 work products once a 21434/TARA hire or partner is in place (founder decision 2026-10-25). The guarantee wording is a Phase 5 decision |
| D | **Named, accountable senior engineers sign each work product** (proposed split, not past roles: Waled: architecture, SWE.1-2, FuSa; Hesham: integration and security, SWE.3-5, 21434) | Founders' profiles [Data, H] show Waled as SWE.2 owner and Hesham on SWE.2/SWE.3; the rest of the split is an [Assumption]. Assessors now ask "can the author be held accountable" and use "comprehension-testing interview questions" [Data, H, intacs-listed event 2026-10-23]. Capgemini states "whoever does the work does not sign it off" but sells it only as an essay [Data, H] | **Yes** as a sold commitment | Low-Medium (easy to say, hard to scale) | **Yes** |
| E | **SM2 / Chinese crypto algorithm experience** | Listed top skill; current programme is a Chinese-customer EPWT ECU [Data, founder-supplied; the customer's nationality is an Assumption] | Rare among EU-facing providers [Opinion, L] | Medium | **Yes, in GB 44495 outreach only** |
| F | **Assessor-controlled AI:** versioned prompts and config, deterministic validators, a provenance log per artifact, client IP kept on controlled infrastructure, mapped to the four intacs axes | Not built [founder-input]. The assessor frame is real and early [Data, H] | Would be unique today | High if built first (process IP + data) | **Proof point to build.** Do not claim until it exists |
| G | **Published accuracy and rework metrics** for agent-produced configuration and evidence | Not built. Nobody publishes any; every competitor "% faster" is "up to" with no baseline [Data, H] | Would be unique | Medium-High (the benchmark becomes owned IP) | **Proof point to build** |
| H | Fixed price per package, with AI savings passed through | Business-model choice. Fixed price alone is table stakes (KPIT 68%) [Data, H]; pass-through is unclaimed [Data, M] | Pass-through: yes. Fixed price: no | Low (copyable) | Supporting line only; detail in Phase 5 |

**Dropped as non-unique:** "AI-native" (5 of 9 competitor homepages lead with AI [Data, H]; A3 words this as "five of eleven competitors", counting all 11 audited, of which 9 homepages were fetched), "human-in-the-loop" (spreading fast: VxLabs, LTTS, Capgemini, Tata Elxsi), "Cairo cost" (owned by Avelabs and Valeo; neutralised by KPIT Tunisia), "fixed price" on its own.

**Founder note, "we will hire experts for missing areas":** that widens B over time, but each stack or MCU family enters the positioning only after the team has delivered on it. The most valuable first additions are EB tresos + NXP HSE and Renesas ICU-M / AURIX TC4x CSRM [Opinion, M].

> **Confidence:** Medium-High for A, D (documented personal experience); Medium for B, C (real but narrower than "any vendor"); Low until built for F, G.

## 3. Value Themes
*Attribute → so what → customer outcome, in the buyer's words (A2 language map).*

### Theme 1: "The security stack works on your ECU, whichever vendors are in it"
- **Attributes:** A, B (and E for China programmes).
- **Customer outcome:** the crypto stack, SecOC, HSM and secure boot pass on target, across the silicon vendor's MCAL and the BSW vendor's stack, without pulling the two senior integrators off other programmes. In their words: no more "weeks to untangle" a single mismatch; the seam where "the customer then does the integration" is someone else's job.
- **Evidence:** pains #1-3 and #5 in A2 (GlobalLogic 2026-05 [Data, H]; TI MCAL guide [Data, H]; BorgWarner SAE 2026-01 [Data, H]; job ads asking for 6-11+ years across the full stack [Data, M]).

### Theme 2: "Evidence your OEM and assessor accept, signed by people who can defend it"
- **Attributes:** C, D (F once built).
- **Customer outcome:** the 21434 work products and ASPICE SWE evidence arrive "in the required format" with the implementation, and a named engineer can sit the assessor's interview. The buyer passes the supplier security review and stays a "Best-in-Class", low-risk supplier.
- **Evidence:** pain #4 (CYMOTIVE: "endless issues during the supplier security review" [Data, M, 2022, >12 mo]); pain #8 and the intacs-listed assessor frame ("is that use controlled?", "can the author be held accountable" [Data, H]); only 5% of automotive organisations have mature AI governance [Data, H, Capgemini Oct 2026].

### Theme 3: "A fixed scope and price you can plan before the deadline"
- **Attributes:** H (G once built).
- **Customer outcome:** one bounded package per ECU with a defined acceptance test on target, priced up front, instead of an open-ended freelancer or ESP ramp-up. It fits a project budget during a headcount freeze and lets the buyer try a new supplier on one ECU ("selective adoption").
- **Evidence:** headcount cuts with fixed SOPs (AUMOVIO, Bosch [Data, H]); 84% of Tier 1s favour "selective adoption" [Data, H, KPMG 2026]; buyers want "outcome-based pricing" (Bain 2026, P3) [Data, M].
- **Caution:** this theme supports the first two; on its own it is copyable.

> **Confidence:** Medium. Themes 1-2 map to well-evidenced pains; buyer willingness to pay for them is unvalidated (no buyer interviews yet).

## 4. Best-Fit Customers
**Profile (characteristics, not demographics):**
1. **A dated security-evidence trigger within 6-12 months:** OEM R155 / 21434 flow-down for a new ECU, or a **GB 44495 carry-over retrofit** for a platform sold in China (all existing types by 1 Jan 2028 [Data, H]).
2. **Runs Vector MICROSAR or ETAS RTA on Infineon AURIX or TRAVEO**, the founders' proven ground, ideally mixed with a third-party HSM firmware or MCAL (the unowned seam).
3. **No in-house HSM / security-BSW expert, or one overloaded expert;** today fills the gap with a long-term German freelancer or vendor consultants.
4. **Mid-size Tier 1 (about 1-10 secure ECU programmes a year) or an OEM in-house ECU team** that already buys from best-cost locations, so Cairo delivery is normal.
5. **Under ASPICE L2/L3 pressure with weak SWE traceability.**

**Channel buyer (first revenue path):** an approved ESP or staffing prime (e.g. distressed body-leasing firms, or Cairo/Indian ESPs lacking security depth) that subcontracts the security package and carries TISAX and the supplier listing [Opinion, M; Phase 3 GTM].

**Why they care more:** a dated deadline makes the security work non-deferrable even in the 2026 ER&D trough, and with no spare expert the alternative is an expensive freelancer who leaves no evidence trail [Opinion, M].

**Poor fit:** large Tier 1s with captive centres and master ESP contracts; OEMs that restrict offshore access to security modules; programmes with no deadline; EB-only or NXP/Renesas-only programmes until the team has delivered on them.

> **Confidence:** Medium-Low. Built from A2 evidence plus the founders' track record; no buyer has confirmed it (Phase 6).

## 5. Market Category
**Chosen category:** **AUTOSAR security integration** (subcategory; "big fish, small pond" where automotive cybersecurity meets BSW integration). Full analysis: `market-category-analysis.md`.

**Why this frame:** it is the only frame where every unique attribute answers a question the buyer already asks: "Who can make SecOC + HSM + secure boot work on our stack, with the 21434 evidence, before the deadline?" The broad ER&D frame hides all of them and invites a rate-card fight with India; "AI-native services" is crowded and buyers don't purchase against it; "compliance evidence" frames the founders as paperwork [Opinion, M; B1].

**Label choice:** "AUTOSAR security integration" uses the buyer's own words from job ads and freelance project listings ("AUTOSAR Security", "Classic AUTOSAR Security Stack") [Data, M]; no public RFQ documents were found. "Secure ECU integration" (B1's working name) is kept as the package/offer name for Phase 5, because "Secure ECU" is a vendor term buyers don't source by [Opinion, M]. Avoid plain "automotive cybersecurity", which makes buyers expect IDS/VSOC products.

**Buyer expectations:** working on-target crypto stack, SecOC, KeyM, HSM, secure boot; key provisioning flow; traceability to TARA goals; experience on the buyer's MCU family; assessor-ready work products.

**Risk:** small pond (no services sizing; inside a USD 3.9-6.9B automotive cybersecurity market growing 15-20% a year [Data, M on direction]); stack vendors are the trusted default for their own HSM; key provisioning at end-of-line is not in the founders' listed experience.

**Investor framing (separate):** "Services-as-Software for safety- and security-critical automotive software", backed by package reuse per MCU family, rising gross margin and the benchmark as owned IP [Opinion, M; B1].

> **Confidence:** Medium. The frame fits the evidence well; the exact label needs testing in discovery calls.

## 6. Trend Overlay
**Primary: assessor-controlled AI.** Assessors are moving from "did they use AI?" to "is that use controlled?" (intacs-listed Gate4SPICE event, 23 Oct 2026; AUMOVIO webinar; intacs SPICE4AI workgroup) [Data, H/M], while only 5% of automotive organisations have mature AI governance and 40% trust AI for development work [Data, H]. This turns the buyer's main AI objection into the reason to buy, and the norm is still forming (early, roughly 12-24 months before it hardens) [Opinion, M]. **Use it only once attribute F exists;** until then, say "built for how assessors now judge AI work" in conversations, not on the homepage.

**Secondary (offer-level only): the GB 44495 carry-over deadline (1 Jan 2028)** and R155 flow-down. Use in the entry offer and outreach; not in the company category, because it expires.

**Not used:** AI adoption hype, EU AI Act / ISO/PAS 8800 (not relevant to AI as an engineering tool), post-quantum crypto (2027+ upsell), talent shortage (not credible during layoffs), low-cost nearshoring (neutralised by KPIT Tunisia) [Opinion, M; B2].

**Would the positioning work without the trend?** Yes. Themes 1-3 stand on regulation-forced demand and the unowned integration seam. The overlay strengthens Theme 2.

> **Confidence:** Medium-High that the trend is real; Medium that buyers will pay for it before assessors codify it.

---

## Expanded JTBD (Deep mode)
| Layer | Job | Evidence | Which theme answers it |
|---|---|---|---|
| Functional | Get the security BSW working on target with HSM firmware, secure boot and key handling across the silicon vendor's MCAL and the chosen stack | A1, A2 [Data, M-H] | 1 |
| Functional | Deliver R155/21434 work products "in the required format" and pass the supplier security review | CYMOTIVE [Data, M, 2022, >12 mo]; Safeguard [Data, L] | 2 |
| Functional | Pass ASPICE L2 (L3 targeted) on SWE.1-6 with real traceability | Aptiv/Autocrypt explainers [Data, M] | 2 |
| Functional | Close production-side security: secure flashing at plant, debug lock, key injection | BorgWarner SAE 2026-01 [Data, H] | 1 (partly; key provisioning is a gap) |
| Functional | Absorb the pre-SOP peak without hiring during a freeze | AUMOVIO, Bosch [Data, H] | 3 |
| Social | "Don't be the manager whose ECU slips SOP or gets a late cybersecurity finding" | A1 reconstruction [Opinion, M] | 2, 3 |
| Social | "Bring AI in responsibly, not be the one whose AI config caused a field issue" | HN "someone needs to be held accountable" [Data, Tier 3]; intacs frame [Data, H] | 2 |
| Social | "Don't look like I'm replacing my own team or the captive" | A1 [Opinion, M] | 3 (pitch as overflow / specialist package) |
| Emotional | Relief from depending on one or two irreplaceable security experts | "Knowledge lives in experts' heads" (EB, P3) | 1 |
| Emotional | Confidence to sign off without "putting my career on the line" | HN 2026 (P3) | 2 |

**The underserved job:** "make the security stack work on target *and* prove it to the assessor, across vendors." Every alternative does one half: vendors and freelancers implement, tools and consultants document [Opinion, M].

## Onliness Stress Test (Deep mode)
- **Draft:** "[Company] is the only AUTOSAR security integration provider that delivers your ECU's security stack working on target, on your existing vendor stack, at a fixed price, with the ISO 21434 and ASPICE evidence included and signed by named engineers."
- **Challenge 1, "only":** true as far as research found (A3 unclaimed-claims table; FESCARO check). FESCARO, Vector, ETAS and Autocrypt bundle implementation with services, but for their own products; eInfochips integrates third-party stacks on T&M without packaged evidence [Data, M]. **Wording must stay "the only one we found"** in any written claim.
- **Challenge 5, 21434 capability:** the founders' proven evidence work is ASPICE SWE.2/SWE.3. Full ISO 21434 work products need a named hire or partner (founder decision 2026-10-25). **Condition added.**
- **Challenge 2, "on your existing vendor stack":** true for Vector and ETAS on Infineon only. **Must be scoped** in copy until EB/NXP/Renesas are delivered.
- **Challenge 3, copyability:** KPIT or an ESP could package the same in months. The defence is speed to the first assessor-validated reference and the controlled-AI / benchmark IP (F, G) [Opinion, M].
- **Challenge 4, buyer relevance:** "evidence included" and "named engineers" map to sourced buyer and assessor language; "fixed price" maps to buyer survey data. Relevance is evidenced; willingness to pay is not.
- **Verdict:** **Pass with conditions** (scope the stacks; say "only one we found"; secure the 21434/TARA hire or partner before claiming 21434 evidence in writing; build F and G within 12 months).

## Positioning Strength Assessment
| Component | Strength | Notes |
|---|---|---|
| Competitive Alternatives | Strong | 12 alternatives incl. status quo; the real rivals (freelancer, deferral) identified |
| Unique Attributes | Moderate | A, B, C, D are real but people-based and narrower than "any vendor"; F, G not built |
| Value Themes | Moderate-Strong | Themes 1-2 match the most evidenced pains and new assessor language |
| Best-Fit Customers | Moderate | Clear characteristics; unvalidated by buyers |
| Market Category | Strong | Subcategory with no services-led owner; buyer vocabulary exists; no category creation needed |
| Trend Overlay | Moderate | Real and early, but depends on building F |
| **Overall** | **Moderate** | Defensible rung, honest scope; strength rises to Strong with one assessor-validated reference and published metrics |

## Strategic Recommendations
1. **Lead with the security wedge, not the Gold-niche promise.** Hold "ASPICE-ready AUTOSAR BSW in half the time and cost" until there is a measured baseline and the 2027 recovery. "Half the cost" against India needs about 2.5-3x productivity, while measured AI gains are 10-19% [Estimate, M; Phase 3]. Expansion frame for year 2+: "evidence-included AUTOSAR BSW integration packages".
2. **Build the two missing proof points first (Phase 6 MVP):** (a) the controlled-AI evidence harness mapped to the four intacs axes; (b) a published benchmark on one reference ECU security package (accuracy, rework rate, review rejections). Have an independent intacs assessor pre-assess the evidence. Target: within 12-18 months, before large ESPs claim "controlled AI" [Opinion, M; B2].
3. **Scope claims to proven ground:** Vector MICROSAR and ETAS RTA on Infineon AURIX/TRAVEO. Widen only after delivery; prioritise hires for EB + NXP HSE and Renesas / TC4x.
4. **Sell first through approved ESPs or staffing primes** that carry TISAX and the supplier listing, and through Infineon partner channels, while working toward TISAX and a company-level reference.
5. **Use the GB 44495 carry-over deadline and Hesham's SM2 experience** for a China-programme retrofit offer. Verify the SM-algorithm requirement first.
6. **Get a legal review before any outreach:** non-solicit and NDA clauses (Avelabs, Luxoft), and whether past programmes can be described even anonymously.
7. **Phase 6 discovery questions:** "How many people on your team can debug a SecOC freshness or HSM provisioning issue on target?"; "What did your last supplier security review find?"; "Would you call this 'AUTOSAR security integration' or something else?"; "How would you describe KPIT, Vector services and your freelancers to a colleague?"

**Social proof warning:** do not fabricate or pre-write testimonials. Use only verifiable quotes. Until there is a company reference, social proof is the founders' anonymised programme history plus the Vector security certification.

## Red Flags
- **No company track record.** All attributes A-D come from the founders' work as employees of Avelabs and Luxoft. Supplier qualification (TISAX, panel listing, references) asks about the company [Data + Opinion, H].
- **Non-solicit / NDA exposure.** The best-fit buyers include the founders' former employers' customers. Do not name programmes or approach those accounts before legal review [Opinion, H].
- **Two proof points are not built** (controlled-AI harness, published accuracy). Claiming them early is aspirational positioning and would fail at the first assessor question [Opinion, H].
- **The "only" holds on packaging, not technology.** A large ESP or FESCARO could launch a similar package; Vector could add security to its agentic configuration [Opinion, M].
- **Key provisioning at end-of-line** is a named buyer pain (BorgWarner) but not in the founders' listed experience. Do not promise it in the first package without a hire or partner [Opinion, M].
- **ISO 21434 / SEC.1-4 evidence is claimed but not yet shown.** "Evidence included" (attribute C) promises ISO 21434 work products and ASPICE-CS SEC.1-4 evidence, but neither founder profile lists 21434 cybersecurity-case or TARA authorship; proven evidence work is ASPICE SWE.2/SWE.3 [Data, founder-input]. **Founder decision (2026-10-25): keep the claim and add a named 21434/TARA hire or partner;** until that person or partner is in place, do not write 21434 evidence into buyer-facing copy or proposals [Opinion, H].

## Yellow Flags
- Small pond: no sizing for security-integration services; assume single-digit EUR millions addressable for a start-up initially [Estimate, L; B1].
- "Human-in-the-loop / governed AI" language will be table stakes by 2027 [Opinion, M; A3].
- Assessor acceptance of AI-generated evidence has no formal intacs/VDA position yet; the frame could harden differently [Data gap].
- GB 44495 urgency depends on no extension and on Chinese OEMs not absorbing retrofits in-house [Opinion, M].
- Cairo talent competition (Valeo AI centre, Avelabs) for the hires that widen the stack coverage [Data, M].

## Data Gaps & Limitations
- No first-person buyer voice from Tier 1 BSW or security managers; best-fit profile and value themes are inferred. Fill: 10-15 discovery interviews (Phase 6).
- No sizing of security-integration services; no Tier 1 RFQ documents.
- No formal intacs/VDA position on AI-generated evidence; GRVA Sep 2026 outcome on R155 not found.
- FESCARO's stack support and NXP/Renesas/ST design-partner offers not fully checked.
- Whether buyers use "AUTOSAR security integration" or another term is untested.
- Founder capabilities come from self-reported profiles; client nationality for the EPWT programme is assumed.
- Resolved 2026-10-25: Hesham confirmed the ETAS RTA / ETAS HSM programmes ran on Infineon AURIX.

## Sources
- Raw research (all 2026-10-25): `raw/alternative-mapping.md`, `raw/customer-intelligence.md`, `raw/positioning-perception-audit.md`, `raw/market-categories.md`, `raw/trends-timing.md`, `raw/fescaro-check.md`, `raw/founder-input.md`.
- Key sources (tier): intacs Gate4SPICE event, 2026-10-23 (T1-2) https://intacs.info/component/rseventspro/event/490-2026-10-23-gate4spice-event-communicating-agreed-work-ai-generated-work-products-onsite-kr ; Capgemini Research Institute, 2026-10-12 (T1) https://www.capgemini.com/news/press-releases/68-of-automotive-organizations-use-or-pilot-agentic-ai-for-product-development-but-only-5-report-mature-ai-governance-2/ ; KPMG Global Tech Report 2026 Automotive (T1) ; TÜV SÜD on GB 44495 (T2) https://www.tuvsud.com/en/knowledge-hub/technical-updates/consumer-products-and-retail-essentials/china-implements-vehicle-cybersecurity-technical-requirements ; GlobalLogic, 2026-05-21 (T2-3) https://www.globallogic.com/insights/blogs/decoding-autosar-ai-workflow-sdv/ ; BorgWarner SAE 2026-26-0628 (T1) ; TI MCAL integration guide (T2) ; AUMOVIO and Bosch cuts via S&P AutoTechInsight (T2) ; Infineon FESCARO partner page (T2).
- Phase 3: `../03-competitors.md` and battle cards.
