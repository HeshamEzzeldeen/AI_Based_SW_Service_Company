Status: COMPLETE. All 4 rounds done; 19 of 25 WebSearch/WebFetch calls used (18 searches + 1 fetch). Raw round notes with every source are in the appendix at the end.

# Alternative Mapping: AI-native AUTOSAR Classic BSW + cybersecurity BSW delivery (Tier 1 / OEM ECU teams)
*Generated: 2026-10-25 | Agent A1 (JTBD lens) | Builds on Phase 3 (`../../03-competitors.md`, battle cards, `raw/pricing-intelligence.md`)*

**Labels:** [Data] = sourced fact, [Estimate] = derived number, [Opinion] = analyst judgement; confidence H/M/L. Phase 3 claims cite the Phase 3 file. New claims cite URLs in the appendix. Switching-cost ratings are [Opinion, M] unless marked otherwise.

---

## The Job to Be Done

**Core functional job, in the buyer's words (reconstructed):** "Get this ECU's basic software configured, integrated and secured on our target MCU, with the evidence our OEM and the assessor will accept, by the SOP date, without blowing my headcount or budget." [Opinion, M]

The job has four parts, and buyers often hire different alternatives for each:
1. **Configure and integrate BSW** (EcuC, MCAL, OS, Com/Diag stacks, RTE) on the chosen stack (MICROSAR, EB tresos, ETAS RTA-CAR). This work is repetitive and plentiful, and derivative ECUs make up much of it.
2. **Make the ECU secure.** Csm/CryIf/Crypto driver, SecOC, KeyM, HSM firmware, secure boot and key provisioning across stack and silicon (AURIX CSRM, NXP HSE, Renesas ICU). Experts are scarce and documentation is under NDA or fragmented (NXP: full HSE docs need an NDA; forum provisioning questions go unanswered) [Data, M].
3. **Produce the evidence.** ASPICE SWE.1-6 work products (CL2 is the common OEM minimum) and the ISO 21434 work products (cybersecurity case, TARA traceability to implementation) that feed the OEM's R155 type approval [Data, M].
4. **Absorb peaks.** Staff the release crunch before SOP and then shed the capacity again.

The buyer does not want "AI" or "hours". They want a **secured, evidenced ECU baseline on time**, and someone accountable if it is wrong [Opinion, M; Phase 3 forum-mining: "Someone needs to be held accountable when things go wrong"].

---

## Direct Competitors (summary from Phase 3; see battle cards)

### Large Indian / global ESPs: KPIT, Tata Elxsi, LTTS, Capgemini Engineering, Luxoft
- **Type:** Direct competitor (agency-outsource)
- **Hired for:** the same job at programme scale: BSW integration teams, ODCs, multi-year frame deals; increasingly fixed-price work packages.
- **Strengths:**
  - Scale, approved-supplier status, TISAX, ASPICE CL2/3 track record [Data, H].
  - KPIT is 68.3% fixed price (Q4 FY26) with "AI-infused delivery" and Qorix BSW; Tata Elxsi runs DevStudio.ai (multi-agent, ASPICE-aligned) [Data, H].
- **Limitations:**
  - AI gains are kept as margin, not passed through [Opinion, M].
  - Small, specialised security packages fall below their deal threshold [Opinion, M].
  - No public AUTOSAR-security AI or accuracy metrics [Data: absence].
- **Best for:** OEMs and large Tier 1s buying capacity for whole programmes.
- **Switching triggers:** ramp-up delays, attrition of named engineers, rate-card pressure, quality escapes before SOP [Opinion, M].
- **Switching costs:** Technical: M | Contractual: H (MSAs, frame agreements) | Emotional: M

### Cairo / regional ESPs: Avelabs (Arrow/eInfochips), Swift Act, Brightskies
- **Type:** Direct competitor
- **Hired for:** low-cost AUTOSAR + 21434 capacity from the founders' own talent pool.
- **Strengths:** Cairo cost (about USD 25-45/h); German/US front offices; Arrow distributor channel [Data/Estimate, M].
- **Limitations:** no AI story; T&M capacity model [Data, M].
- **Switching triggers:** need for fixed price or a faster calendar.
- **Switching costs:** Technical: M | Contractual: M | Emotional: L-M
- *Note:* founders' non-solicit exposure (Phase 3 red flag).

### Stack vendors' own professional services: Vector, Elektrobit (Aumovio), ETAS/ESCRYPT (Bosch)
- **Type:** Direct competitor (the **default** for security BSW)
- **Hired for:** "make our stack work on this MCU and secure it", plus TARA, CSMS/SUMS, audits and training (Vector Consulting) [Data, H].
- **Strengths:**
  - They own the code and the configuration data model. Vector's MICROSAR HSM firmware "can be integrated together with any AUTOSAR Basic Software" and runs on the AURIX TC4x CSRM. ETAS CycurHSM 3.x is integrated into the TC4x CSRM (Apr 2024) and runs on the Renesas ICU-M [Data, H].
  - "Nobody gets fired for calling Vector." Defect fixes and licence support come from the same place [Opinion, H].
  - Vector DaVinci 6.4/6.5 brings agentic configuration and MCP. EB integration-as-code plus pre-integrated MCAL with Microchip (15 Oct 2026) [Data, H].
- **Limitations:**
  - Single-stack. A mixed ECU (MICROSAR BSW + CycurHSM + NXP RTD crypto driver) has no single accountable owner [Opinion, M].
  - German cost base (premium onsite rates) and capacity queues [Data/Opinion, M].
  - Vector's AI messaging does not mention security or crypto [Data, M; Phase 3].
- **Best for:** buyers standardised on one stack with budget and time.
- **Switching triggers:** vendor services queue too long for the SOP; cross-vendor integration falling between vendors; the price of senior vendor consultants [Opinion, M].
- **Switching costs:** Technical: H | Contractual: H (licence + support bundled) | Emotional: H

### AI-TARA / cybersecurity documentation tools: VxLabs, ThreatZ, Ketryx, C2A, Cybellum, etc.
- **Type:** Adjacent tool → direct for 21434 documents
- **Hired for:** TARA and 21434 work products, faster (claims of 70-90% savings, unaudited) [Data, M].
- **Limitations:** stop at paperwork; none implement HSM/SecOC/secure boot [Data, M].
- **Switching costs:** Technical: M | Contractual: M (seat licences) | Emotional: L

---

## Adjacent / Indirect Alternatives (new in this phase)

### Freelancers / contractors (GULP, Hays, freelancermap, freelance.de, Malt)
- **Type:** Agency-outsource (individual)
- **Hired for:** plugging a named skill gap: "we need a SecOC/HSM person for 6-12 months" or "BSW config + MCAL integration, 6 months + extension" (live freelancermap and Hays listings) [Data, M].
- **Strengths:**
  - Fast to get (days to weeks); real supply exists. GULP profiles in 2026 list SecOC feature ownership, Csm/CryIf/Crypto/HSM integration, ISO 21434, vHSM/TARA/ASIL-D (one TÜV-certified architect with 14+ yrs) [Data, M].
  - Cheaper and more flexible than German ESPs. Rates: DACH IT freelancer median EUR 95/h (range 80-120); embedded EUR 85/h; AUTOSAR listing EUR 85/h; security specialists EUR 120-180/h (3rd-party estimate, L). The Freelancer-Kompass 2026 average fell for the first time (EUR 103, -1) [Data, M].
  - Low switching cost (short contracts) [Data, M; Phase 3].
- **Limitations:**
  - A body, not an outcome. The buyer still carries integration risk, evidence and the ASPICE process [Opinion, H].
  - Knowledge walks out at contract end; quality depends on the person; no process maturity to show an assessor [Opinion, M].
  - AÜG scheinselbstständigkeit / hidden labour-hire risk in Germany pushes buyers to Werkvertrag or broker-intermediated contracts [Data, M; Phase 3 gtm-analysis].
  - Security specialists are scarce: profiles show "Stundensatz auf Anfrage" and availability windows months out [Data, M].
- **Best for:** German Tier 1 teams with a strong internal lead who need one extra pair of expert hands.
- **Switching triggers:** freelancer leaves mid-project; the person is unavailable at the crunch; procurement/compliance blocks direct freelancers; cost of 2-3 security freelancers versus one fixed-price package [Opinion, M].
- **Switching costs:** Technical: L | Contractual: L | Emotional: L-M (personal trust in "our" freelancer)
- **[Opinion, M] This is the easiest displacement target**, at a German cost of about EUR 14-19k per freelancer-month (EUR 85-120/h × 160 h) [Estimate, M].

### Body leasing / staffing ESPs (Akkodis, Alten, Ferchau, Bertrandt, EDAG, IAV)
- **Type:** Agency-outsource
- **Hired for:** onsite capacity under framework agreements via AÜG, Dienstvertrag or Werkvertrag (Bertrandt Services offers all three) [Data, M].
- **Strengths:**
  - Already on approved-supplier lists; German language; works-council familiarity; physical proximity [Data/Opinion, M; Phase 3].
  - They hire permanent "Cybersecurity Engineer Vehicle Systems" staff to place (Akkodis Kassel, Jul 2026; FERCHAU Wetzlar, Friedrichshafen with ISO 21434 + AUTOSAR) [Data, M].
- **Limitations:**
  - German cost: about EUR 85-130/h onsite (Phase 3) [Data, M]. 2026 billing rates for Bertrandt/Ferchau/Akkodis: DATA GAP.
  - In distress or restructuring: Bertrandt revenue -18% with a loss, offshoring; Akkodis -4% organic (Phase 3) [Data, H].
  - Generalists: security BSW depth varies by placed individual [Opinion, M].
  - AÜG reform makes outcome contracts the legally cleaner option [Data, M].
- **Best for:** German OEMs and Tier 1s who value proximity and frame-contract simplicity.
- **Switching triggers:** frame-contract renewal, cost-cutting rounds (see AUMOVIO and Bosch below), AÜG maximum-duration limits, poor quality of placed staff [Opinion, M].
- **Switching costs:** Technical: L-M | Contractual: M-H (framework agreements) | Emotional: M
- **[Opinion, M]** These firms are also a **channel** (subcontract prime), as Phase 3 already noted.

### Captive offshore / in-house centres (Valeo Cairo, BGSW India, AUMOVIO Romania/India, Bosch/ZF/Aptiv captives)
- **Type:** Internal alternative
- **Hired for:** the same job at cost, inside the firewall.
- **Strengths:**
  - Huge capacity: BGSW about 35k engineers, target about 38k by 2027 (secondary source) [Data, M]. Valeo Cairo about 2,000-2,500 engineers producing about 50-60% of Valeo SW output, plus an AI Development Center (Apr 2026) [Data, H; Phase 3]. Timisoara has about 84 open AUTOSAR developer postings across employers (Aug-Oct 2026) [Data, M].
  - Same cost base as the founders (Cairo); no supplier qualification; IP stays inside; they already hold the licences [Data/Opinion, H].
- **Limitations:**
  - Booked through SOP. Captives are planned at annual capacity and cannot flex for peaks [Opinion, M].
  - Being cut: AUMOVIO is removing up to 4,000 R&D roles by end-2026 including India, Romania and Serbia, targeting R&D <10% of sales in 2027 (from 11.9%) and "intensifying development partnerships". Bosch is cutting another 13,000 jobs [Data, H]. Headcount freezes create demand for outcome-priced external work [Opinion, M].
  - Security-BSW expertise is concentrated in a few people at headquarters [Data, Tier 3; Phase 3].
- **Best for:** large Tier 1s with captives in Cairo/India/Romania.
- **Switching triggers:** hiring freeze + SOP crunch; captive lacks HSM/key-provisioning skill; a new MCU family (TC4x, S32K3/S32G, RH850/U2x) the captive has not done before [Opinion, M].
- **Switching costs:** Technical: L | Contractual: L | Emotional: **H** (internal politics; "replacing our own people")
- **[Opinion, M]** Pitch overflow and specialist packages, never replacement.

### MCU vendors' reference integrations and partner networks (Infineon, NXP, Renesas, Microchip)
- **Type:** Adjacent tool / free starting point
- **Hired for:** "get the HSM/crypto running on our silicon" using reference SW, demo apps and FAE support.
- **Strengths:**
  - Free or bundled with the silicon. NXP RTD includes the AUTOSAR Crypto driver using HSE plus an mbedTLS-on-HSE example. Renesas ships ICU-M firmware and an ICU-M LLD reference driver. EB + Microchip pre-integrated MCAL [Data, M-H].
  - Silicon vendors curate partner networks (Infineon Security Partner Network includes Vector; TC4x CSRM co-developed with ETAS) [Data, H].
- **Limitations:**
  - Reference ≠ product. NXP full HSE docs are under NDA; SCST is paid "premium software"; an NXP forum SHE key-provisioning-in-MCAL question went unanswered and was deferred to another team [Data, M].
  - They route integration to stack partners (Vector, ETAS) instead of doing it [Opinion, M].
  - No ASPICE/21434 work products for the customer's ECU [Opinion, H].
  - FAE support is prioritised by volume, so small Tier 1/2 programmes get little [Opinion, M].
- **Best for:** teams prototyping security on a new MCU; teams with strong in-house integrators.
- **Switching triggers:** reference demo works but production integration (key provisioning flow at end-of-line, secure boot chain, SecOC across the stack) does not; FAE support stalls [Opinion, M].
- **Switching costs:** Technical: L | Contractual: L | Emotional: L
- **[Opinion, M]** A partner, not a rival. An MCU vendor's partner listing is a lead source.

### DIY with coding agents + vendor AI/MCP (Copilot, Claude Code, Devin/Windsurf, Gemini Code Assist, Cursor; Vector MCP/EcuC-as-Code; PopcornSAR PAIO; AurigaExplore)
- **Type:** Adjacent tool / internal
- **Hired for:** speeding up the internal team's configuration and code; "do more with the same headcount".
- **Strengths:**
  - Already licensed company-wide (Bosch Copilot org, Mercedes Devin, Valeo Gemini) [Data, H; Phase 3].
  - Vector DaVinci 6.4/6.5 agent + MCP lets any agent drive MICROSAR configuration. PopcornSAR PAIO offers "describe what you need in plain language instead of clicking through thousands of ARXML parameters" with Claude/Gemini/Codex runtimes. AurigaExplore ARXML assistant has BYO model gateways, self-hosted Claude included [Data, M; vendor claims].
  - Cheapest marginal cost; IP stays inside [Opinion, H].
- **Limitations:**
  - Measured gains are modest: 10-19% surveyed (Capgemini, Oct 2026); TUM found only template-augmented prompts produced working automotive code [Data, H; Phase 3].
  - No tool-confidence argument (ISO 26262-8 Cl. 11) and no "controlled AI use" evidence for assessors; only 5% of automotive organisations have mature AI governance [Data, H; Phase 3].
  - Security BSW is the least documented area (NDA silicon docs), so agents have the least to learn from [Opinion, M].
  - DATA GAP: no first-hand public reports of Claude Code/Copilot on BSW/ARXML found (3 query variants across Phase 3 and 4).
  - GlobalLogic: "AI is not a shrink-wrapped silver bullet" in ASIL domains [Data, M].
- **Best for:** large Tier 1s with internal AI programmes, on derivative ECUs they already understand.
- **Switching triggers:** the assessor asks "how is AI use controlled?"; an agent-generated config causes a late integration bug; leadership demands a measurable AI ROI the team cannot show [Opinion, M].
- **Switching costs:** Technical: L-M | Contractual: L | Emotional: M-H (the team's own AI initiative; "we built it")
- **[Opinion, M]** Threat rises to High by 2027-28 (Phase 3). Turn it into a second product: validation harness, skills/MCP packs, evidence templates.

---

## Manual / Status Quo Alternatives

### Status quo A: Internal team works harder (overtime, re-prioritisation, slipping internal milestones)
- **Type:** Status quo
- **Hired for:** getting it done without new spend or procurement.
- **Strengths:** no purchase order, no supplier onboarding (an estimated 6-18 months for a new supplier, Phase 3), no IP risk [Opinion/Estimate, M].
- **Limitations:**
  - Integration is "slow and painful" and "a single parameter change cascades into hours of rework" [Data, Tier 3; Phase 3].
  - ECU delivery slips "strain relationships and increase costs" with the OEM (dSPACE, vendor article) [Data, L-M].
  - DATA GAP: no named 2026 SOP slip publicly attributed to BSW integration.
- **Switching triggers:** OEM escalation; a missed B/C-sample milestone; burn-out or attrition of the one security expert [Opinion, M].
- **Switching costs:** Technical: L | Contractual: L | Emotional: M (admitting the team cannot make it)

### Status quo B: Cut or defer scope (ship without full SecOC coverage, defer secure boot or key-management features, plan "fix in a later SW release / OTA")
- **Type:** Status quo / non-consumption
- **Hired for:** protecting the SOP date by dropping security work.
- **Evidence:**
  - At fleet level, the precedent is stark. VW (Up!, Transporter 6.1) and Porsche (ICE Macan, 718 Boxster/Cayman) **dropped models from EU sale rather than re-engineer electronics for R155**; the cost was "deemed too high" [Data, H; Apr 2024, >12 months old].
  - Doing nothing *is* a real alternative at programme level [Opinion, M].
- **Limitations:**
  - R155 applies to all new EU registrations since Jul 2024, and GB 44495 in China since Jan 2026. OEM flow-down clauses make security features contractual for Tier 1s [Data, H; Phase 3].
  - Deferring security for a new ECU risks the OEM's type approval [Opinion, M].
- **Switching triggers:** OEM RFQ/flow-down makes SecOC/secure boot mandatory; new MCU generation (TC4x, S32K3) removes legacy SHE-only options; Chinese market entry (GB 44495) [Opinion, M].
- **Switching costs:** Technical: L | Contractual: L | Emotional: L-M

### Status quo C: Accept the audit finding (ASPICE or 21434), run an improvement plan, re-assess later
- **Type:** Status quo
- **Hired for:** "paper over" missing work products and keep shipping.
- **Evidence:**
  - ASPICE is not pass/fail. OEMs set the required CL per project (CL2 common, CL3 planned), and shortfalls are handled through the customer relationship, typically via improvement plans [Data, M].
  - An unverified vendor blog (Safeguard, May 2026) says "several OEMs have had findings that pushed back type approval decisions in 2024 and 2025". It also says suppliers that treated audits as paperwork "frequently received findings that affected their program qualification status", and that "the linkage between the CSMS and supplier-delivered evidence is often thin" [Data, L].
- **Strengths:** cheap in the short term; findings are survivable [Opinion, M].
- **Limitations:**
  - Repeated findings hit supplier ratings and future sourcing ("filtered out of new programs", Tier 3) [Data, L].
  - One premium OEM found that ASPICE suppliers detected 90% of defects 11 months before SOP, against 2 months for non-ASPICE suppliers. OEMs therefore link process maturity to launch risk [Data, M; vendor explainer].
- **Switching triggers:** a finding that blocks a nomination or sourcing decision; OEM demands a re-assessment before the next sample; the cybersecurity case for an ECU cannot be closed for type approval [Opinion, M].
- **Switching costs:** Technical: L | Contractual: L | Emotional: M (the manager's reputation)

---

## Jobs to Be Done (functional, social, emotional)

*All [Opinion, M] unless noted: reconstructed from Phase 3 forum and social mining and this phase's evidence. Validate in interviews (Phase 6).*

### Functional jobs
1. **Get the ECU's BSW configured and integrated on target** for each sample (A/B/C) and for SOP, including derivatives.
2. **Make the security stack work end to end:** Csm/CryIf/Crypto driver → HSM firmware → SecOC/KeyM, secure boot chain, key provisioning at end-of-line, across stack + silicon.
3. **Produce assessor- and OEM-accepted evidence:** ASPICE SWE.1-6 traceability and reviews; 21434 cybersecurity case and TARA-to-implementation links that the OEM can use for R155/GB 44495 type approval.
4. **Flex capacity for the pre-SOP crunch** without hiring permanently (hiring freezes at AUMOVIO and Bosch [Data, H]).
5. **Hit the budget:** keep R&D cost per ECU inside the target (e.g. AUMOVIO R&D <10% of sales [Data, H]) and show savings to purchasing.
6. **Adopt AI safely:** show management an AI productivity gain without creating a tool-qualification or audit problem.

### Social jobs
1. **"Don't be the manager whose ECU slips SOP"** or causes an OEM escalation.
2. **"Pass the ASPICE / R155 / 21434 audit without a finding"** and be seen by the OEM as a mature, low-risk supplier (supplier rating, next nomination).
3. **"Be seen as the one who brought AI in responsibly"**: modern, but not the person whose AI-generated config caused a field issue.
4. **"Protect my team"**: avoid looking like I am replacing internal engineers or the captive centre (politics).
5. **"Pick a supplier my purchasing and quality departments won't question"**: approved-list, TISAX, known names.

### Emotional jobs
1. **Sleep at night before SOP**: confidence that security and integration are not the hidden critical path.
2. **Relief from dependence on one or two irreplaceable security experts** (and fear of losing them).
3. **Feel in control of AI** rather than surprised by it ("someone needs to be held accountable", HN 2026 [Data, Tier 3]).
4. **Avoid the embarrassment** of an audit finding or a type-approval delay traced back to my ECU.

---

## Alternative Landscape Summary

| Alternative | Type | Job match | Key strength | Key limitation | Switching cost (T/C/E) |
|---|---|---|---|---|---|
| KPIT / Tata Elxsi / LTTS / Capgemini / Luxoft | Direct (ESP) | Full job at scale | Scale, approved, fixed price + AI (KPIT) | Small specialised security packages below threshold; AI margin kept | M/H/M |
| Avelabs / Cairo ESPs | Direct (ESP) | Capacity | Same Cairo cost + talent | T&M, no AI | M/M/L-M |
| Vector / EB / ETAS services | Direct (vendor) | Security + stack integration | Own the code, HSM firmware, agentic config | Single-stack; premium cost; queues | H/H/H |
| AI-TARA tools | Adjacent → direct | 21434 docs only | 70-90% claimed doc savings | No implementation | M/M/L |
| Freelancers (GULP, Hays, freelancermap) | Outsource (individual) | Skill gap, 6-12 mo | Fast, EUR 85-120/h, flexible | No outcome/evidence owner; knowledge leaves | L/L/L-M |
| Body leasing (Akkodis, Alten, Ferchau, Bertrandt) | Outsource (staffing) | Onsite capacity | On approved lists, proximity | German cost; distressed; AÜG | L-M/M-H/M |
| Captive centres (Valeo Cairo, BGSW, AUMOVIO RO/IN) | Internal | Full job at cost | Same cost, IP inside, licences | Booked through SOP; being cut; scarce security experts | L/L/H |
| MCU vendor reference SW (Infineon, NXP, Renesas, Microchip) | Adjacent (free) | Security bring-up | Free, silicon-exact | Reference ≠ production; NDA docs; no evidence | L/L/L |
| DIY coding agents + Vector MCP / PAIO | Internal tool | Config speed-up | Already licensed; cheapest marginal cost | 10-19% gains; no tool-confidence/controlled-AI evidence | L-M/L/M-H |
| Status quo A: work harder / slip | Status quo | Avoid spend | No procurement | SOP risk; expert burn-out | L/L/M |
| Status quo B: cut / defer security scope | Non-consumption | Protect SOP date | Saves time now | R155/GB 44495 flow-down makes it untenable | L/L/L-M |
| Status quo C: accept audit finding | Status quo | Keep shipping | Cheap, survivable | Supplier rating, sourcing, type-approval risk | L/L/M |

---

## Key Insights

1. **The real competitors in most deals are freelancers + captives + "work harder", not KPIT.** For a specialised security-BSW package the buyer's default is (a) the stack vendor's consultants if budget allows, otherwise (b) one or two GULP/Hays security freelancers at about EUR 85-120/h, or (c) loading the captive. Position against these first [Opinion, M].
2. **Freelancers are the cleanest switching target.** Low switching costs on all three axes; same price class per month (about EUR 14-19k/freelancer-month in DACH [Estimate, M]); and the freelancer cannot sell an *outcome + evidence + accountability*. A fixed-price "Secure ECU package" is a direct upgrade from "rent a SecOC freelancer" [Opinion, M].
3. **The 2026 cost-cutting wave is a switching trigger, not only a headwind.** AUMOVIO (-4,000 R&D, <10% R&D/sales by 2027, "intensifying development partnerships") and Bosch (-13,000) freeze headcount while SOPs stay fixed, which favours outcome-priced external packages over hires and body leasing [Data, H + Opinion, M].
4. **Nobody owns cross-vendor security integration.** MCU vendors pass it to stack partners, stack vendors cover only their own stack, freelancers cover only themselves, and NXP forum key-provisioning questions go unanswered. The "integration seam" between silicon HSM, stack crypto and SecOC is the gap no alternative is accountable for [Data, M + Opinion, M].
5. **Doing nothing is a credible alternative, and R155 shows how it ends.** VW/Porsche dropped models rather than re-engineer for R155. At ECU level, "defer security / accept the finding" is the status quo to beat. The urgency argument is regulation flow-down (R155, GB 44495) plus findings that hit sourcing [Data, H/L + Opinion, M].
6. **The emotional and social jobs are about blame avoidance, not speed.** "Don't slip SOP" and "no audit finding" dominate. Messaging should lead with *accountable, evidenced delivery by named engineers*; "AI" is the means. This matches the Phase 3 finding that the AI objection is about accountability [Opinion, M].
7. **DIY-with-agents and captives share one weakness:** no controlled-AI / tool-confidence evidence. Selling that evidence layer (harness + templates + sign-off) to DIY teams turns the rising threat into a second revenue line [Opinion, M; aligns with Phase 3].
8. **MCU vendors and staffing firms are channels, not rivals.** Infineon/NXP/Renesas partner networks and distressed staffing ESPs (Bertrandt, Akkodis) need partners for cross-vendor security packages [Opinion, M].

## Data Gaps
- **Freelancer rates specific to AUTOSAR security** (SecOC/HSM): profiles show "auf Anfrage". The EUR 120-180/h security figure is a third-party estimate (L). *Fill by:* asking 3-5 GULP/Hays recruiters or freelancers directly.
- **2026 billing rates for Akkodis, Alten, Ferchau, Bertrandt (AÜG vs Werkvertrag):** not found. *Fill by:* Lünendonk staffing studies; ask Tier 1 purchasing contacts.
- **Captive-centre internal transfer rates** (Valeo Cairo, BGSW, AUMOVIO RO) and whether captives sell security BSW internally: not found.
- **Named SOP slips caused by BSW/security integration:** none found publicly. *Fill by:* interviews ("tell me about the last ECU that slipped").
- **Real consequences of ASPICE/21434 findings** (sourcing blocks, re-assessment timelines): only general/vendor sources; the Safeguard claims are unverified. *Fill by:* intacs assessors; OEM supplier-quality requirement documents.
- **First-hand reports of Claude Code/Copilot/Devin on BSW/ARXML:** none found. *Fill by:* LinkedIn/Reddit outreach; own benchmark.
- **Vector/EB/ETAS professional-services day rates and lead times:** not found (vendor sites; ETAS services returned nothing).
- **Malt / Alten:** no automotive-security results surfaced; coverage of these two is assumed by analogy (L).
- **Switching stories** ("we moved from freelancers/ESP X to Y"): no public examples, consistent with Phase 3's finding that buyer voice is almost absent.

---

# Appendix: Raw round notes (sources)

# Alternative Mapping (A1, JTBD lens) - working notes

## Round 1 findings (freelancers, staffing)
- GULP profiles (2026) list freelance AUTOSAR security engineers with SecOC, HSM, Csm/CryIf/Crypto and ISO 21434. One profile updated Aug 2026 is available from 10 Aug 2026; one TÜV-certified architect with 14+ yrs covers vHSM/SecOC/TARA/ASIL-D for DACH. Rates are not shown ("auf Anfrage") [Data, M] https://www.gulp.de/freelancer/GGBVZMTNG ; https://www.gulp.de/freelancer/9AYXBZJK9 ; https://www.freelance.de/freelancer/304363-Automotive-cyber-security-expert (Jan 2026)
- Hays advertises freelance AUTOSAR architecture/DaVinci tooling projects (Lippstadt/remote) and Classic AUTOSAR BSW + security roles for a premium OEM in Berlin [Data, M] https://www.hays.de/jobsuche/stellenangebote-jobs-detail-senior-software-engineer-it-embedded-security-for-a-premium-automotive-company-berlin-688463/1
- Freelancermap lists 6-month BSW configuration + MCAL integration projects with extension options [Data, M] https://www.freelancermap.de/projektboerse/projekte/entwicklung/2386983-projekt-freelance-embedded-software-developer-germany.html
- Akkodis (Kassel, 28 Jul 2026) and FERCHAU (Wetzlar, Friedrichshafen) hire permanent "Cybersecurity Engineer Vehicle Systems / Automotive" staff (ISO 21434, AUTOSAR) to place with clients [Data, M] https://www.make-it-in-germany.com/en/working-in-germany/job-listings/job/job-12634-BB-643684-7878-3418-S ; https://en.devjobs.de/job/551bf1bfc178f2872ad4e2eebf9ae96d
- Phase 3 rates: freelancermap DACH engineering freelancers average EUR 95/h (Feb 2026); embedded EUR 85/h; AUTOSAR listing EUR 85/h [Data, M] (03-competitors/raw/pricing-intelligence.md)

## Round 2 findings (vendor services, MCU vendors, captives)
- Vector Consulting security portfolio (page dated 31 May 2026): cybersecurity design, TARA, security testing, CSMS/SUMS implementation, audits, supplier risk management, training; "practical implementation support". MICROSAR ships crypto stack, SecOC, Ethernet firewall and an AUTOSAR HSM firmware that "can be integrated together with any AUTOSAR Basic Software" [Data, H] https://www.vector.com/en/business-unit/consulting/insights/articles/security-solutions-at-a-glance/ ; Vector is a member of the Infineon Security Partner Network https://www.vector.com/en/business-unit/software-platform/resources/vector-is-a-member-of-the-infineon-security-partner-network/
- Infineon AURIX TC4x: named HSM-firmware partners are Vector (MICROSAR HSM on the Cyber Security Realtime Module) and ETAS (ESCRYPT CycurHSM 3.x integrated into the CSRM, 29 Apr 2024, >12 months old) [Data, H] https://infineon.com/cms/jp/about-infineon/press/market-news/2024/INFATV202404-098.html ; https://international.electronica-azi.ro/?p=40183. So the MCU vendor routes security integration to stack partners rather than doing it itself [Opinion, M].
- NXP S32K3/S32G: NXP provides only the AUTOSAR Crypto driver in RTD, which uses HSE. Full HSE firmware docs need an NDA. Some safety SW (SCST) is paid "premium software". A SHE key-provisioning-in-MCAL question went unanswered on the community forum, and NXP deferred to another support team [Data, M] https://community.nxp.com/t5/S32K/Support-Request-for-HSE-Firmware-Installation-Secure-Key-Storage/td-p/2181791 ; https://community.nxp.com/t5/S32K/Guidance-Required-for-Crypto-Library-and-HSE-Integration-on/m-p/2371226 ; https://community.nxp.com/t5/S32G/HSE-concept/td-p/2250995
- AUMOVIO (ex-Continental Automotive, spun off Sep 2025) is hiring in Timisoara. About 84 AUTOSAR SW developer postings in Timisoara across all employers (Aug-Oct 2026). Employer split and AUMOVIO AUTOSAR headcount: DATA GAP [Data, M] https://www.hipo.ro/locuri-de-munca/cautajob/Inginerie,IT-Software/Timisoara/ded-Software-Developer--AUTOSAR

## Round 3 findings (captives, status quo, DIY, rates)
- Bosch Global Software Technologies (BGSW, India): about 35,000 engineers, target about 38,000 by 2027 (secondary GCC profile site). Bosch Ltd lists 38,655 associates (31 Mar 2025). New Pune centre to hire about 1,500 in year 1 [Data, M; secondary] https://www.businessofgcc.com/gcc-data/companies/robert-bosch-india ; https://autotechinsight.spglobal.com/news/5265184/bosch-global-software-technologies-sets-up-new-center-in-pune-india
- R155/R156 status quo precedent: the VW Up!, VW Transporter 6.1, ICE Porsche Macan and Porsche 718 Boxster/Cayman were dropped from EU sale rather than re-engineered for R155 (cost of upgrading electronics "deemed too high"). Mercedes said it was unaffected [Data, H; Apr 2024, >12 months old] https://www.fortune.com/europe/2024/04/16/volkswagen-porsche-killing-old-models-new-eu-cybersecurity-rules-opportunity-for-chinese-rival-byd ; https://autotechinsight.spglobal.com/news/5276625/navigating-compliance-costs-oems-dilemma-in-making-legacy-vehicles-compliant-with-cybersecurity-
- ECU delivery slips: dSPACE names software complexity, HW shortages and limited test capacity as the causes of late ECU delivery, which "strain relationships and increase costs" (vendor article, undated) [Data, L-M] https://www.dspace.com/en/ltd/home/news/engineers-insights/5-reasons-of-late-ecu-delivery.cfm. DATA GAP: no named 2026 SOP slip caused by BSW integration.
- EB + Microchip (15 Oct 2026) pre-integrated AUTOSAR to "reduce integration effort, lower development risk"; EB + AutoChips likewise. The MCU-vendor reference integration is moving upstream [Data, H] https://www.microchip.com/en-us/about/news-releases/products/elektrobit-and-microchip-collaborate-on-pre-integrated-autosar-solutions
- ASPICE: many OEMs require CL2 from all suppliers, with CL3 planned. It is not pass/fail, so shortfalls are handled in the customer relationship (improvement plans), not by an automatic ban. One premium OEM found ASPICE suppliers detected 90% of defects 11 months before SOP vs 2 months for non-ASPICE suppliers [Data, M; vendor explainer] https://www.aptiv.com/en/insights/article/what-is-aspice ; https://autocrypt.io/aspice-automotive-software-supply-chain/
- DIY with LLMs: PopcornSAR PAIO (Korea) is an AI AUTOSAR design tool with Claude/Gemini/Codex runtimes ("describe what you need in plain language instead of clicking through thousands of ARXML parameters"). AurigaExplore's ARXML assistant supports BYO model gateways (Azure OpenAI, Ollama, self-hosted Claude). GlobalLogic: "AI is not a shrink-wrapped silver bullet" in an ASIL domain [Data, M; vendor claims] https://kr.linkedin.com/in/popcornsar ; https://www.globallogic.com/insights/blogs/decoding-autosar-ai-workflow-sdv/ . DATA GAP: no first-hand reports of Claude Code/Copilot on ARXML/BSW.
- Freelancer rates: Freelancer-Kompass 2026 average across all freelancers is EUR 103/h, the first decline ever (-1 EUR). The IT DACH median is EUR 95/h (range 80-120); security specialists EUR 120-180/h (jobrise, 3rd-party estimate) [Data, M] https://www.freelancermap.de/blog/stundensatz-it-freelancer/ ; https://www.freelancermap.at/media/press_release/2026-03-17-PM-Einkommen.pdf ; https://jobrise.io/de/blog/freelance-developer-deutschland-2026/

## Round 4 findings (MCU vendors, audits, staffing rates, buyer cost-cutting)
- Renesas RH850: ESCRYPT CycurHSM runs on the ICU-M (SHE/SHE+ to full HSM: secure flashing, SecOC, secure boot). Renesas claimed that for an existing AUTOSAR application the rest is "mainly configuration", cutting effort "by up to 90%" (vendor claim, Nov 2016, very old). Renesas now also ships its own ICU-M firmware and an ICU-M LLD reference driver for RH850/U2C [Data, M] https://www.renesas.com/en/about/press-room/renesas-electronics-and-escrypt-collaborate-state-art-combined-hardwaresoftware-solution-high-level ; https://www.renesas.com/eu/en/application/automotive/automotive-security
- Safeguard blog (8 May 2026, no named sources): "several OEMs have had findings that pushed back type approval decisions in 2024 and 2025"; "the linkage between the CSMS and supplier-delivered evidence is often thin"; suppliers that treated audits as paperwork "frequently received findings that affected their program qualification status"; Tier 3 suppliers without formal processes are "being filtered out of new programs" [Data, L, unverified vendor blog] https://www.safeguard.sh/resources/blog/automotive-iso-21434-supply-chain-2026
- Bureau Veritas runs an on-demand webinar, "UNECE R155 for suppliers" (supplier-side demand for R155 guidance) [Data, M] https://cybersecurity.bureauveritas.com/webinar/webinar-unece-r155-for-suppliers
- Staffing/body leasing: no 2026 Bertrandt/Ferchau/Akkodis billing rates were found (DATA GAP). Proxies: freelance engineer EUR 95/h; employed engineer pay about EUR 33/h; the AÜG (TQZ) tariff from 1 Feb 2026 starts at EUR 15.34/h (lowest group). Bertrandt Services offers AÜG, Dienstvertrag and Werkvertrag [Data, M] https://www.freelancermap.de/blog/?p=68600 ; https://www.tarifregister.nrw.de/material/Arbeitnehmerüberlassung%20(TQZ) ; https://adlershof.de/firmensuche-institute/adressverzeichnis/firma/detail/bertrandt-services-gmbh
- Buyer cost-cutting: AUMOVIO is cutting up to 4,000 R&D roles by end-2026 (India, Singapore, Romania, Serbia, Germany, Mexico) to bring R&D below 10% of sales in 2027 (from 11.9% in Q3 2025) while "intensifying development partnerships". Bosch is cutting another 13,000 jobs (EUR 2.7bn provisions; 7% margin target pushed to 2027 at the earliest). ZF is also cutting [Data, H] https://autotechinsight.spglobal.com/news/5286328/aumovio-plans-strategic-realignment-of-global-r-d-activities-move-to-result-in-loss-of-4000-jobs ; https://thebrakereport.com/aumovio-cuts-4000-rd-positions-by-2026/ ; https://www.boersen-zeitung.de/unternehmen-branchen/ergebnis-von-bosch-bricht-um-fast-die-haelfte-ein
