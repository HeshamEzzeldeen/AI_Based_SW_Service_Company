# Grand Slam Offer: Secure ECU Package (AUTOSAR security integration)
*Skill: sk-offer | Generated: 2026-10-25 | Status: complete; prices are provisional model outputs until the founders replace the estimated module hours*

*Inputs: 02-niches.md (Gold I, Silver H as first offer), 04-positioning.md (category "AUTOSAR security integration"), 03-competitors/pricing-landscape.md, founder answers on 2026-10-25. Labels: [Data] sourced, [Estimate] derived, [Assumption] untested, [Opinion] judgement. "[Company]" is a placeholder.*

## Founder decisions (2026-10-25)
- **Effort baseline:** a full security scope for one ECU (crypto stack, SecOC/FVM/KeyM, HSM integration and updater, secure boot, secure flashing and diagnostics, on target) took **3-6 person-months** on the founders' past programmes, without AI [Data, founder-supplied, M].
- **Promise:** "Your ECU's security stack working on target, evidence included."
- **Guarantee:** both, i.e. final payment on on-target acceptance **and** free fixes of findings on the delivered scope.
- **Entry offer:** the full security package for one ECU (no separate pilot).
- **Name:** Secure ECU Package.
- **Value-equation ratings:** confirmed as proposed (Dream 8, Likelihood 4, Time 4, Effort 4).
- **Pricing method:** prices come from an hours-based model per package, not from a market anchor. Model: [05-offer/pricing-model.xlsx](05-offer/pricing-model.xlsx).

---

## Step 1: Six P's One-Pager

### Person
- **Role:** BSW/integration manager or cybersecurity manager (sometimes the SW department head) at a **mid-size Tier 1** with about 1-10 secure ECU programmes a year, or an OEM in-house ECU team. Typically 35-50, an engineer promoted into management, based in Germany/EU (later NA, Japan/Korea).
- **Situation:** runs Vector MICROSAR or ETAS RTA on Infineon AURIX/TRAVEO; has one or two overloaded security experts or a long-term freelancer; faces an R155 flow-down or GB 44495 carry-over deadline within 6-12 months.
- **Values and fears:** values predictability, "no surprises before SOP", being seen by the OEM as a low-risk supplier. Fears a late cybersecurity finding, an SOP slip traced to their team, and being the person who brought in an AI supplier that failed.
- **Aspiration:** be the manager who unblocked the programme and passed the supplier security review cleanly.
- **Where they are:** Vector and Infineon/NXP communities, LinkedIn (AUTOSAR, ISO 21434, ASPICE groups), escar Europe, Vector Congress, intacs regional events, VDA QMC, Automotive SPICE conferences, SAE WCX. Reads Elektronik automotive, ATZelectronics, Automotive World, MONOist (Japan).

### Problem
- **Core pain:** the ECU's security stack has to work on target across the silicon vendor's MCAL, the stack vendor's crypto modules and the HSM firmware, and the OEM wants the R155/21434 evidence "in the required format" by a fixed date. No one owns that seam [Data, M; Phase 4].
- **Why now:** OEM flow-down clauses (R155 applies to all new EU registrations since Jul 2024); GB 44495 applies to all existing vehicle types from 1 Jan 2028, so carry-over ECUs need retrofits in 2027; headcount freezes at AUMOVIO (−4,000 R&D) and Bosch (−13,000) while SOP dates stay fixed [Data, H].
- **Cost of not solving:**
  - Hiring freelancers: 3-6 months of a senior DACH freelancer is about **EUR 42-114k for hours only**, with no evidence ownership [Estimate, M: EUR 85-120/h × 160 h × 3-6 months].
  - A finding in the supplier security review or ASPICE assessment costs re-work, re-assessment and supplier-rating damage [Data, L-M].
  - The worst case is a type-approval delay or a lost nomination. VW/Porsche pulled models rather than re-engineer for R155 [Data, H, Apr 2024].

### Pain
- **Rating: 8/10 for buyers with a dated deadline; about 4/10 without one** [Opinion, M; founders to confirm in Phase 6]. Sell only to the first group.
- **In 6 months:** the B/C-sample ships without full SecOC or secure boot; the supplier security review raises findings; the one security expert burns out or leaves.
- **In 2 years:** the OEM's type approval for the platform is at risk, the supplier rating drops, the next nomination goes to a competitor, and China sales of carry-over platforms stop at the GB 44495 deadline.

### Promise
**"Your ECU's security stack working on target, evidence included."** (9 words)

### Plan (cliff-to-cliff bridge)
1. **Scope lock (week 1-2):** intake of security requirements / TARA goals, audit of the customer's stack, MCU, HSM firmware and bootloader; agree the fixed price, the on-target acceptance tests and the evidence list.
2. **Crypto foundation:** HSM firmware integration and HSM updater; Csm/CryIf/crypto driver; key handling (KeyM) for the agreed key set.
3. **Secure boot and secure flashing:** boot chain from bootloader to HSM, including the OTA path where in scope; secure flashing and secure diagnostics access.
4. **Secure communication:** SecOC/FVM configured and verified on the bus with the OEM's freshness and MAC scheme.
5. **Acceptance and handover:** acceptance tests run on the customer's hardware; evidence package handed over; founders walk the customer (and, if wanted, the assessor) through it.

*Calendar estimate: 8-14 weeks per ECU with the two founders plus AI agents [Estimate, L: 3-6 PM baseline; AI speed-up unmeasured]. Do not promise a week count until the first project is measured.*

### Product (what the customer receives)
1. The integrated, configured security BSW **inside the customer's own Vector or ETAS project** (no new tool or licence for them).
2. **On-target acceptance test report:** secure boot, SecOC MACs on the bus, HSM services, secure flashing and diagnostics.
3. **Evidence package for the scope:** ASPICE SWE.2-SWE.6 work products (architecture, detailed design, unit/integration verification, traceability) and the matching ISO 21434 work products once the 21434/TARA hire or partner is in place (Phase 4 decision). Until then, 21434 is sold as "traceability to your TARA goals".
4. **Named sign-off:** each work product signed by Hesham (integration and security) or Waled (architecture).
5. **Derivative recipe:** what changes for variants and how to re-configure.

### Price
**Prices are set by the hours-based model in [05-offer/pricing-model.xlsx](05-offer/pricing-model.xlsx)** (founder decision, 2026-10-25). How it works:
1. **Module hours** (Modules sheet): baseline hours per module for one new ECU, without AI. The defaults are Claude's split of the founders' 3-6 person-month total (480-960 h) across 8 modules; the founders replace them with their own numbers.
2. **Packages** (Packages sheet): each package is a set of modules with a factor (1 = full new work, 0.3-0.6 = reused work, 0 = excluded).
3. **Our cost:** core hours + evidence (30%) + PM and named sign-off (10%), minus the AI saving (15%, unmeasured), plus 15% contingency, at EUR 45/h loaded internal cost.
4. **Two prices, take the higher, round up to EUR 5k:** (A) cost-plus floor that keeps a 35% gross margin after a 10% guarantee reserve; (B) value-based: the hours a team without AI would need × EUR 95/h (DACH freelancer median), minus 50% of the AI saving passed through.
5. **Never quote hours or rates to buyers.** Quote per package only.

**Current model output (Mid estimate, all defaults) [Estimate, L until founders' hours replace the defaults]:**
| Package | Customer-equivalent hours | Our delivery hours | Price | Gross margin | Calendar weeks (2 founders) |
|---|---|---|---|---|---|
| **P1 Secure ECU Package (new ECU)** | 936 | 1,023 | **EUR 85,000** | 36% | ~15 |
| P2 Secure ECU Derivative | 352 | 384 | EUR 35,000 | 41% | ~5.5 |
| P3 Secure Boot & Flashing (no SecOC) | 739 | 808 | EUR 70,000 | 38% | ~11.5 |
| P4 Secure Communication (SecOC; HSM and crypto already in place) | 339 | 370 | EUR 35,000 | 42% | ~5.5 |

*P3 and P4 are smaller packages the model can price; the entry offer remains P1 (founder decision).*

**Founding-customer price (proposal):** EUR 75,000 for P1 for the first three customers in exchange for reference rights. At model defaults that leaves about a 29% gross margin [Estimate, L].

**How P1 compares (same customer-equivalent hours, 936 h):**
| Alternative | Cost for the scope | What's missing |
|---|---|---|
| German ESP / vendor services (EUR 85-130/h) | EUR 80-122k, evidence often billed extra | Single stack; queues |
| DACH freelancer (EUR 80-120/h) | EUR 75-112k | No evidence ownership, no accountability, knowledge leaves |
| Eastern Europe ESP (EUR 45-75/h) | EUR 42-70k | T&M; evidence extra |
| India / Egypt ESP (EUR 23-41/h) | EUR 22-38k | T&M; ramp-up; evidence extra |
| **Secure ECU Package** | **EUR 85k fixed, evidence and guarantees included** | |

**[Opinion, M]** EUR 85k sits at the low end of the German range and inside the freelancer range, with evidence and guarantees included, but it is **2-4x Indian/Egyptian T&M**. Sell to buyers whose real alternative is German freelancers or vendor services.

**What AI leverage does to P1 (AI scenarios sheet) [Estimate, L]:**
| AI saving | Our hours | Margin at EUR 85k | Recalculated price |
|---|---|---|---|
| 0% | 1,184 | 27% | EUR 100,000 |
| 15% (default) | 1,023 | 36% | EUR 85,000 |
| 30% | 861 | 44% | EUR 80,000 |
| 45% | 700 | 53% | EUR 70,000 |
**Insight:** without any AI saving, the cost-plus floor pushes P1 to about EUR 100k; the business only works at the EUR 75-85k level if AI (or reuse) saves at least ~15% of hours. Measure it on the first package.

**Revenue math (skill formula, at P1 = EUR 85k):**
- EUR 100k/year needs 100,000 / 85,000 / 12 = **0.10 packages a month (about 1.2 a year)**.
- EUR 1M/year needs 1,000,000 / 85,000 / 12 = **0.98 packages a month (about 12 a year)**.
- **Capacity check:** two founders (35 h/week, 44 weeks) deliver about **3 P1 packages a year, about EUR 256k**, or about 8 derivatives (EUR 281k). EUR 1M needs roughly 4x the delivery capacity: hires, higher AI leverage, and a derivative-heavy mix [Estimate, L].

---

## Step 2: Value Equation
*Ratings proposed by Claude from the research; founders to adjust. Formula used: Value = (Dream × Likelihood) / (Time × Effort), with Time and Effort rated so that lower is better.*

| Factor | Rating | Reasoning |
|---|---|---|
| Dream Outcome | **8/10** | Security stack working on target and evidence accepted before the deadline: removes the scariest item from the SOP plan |
| Perceived Likelihood | **4/10** | Unknown two-person company, no company references, AI scepticism (40% trust AI for development [Data, H]) |
| Time Delay (lower = better) | **4/10** | 8-14 weeks vs a 3-6-month ESP ramp-up or a freelancer search, but still a quarter of a year |
| Effort & Sacrifice (lower = better) | **4/10** | Customer must onboard a new supplier, give tool and hardware access, share NDA HSM documents |

**Value = (8 × 4) / (4 × 4) = 2.0**

**Weakest factor: Perceived Likelihood.** Levers, roughly in order of impact:
1. **Guarantees** (acceptance-based payment + free fixes on scope): the risk moves to the founders.
2. **Named engineers with a documented record:** anonymised programme list (US OEM ADAS ECU on AURIX TC3xx, US OEM inverter on ETAS, UK luxury OEM ECU on TRAVEO), Hesham's Vector Certified Embedded Professional AUTOSAR Classic - Security. **Only after the NDA/non-solicit legal review.**
3. **Independent assessor pre-assessment** of the first evidence package (Phase 4 proof point).
4. **Selling through an approved ESP** that carries the supplier risk.
With 1-3 in place, likelihood rises to about 7, and Value = (8 × 7) / (4 × 4) = **3.5**.

**Second lever: Effort.** Work inside the customer's existing tools and licences, remote hardware access (customer-shipped boards), a one-page onboarding checklist.

---

## Step 3: Problems & Solutions Brainstorm
| # | Obstacle on the customer's path | Solutions (delivery model) |
|---|---|---|
| 1 | Security stack doesn't work across MCAL, stack and HSM firmware | Integrate and verify on target (DFY); seam checklist per MCU (DIY) |
| 2 | The only security expert is overloaded or leaving | Take the scope off their desk (DFY); knowledge-transfer session at handover (DWY) |
| 3 | OEM wants R155/21434 evidence in its format | Evidence package mapped to the OEM template (DFY); template mapping workshop (DWY) |
| 4 | ASPICE assessment of the security scope | SWE.2-6 evidence included (DFY); pre-assessment walkthrough (DWY) |
| 5 | Fear that AI-produced work won't be accepted | Named sign-off (DFY); provenance log per artifact once built (DFY); assessor walkthrough (DWY) |
| 6 | Unknown supplier: purchasing and qualification | Subcontract via an approved ESP (DFY); supplier info pack: insurance, NDA, data handling (DIY) |
| 7 | IP and data leaving the company / to LLMs | Work on customer-controlled or on-prem infrastructure; no client data to public LLMs (DFY); written data-handling policy (DIY) |
| 8 | Tool licences (Vector/ETAS) | Work inside the customer's licences and seats (DFY) |
| 9 | NDA-gated HSM documentation | Customer passes silicon NDA access; founders sign the NDA chain (DWY) |
| 10 | Budget arrives as headcount, not projects | Fixed price fits a project/Werkvertrag budget (DFY); business-case one-pager vs freelancer (DIY) |
| 11 | Variants and derivatives after SOP | Derivative recipe (DIY); derivative package at reduced price (DFY) |
| 12 | Production security: secure flashing at plant, debug lock | Production handover checklist (DIY); support for the first production flash (DWY) |
| 13 | Key provisioning at end-of-line | **Not in the founders' record:** partner or hire before offering (flag) |
| 14 | China programmes need SM2/SM3/SM4 crypto | SM-algorithm crypto configuration for GB 44495 retrofits (DFY; Hesham lists SM2) |
| 15 | Late surprises before SOP | Weekly on-target status report with test results (DIY); 30-day post-acceptance support (DWY) |

## Step 4: Trim & Stack
| Solution | Cost to deliver | Value to customer | Decision |
|---|---|---|---|
| Integration + verification on target (1) | High | High | **Keep (core)** |
| Evidence package SWE.2-6 (3, 4) | Medium | High | **Keep (core)** |
| Named sign-off (5) | Low | High | **Keep (core)** |
| Acceptance-based payment + fix-findings guarantee | Medium (risk) | High | **Keep** |
| Scope-lock audit (Plan step 1) | Low | High | **Keep** |
| Assessor / OEM walkthrough session | Low | High | **Keep (bonus)** |
| Derivative recipe + derivative price | Low | High | **Keep (bonus)** |
| Production security handover checklist (12) | Low | Medium-High | **Keep (bonus)** |
| 30-day post-acceptance support (15) | Low-Medium | High | **Keep (bonus)** |
| Weekly on-target status report (15) | Low | Medium | **Keep** |
| Data-handling policy + supplier info pack (6, 7) | Low | Medium-High | **Keep (bonus)** |
| SM2/SM3/SM4 crypto for China (14) | Medium | High (China programmes only) | **Keep as an option** |
| Full ISO 21434 work products (TARA, cyber case) | High (needs hire/partner) | High | **Consider:** add once the partner is in place |
| OEM template-mapping workshop | Medium | Medium | Cut (fold into the walkthrough) |
| Knowledge-transfer training course | Medium | Medium | Cut (fold into handover) |
| End-of-line key provisioning (13) | High (not proven) | High | **Cut for now** (partner/hire later) |

### The Offer Stack
**Secure ECU Package: EUR 85,000 per ECU (model output; founding customers EUR 75,000)**
1. Scope-lock audit of your stack, MCU, HSM and bootloader, with a fixed price and acceptance tests agreed up front.
2. Crypto foundation: HSM firmware integration and HSM updater, Csm/CryIf/crypto driver, KeyM.
3. Secure boot and secure flashing, plus secure diagnostics access.
4. SecOC/FVM verified on your bus.
5. On-target acceptance test report.
6. ASPICE SWE.2-SWE.6 evidence for the scope, traced to your TARA goals (full ISO 21434 work products once our 21434 partner is in place).
7. Named sign-off on every work product.
8. Weekly on-target status reports.
**Bonuses:**
- Assessor / OEM walkthrough: the engineers who did the work sit your review.
- Derivative recipe, and the next derivative at EUR 35,000.
- Production security handover checklist (secure flashing at plant, debug lock).
- 30 days of post-acceptance support.
- Supplier information pack and data-handling policy (no client data to public LLMs).
**Option:** SM2/SM3/SM4 crypto configuration for China (GB 44495) programmes.

## Step 5: Enhance the Offer

### Scarcity (real)
The two founders can deliver about **3 new-ECU packages a year** at model defaults (more if the mix includes derivatives) [Estimate, L]. State it plainly: "We take on a limited number of ECU programmes per half-year so that the engineers who sign the work also do it." Exact number to set once the delivery capacity with AI is measured.

### Urgency (real)
- **GB 44495 (all existing types by 1 Jan 2028):** with 8-14 weeks of delivery plus the OEM's own review time, carry-over ECUs need to start by about **mid-2027** [Estimate, M].
- **Founding-customer price** (EUR 75k instead of EUR 85k) ends after three customers.

### Bonuses
Listed in the stack. Each answers an objection: walkthrough → "who defends it?"; derivative price → "what happens with variants?"; production checklist → "what about the plant?"; support → "what if something breaks after you leave?"; data policy → "where does our IP go?".

### Guarantees (founder choice: both)
1. **Acceptance-based payment:** the final 40% is due only when the agreed on-target acceptance tests pass.
2. **Findings fixed at our cost:** any OEM or assessor finding on the delivered scope, raised within 12 months of acceptance, is fixed free.
**Bounds the founders must put in the contract [Opinion, H]:** scope = the agreed modules and evidence list only; customer-side changes (requirements, stack version, MCAL) are excluded; total liability capped at the contract value; professional liability insurance in place. Without these bounds, one bad project could consume the company's runway (Phase 3 red flag).

### Naming
Formula: [Result] + [Time Period] + [Container]. Options:
1. **Secure ECU Package** (Phase 4 candidate; plain and in buyer language) ← **chosen by the founders**
2. Secure ECU 90 (adds a time promise; only once delivery time is measured)
3. On-Target Security Integration Package
4. SecureStart ECU Package
5. Evidence-Included Secure ECU Package

## Step 6: Commodity Check
**Can a buyer compare this side by side with a competitor?** Partly. Procurement will try to convert the price into person-months and compare with an India rate card [Opinion, M].
- **Against freelancers and T&M ESPs:** not directly comparable. They sell hours; this sells a working, evidenced result with acceptance-based payment.
- **Against stack vendor services:** they work on one stack and charge for evidence separately.
- **Against KPIT:** fixed price exists, but not as a published per-ECU package with evidence, named sign-off and a findings guarantee.
- **Against FESCARO:** bundles its own HSM firmware; this package works on the customer's chosen Vector or ETAS stack.

**Verdict: hard to commoditise, provided the founders never quote hours or day rates.** Quote per ECU, per derivative, per outcome only.

---

## Red Flags
- **Guarantee risk on a two-person company.** Both guarantees together are strong but dangerous without liability caps, scope exclusions and insurance [Opinion, H].
- **Price above offshore T&M.** Buyers who benchmark India (USD 25-45/h) will see 2-4x. Target only buyers whose alternative is German freelancers or vendor services [Estimate, M].
- **Full package as the entry offer means a longer first sale** (supplier qualification estimated at 6-18 months direct, 1-3 months via an ESP) [Estimate, L-M, Phase 3]. Keep the ESP subcontract route open from day one.
- **21434 work products depend on a hire or partner** that doesn't exist yet (Phase 4 decision).
- **Legal review before any sale:** non-solicit and NDA clauses, and whether past programmes can be cited.

## Yellow Flags
- Effort baseline (3-6 PM) is from memory of past programmes, not timesheets; AI speed-up is unmeasured.
- Internal cost per person-month (EUR 6-8k) is an assumption.
- Value-equation ratings are Claude's proposal, not buyer data.
- Capacity: about 3 new-ECU packages a year with the founders alone (about EUR 256k) until AI leverage or hires are proven.
- Module hours, package factors, evidence %, AI saving and internal cost in the pricing model are Claude's estimates; the founders should replace them from timesheets of past programmes.

## Sources
- `04-positioning.md` and `04-positioning/` deliverables; `03-competitors/pricing-landscape.md` (rates and the V1-corrected cost table); `04-positioning/raw/alternative-mapping.md` (freelancer rates); founder answers, 2026-10-25.
