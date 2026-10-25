# Phase 1: Diverge -- Divergent Thinking (fast-tracked)

> **Note:** The founder arrived with a formed idea, so this phase was compressed. Instead of a 50+ problem brainstorm, the core idea was split into distinct sub-niches (different buyer, problem, or slice of the V-model) so Phase 2 can score them against each other. A full `/sk-diverge` can be run later to widen the pool.

---

## Founder's Core Idea (verbatim intent)

An automotive software engineering services company that relies on AI agents as much as possible to develop and test software (the work typically done by engineering service suppliers), with human engineers only at the necessary checkpoints in the workflow to guarantee quality. Goal: cut time and cost for Tier 1 suppliers and OEMs.

**Terminology note:** In supply-chain terms, "Tier 3" usually means raw-material/component suppliers. The role described here is an **engineering service provider (ESP)** that sells to Tier 1s and OEMs (in the same space as KPIT, Tata Elxsi, LTTS, Capgemini Engineering, Luxoft, Bertrandt). Positioning as an "AI-native ESP" is clearer to buyers.

---

## Craft Skills (from founder's LinkedIn profile)

Founder: Staff II Embedded SW Engineer at Avelabs (Cairo), ~9.5 years in automotive SW, 10+ in embedded. Projects for Ford (ADAS DAT2.x), GM/Garrett (fuel cell inverter), Daimler/Luminar (lidar), Bentley (cargate), Hande (EPWT).

| # | Skill | Years | Confidence |
|---|-------|------:|:----------:|
| 1 | AUTOSAR Classic BSW configuration & integration (Vector + ETAS stacks: COM, Diag, NvM, Ethernet, XCP, OS/RTE, Mode Mgmt, PN) | ~9 | H |
| 2 | Automotive cybersecurity architecture (HSM, secure boot/flashing/diag/logging/storage/debug, SecOC/FVM/KeyM, crypto stack, SM2) | ~5 | H |
| 3 | Bootloaders & HSM integration (ETAS, Vector; AURIX TC3xx, TRAVEO) | ~5 | H |
| 4 | Diagnostics (UDS, DEM/DCM, DoIP) | ~4 | H |
| 5 | ASPICE work products (SWE.2/SWE.3) & quality control | ~6 | M-H |
| 6 | Technical lead / Product Owner of Scrum teams | ~6 | H |
| 7 | Sales, marketing & accounting (family import/trading business) | 11 | M |
| 8 | Teaching / explaining (math TA, Ain Shams) | 4 | H |
| 9 | AI agents / LLM tooling for engineering workflows | TBD | TBD |

### Co-founder: Waled Ezz Eldin Ahmed (brother, co-originator of the idea)

From his LinkedIn PDF: Staff (Architect/Lead) Embedded SW Engineer, 12+ years in embedded SW.

| # | Skill | Years | Confidence |
|---|-------|------:|:----------:|
| 1 | Automotive SW architecture & modeling (Enterprise Architect); full ASPICE SWE.2 owner (Luxoft: radar platform, ADAS camera, BookShelf components platform) | ~4 | H |
| 2 | Co-leading SW teams across Communication, Diagnostics, NvM, DLT, Functional Safety | ~4 | H |
| 3 | Change-request & problem analysis (FTA, fishbone) | ~4 | H |
| 4 | Automotive SW design/dev/test, AUTOSAR & non-AUTOSAR, MCAL (Dio 4.3), CAN/LIN/FlexRay/Ethernet, requirements extraction (Avelabs 2017-2022) | ~9.5 | H |
| 5 | System integration & test planning; multicore DSP, RTOS (Axxcelera, LTE) | ~3 | H |
| 6 | Scripting: Python, TCL, shell | 10+ | H |
| 7 | Director of Sales & Marketing, family import/trading business | 13 | H |

**Team note:** Both brothers have worked at Avelabs (Waled 2017-2022), so non-solicit clauses may cover Avelabs customers for both. Natural split: Waled = architecture/design + ASPICE checkpoints (SWE.1-SWE.2, FuSa); Hesham = integration + cybersecurity checkpoints (SWE.3-SWE.5, ISO 21434).

---

## Problems Observed (Tier 1 / OEM side)

| # | Problem | Who Has It? | Pain (1-10) | Category |
|---|---------|-------------|:-----------:|:--------:|
| 1 | Unit/integration test backlogs; ISO 26262 coverage targets (statement/branch/MC/DC) are labor-intensive | Tier 1 SW test managers | 8 | A |
| 2 | ASPICE work products (requirements, architecture, traceability, test specs) consume huge engineering hours | Tier 1 SW project leads, quality managers | 8 | A |
| 3 | Requirements-to-test traceability breaks across tool chains (DOORS/Polarion/Jama to test tools) | Tier 1 / OEM requirements engineers | 7 | A |
| 4 | AUTOSAR Classic BSW/MCAL configuration and integration is slow, error-prone, and expert-scarce | Tier 1 integration teams | 7 | A |
| 5 | MISRA C / static-analysis findings backlogs before release | Tier 1 SW teams | 6 | A |
| 6 | Legacy ECU code migration to new platforms / SDV / zonal architectures | OEMs and Tier 1s | 8 | A/B |
| 7 | Scenario-based virtual validation (SIL/HIL) for ADAS needs thousands of test scenarios | ADAS validation teams | 8 | A |
| 8 | ISO 21434 cybersecurity work products (TARA etc.) and UN R155/R156 evidence | OEM & Tier 1 cybersecurity teams | 7 | A |
| 9 | Engineering service providers are expensive and slow to ramp; offshore rates rising | OEM/Tier 1 procurement & SW managers | 8 | B |
| 10 | Shortage of experienced automotive embedded engineers | Everyone in the chain | 9 | B |

---

## Raw Niche Ideas (Skills x Problems)

| # | Niche idea | For whom? | Excited? |
|---|-----------|-----------|:--------:|
| A | AI-native full-stack automotive SW ESP (founder's original, broad) | Tier 1 / OEM SW departments | Y |
| B | AI-driven unit & integration test generation for safety-critical embedded C (ISO 26262 coverage) | Tier 1 SW test managers | TBD |
| C | ASPICE / ISO 26262 work-product & traceability automation | Tier 1 quality & project leads | TBD |
| D | AUTOSAR Classic configuration & integration accelerator | Tier 1 integration teams | TBD |
| E | Legacy ECU code migration/modernization (to SDV/zonal/AUTOSAR) | OEMs and large Tier 1s | TBD |
| F | ADAS scenario generation for virtual (SIL) validation | ADAS validation teams | TBD |
| G | ISO 21434 cybersecurity work-product automation (TARA) | Cybersecurity leads | TBD |
| H | AI-accelerated cybersecurity BSW integration (HSM, secure boot, SecOC, crypto stack) + ISO 21434 work products -- merge of D + G around founder's strongest skills | Tier 1 SW/cybersecurity leads | TBD |

---

## Summary

- **Raw niche ideas:** 7 (A-G), all slices of the founder's core idea
- **Brought into Phase 2:** all 7, for scoring
