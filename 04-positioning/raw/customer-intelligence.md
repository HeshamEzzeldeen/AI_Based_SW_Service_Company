# Customer Intelligence: AI-native AUTOSAR Classic BSW + cybersecurity ESP (Tier 1 / OEM ECU teams)
Status: COMPLETE. Rounds 1-4 done; 23 of 25 search/fetch calls used.
*Generated: 2026-10-25, Agent A2 (Customer Intelligence)*

> **Evidence warning.** Public sources still contain almost no direct buyer voice from Tier 1 SW department heads or BSW managers. Kununu and Glassdoor turned up no reviews of ESP delivery quality. The search tool does not index LinkedIn posts. NXP, Infineon and ST forums return few HSM integration threads, and fetches of them are blocked. The most useful new sources are:
> - an **intacs-listed assessor event on AI-generated work products (2026-10-23)**
> - a **GlobalLogic CTO post (2026-05)**
> - a **BorgWarner SAE paper (2026-01)**
> - job ads
> - the **KPMG 2026 automotive survey**
>
> Verbatim quotes reused from Phase 3 (forum-mining, review-mining, social-sentiment) are marked "(P3)". Raw notes for each round are in the appendix. Labels: [Data]/[Estimate]/[Opinion], confidence H/M/L.

## Language Map

### How customers describe the problem
**BSW configuration and integration**
- "A single parameter mismatch in memory mapping or network routing can take senior architects weeks to untangle." (GlobalLogic CTO Automotive, 2026-05-21) [Data, H]
- "millions of interdependent XML configuration lines in the Basic Software (BSW) and Runtime Environment (RTE)" (same)
- "a severe bottleneck to Time-to-Market" (same)
- "merging Software Components (SWCs) from multiple suppliers frequently leads to mismatched interfaces and resource conflicts" (same)
- "a single parameter change cascades into hours of rework" / "Knowledge lives in experts' heads." / "CI/CD remains aspirational." (Elektrobit, ~2026-06) (P3)
- "Integration Cycles are more complex due to the high number of modules and the increased number of providers. Therefore the integration in each customer project takes more effort." (Continental B&S paper, date unverified) [Data, M]
- "integration hell" (MONOist #41, 2026-07-16) (P3)
- "getting pin to change state every 10ms is operation for at least a week" / "Slow and painful." (HN, 2026) (P3)
- "observability sucks" / "no one understands it" (HN, 2025-06) (P3)
- In TI's documented setup, the silicon vendor supplies the MCAL, a separate vendor supplies the BSW, and "The customer then does the integration." (TI MCAL integration guide) [Data, H]

**Cybersecurity, R155/21434, HSM**
- "lack of standardized approach to ensure implementation of robust cybersecurity measures during ECU production" (BorgWarner, SAE 2026-26-0628, 2026-01-16) [Data, H]
- "secure flashing at plant", "plant password generation", "securing the debug interface" (same paper; these are the production-side jobs)
- "There are endless issues during the supplier security review." / "There is too much information." (CYMOTIVE, 2022-08, older than 12 months) [Data, M]
- "reports, evidence and artifacts to the OEM in the required format" / "This process takes many months" (same)
- "legal liability of the Tier 1 towards the OEM in case of a major mishap" (same)
- "late discovery of cybersecurity gaps" (GlobalPlatform SESIP deck, 2026-05) [Data, M]
- "some overcomplicated AUTOSAR nightmare that doesn't solve for key provisioning" (HN, 2025-11) (P3)
- "still do it in Excel" (TARA, vendor) / "living document" (itemis) (P3)
- No demo exists for SHE key provisioning with the "EB AUTOSAR stack" (NXP Community) (P3)
- HSM debug and integration need an NDA: "the debugger vendor will first have to ask NDA permissions from Infineon" (Infineon community, 2019, older) [Data, M]

**Process / ASPICE**
- "a byword for paperwork" / "produce documentation, defend it in audits, repeat" (Free Press Journal, 2026-06) (P3)
- "paperwork for the auditor" (LinkedIn snippet) (P3)
- "Why Engineers Have Given Up with ASPICE" (SAE WCX 2026 title) (P3)
- "The delivery processes for OEMs were not standardized" / "poor product quality and faults" from "uncontrolled or late changes in the software, missing integration tests or verification faults" (German Tier 1, UL case study, undated) [Data, M]

### What "better" means to them
- "once you configure the goddamn' modules they do work" (HN, 2025-06). The job is working, configured BSW. (P3)
- "Integration as code" / CI/CD for ECU configuration (EB) (P3)
- "real-time semantic validation engines designed to catch circular dependencies and parameter conflicts" (GlobalLogic, 2026-05) [Data, H]
- "objective, traceable, and reproducible evidence" (AUMOVIO AI & ASPICE webinar, 2025-12, snippet) [Data, M]
- "Repeated 'Best-in-Class' certification by OEMs" / "Successful Automotive SPICE Level 3 assessments" / "Low-friction increase in workforce" (outcomes a German Tier 1 valued, UL) [Data, M]
- "demonstrate ASPICE Level 2 capability on critical processes" (the OEM gate before BEV awards) (P3)
- "faster timelines, and outcome-based pricing" (Bain buyer survey, 2026-04) (P3)
- "deterministic" setups, meaning fixed prompts, data and parameters with versioned outputs (AUMOVIO) [Data, M]

### Words they use to evaluate (incl. AI)
- "is that use controlled?", replacing "did they use AI?" (intacs-listed Gate4SPICE event, Seoul, 2026-10-23) [Data, H]
- "polished output no longer reliably signals process capability" (same)
- "can the author be held accountable" / "real engineering evidence" (same)
- "hallucinations, missing quantities, superficial traceability, IP leakage" (same; the assessor's list of AI risks)
- "human verification & accountability", "tool reliability & control", "confidentiality & IP compliance" (same; the event's four-axis frame)
- "comprehension-testing interview questions" (same; assessors will quiz the named engineer)
- "Someone needs to be held accountable" / "put their careers on the line" / "who's verifying the AI doing the verifying" (HN, 2026-03) (P3)
- "AI is not a shrink-wrapped silver bullet" / "LLM's when fed with too much information are likely to hallucinate" (GlobalLogic) [Data, H]
- "few trust it enough to use it" (Automotive News on the Capgemini survey, where 40% trust AI for development) (P3)
- "liability allocation", a top AI concern for 48% of respondents (Dykema 2026) [Data, M]
- "selective adoption", favoured by 84% of Tier 1s (KPMG 2026) [Data, H]
- "consultants who didn't understand anything ... over sold what it did" (HN) (P3)
- "Each account has its own tools, processes, and expectations" / "onboarding complexity" (Luxoft employee, Glassdoor snippet) (P3)

## Pain Hierarchy
| # | Pain point | Frequency | Severity | Example quote (source) |
|---|---|---|---|---|
| 1 | BSW configuration and integration consume senior experts, and one error costs weeks | Common | Deal-breaker (time to market, SOP) | "A single parameter mismatch ... can take senior architects weeks to untangle." (GlobalLogic, 2026-05) [Data, H] |
| 2 | Seams in a multi-vendor stack: MCAL from the silicon vendor, BSW from Vector/EB/ETAS, SWCs from other suppliers | Common | Frustrating to deal-breaker | "Integration Cycles are more complex due to ... the increased number of providers." (Continental) ; MCU01803 XPath error when running the tresos generator inside DaVinci (Infineon forum, 2021) (P3) ; "The customer then does the integration." (TI) |
| 3 | Security-BSW skills (Csm/CryIf/SecOC/HSM/secure boot) are scarce and senior | Common (every job ad asks for the full stack, 6-11+ years) | Deal-breaker for R155/GB 44495 programmes | "Strong hands-on expertise in AUTOSAR security, SecOC, Adaptive AUTOSAR Crypto, HSM, Secure Boot, and Root of Trust" (Security Lead ad, 2026-08) ; talent shortages hold back digital transformation at 46% of Tier 1s (KPMG 2026) [Data, M/H] |
| 4 | R155/21434 evidence flows down to the Tier 1: required format, months of effort, liability | Common | Deal-breaker (no evidence means no nomination or type approval) | "There are endless issues during the supplier security review." ; "legal liability of the Tier 1 towards the OEM" (CYMOTIVE, 2022, older) [Data, M] |
| 5 | HSM, key provisioning and production security have no standard recipe | Occasional, but every secure ECU hits it | Frustrating; risk late in the programme | "lack of standardized approach ... during ECU production" (BorgWarner SAE, 2026-01) ; no SHE key-provisioning demo with the EB stack (NXP, P3) [Data, H/M] |
| 6 | ASPICE paperwork adds little engineering value but remains a mandatory gate | Common | Frustrating (cannot be dropped) | "produce documentation, defend it in audits, repeat" (P3) ; "Why Engineers Have Given Up with ASPICE" (SAE 2026, P3) |
| 7 | Delivery quality depends on individuals; ramp-up and onboarding cause friction | Occasional | Frustrating | "The delivery processes for OEMs were not standardized" (UL, German Tier 1) ; "onboarding complexity" (Luxoft, P3) [Data, M] |
| 8 | Trust in AI output: accountability, hallucination, IP leakage | Common (as an objection) | Deal-breaker if uncontrolled | "is that use controlled?" ; "IP leakage" (intacs-listed event, 2026-10) ; 40% trust AI for development (Capgemini, P3) |
| 9 | Tool lock-in and opaque licensing | Occasional | Annoying | "the cost of retraining teams, rebuilding test assets, requalifying evidence" (btw.media, P3) |

[Opinion] Pains 1-5 are the wedge. Pains 4 and 5 (R155/GB 44495 evidence and production security) are tied to external, dated deadlines, so they create urgency. Pain 8 is not a pain to solve. It is the gate the offer must pass.

## Jobs to Be Done
### Functional Jobs
- Get the security BSW (Csm/CryIf/Crypto driver/SecOC/KeyM) working on target together with the HSM firmware, secure boot and key provisioning, across the silicon vendor's MCAL and the chosen BSW vendor's stack.
- Hit integration milestones (B/C-sample, SOP) without pulling the 2-3 senior integrators off other programmes.
- Deliver R155/21434 work products (TARA inputs, cybersecurity case, CIA deliverables) to the OEM "in the required format" and pass the supplier security review.
- Pass the ASPICE assessment (L2 now, L3 targeted) on SWE.1-6 with real traceability.
- Close production-side security: secure flashing at the plant, debug interface lock, plant passwords, key injection.
- Absorb peaks in demand without a 3-6 month ESP ramp-up.

### Social Jobs
- Be seen by the OEM as a "Best-in-Class", low-risk supplier: no late cybersecurity findings, no escalations (language from the UL outcome list).
- Show management that AI is in use ("AI-accelerated engineers", VW), but in a controlled way that an assessor accepts.
- For the BSW manager: be the person who unblocked the programme, not the one who brought in an unknown Cairo startup that failed.

### Emotional Jobs
- Relief from depending on one or two people who hold the integration knowledge ("knowledge lives in experts' heads").
- Confidence to sign off, without "putting their career on the line" for artifacts produced by AI or by an outside firm.
- Less anxiety before supplier security reviews, OEM audits and the type-approval deadline.

## Best-Fit Customer Profile
[Opinion, built from the evidence above; validate in Phase 6 interviews]
- **Who:** a BSW/integration manager or SW department head at a mid-size Tier 1 (roughly 1-10 secure ECU programmes a year), or an OEM in-house ECU team, building AUTOSAR Classic ECUs.
- **Predictors of high satisfaction and fast value:**
  1. **Mixed-vendor stack:** a silicon-vendor MCAL (Infineon/NXP/TI/ST, configured in tresos) inside a Vector, EB or ETAS BSW. The TI guide and the Infineon forum both document this seam, and no vendor owns it.
  2. **Dated regulatory trigger:** a programme that must show R155/21434 evidence for OEM type approval, or GB 44495 evidence for China (in force since 2026-01-01), within 6-12 months.
  3. **No in-house HSM or security-BSW expert,** or an overloaded one. Today the gap is often filled with German freelancers on long-term contracts (the pattern shows in gulp.de and freelance.de profiles).
  4. **ASPICE L2/L3 pressure** combined with weak SWE traceability.
  5. **Already buys from best-cost locations** (India, Egypt, Eastern Europe) and is under OEM price pressure (Bertrandt, IAV and KPIT signals, P3). For this buyer, a Cairo delivery base is normal rather than exotic.
- **Who pays without heavy negotiation:** a programme that is late against a fixed SOP or type-approval date, where the alternatives are an expensive German freelancer or a slow ESP ramp-up. A fixed price for a bounded package (security BSW on target plus evidence) fits a project budget better than an FTE line, which procurement cuts first (KPIT, Jul 2026, P3).
- **Who becomes a champion:** the integration lead who gets the senior engineers' time back, and the cybersecurity manager who passes the OEM review without findings.
- **Poor fit:**
  - large Tier 1s with captive centres (Valeo Cairo, Bosch, Continental/Aumovio India) and master ESP contracts
  - OEMs that restrict offshore access to sensitive modules
  - programmes with no deadline

## Switching Triggers
### What triggers a search
- R155/21434 or GB 44495 evidence falls due for an OEM nomination or type approval, or a supplier security review produces findings.
- An integration milestone slips because the senior integrator is the bottleneck ("weeks to untangle").
- The security-BSW engineer leaves, or a job req for "AUTOSAR Security / HSM" stays open.
- A new MCU generation (e.g., TC2xx to TC3xx/TC4xx, or S32K3) breaks reused crypto code ("throughput bottlenecks and IPC deadlocks", a vendor claim on LinkedIn, L).
- The incumbent ESP cuts or rotates staff ("sudden layoffs whenever clients lost", P3), or bills for a ramp-up.
- Procurement pushes to cut ESP rate cards and move to "outcome-based pricing" (Bain, P3).

### What triggers the actual switch
- A bounded, fixed-price pilot on one ECU's security BSW, with a defined acceptance test on target. [Assumption] This matches the "selective adoption" preference in KPMG's data.
- Proof that the AI use is "controlled": versioned prompts and configuration, deterministic validators, a named reviewer for each work product, and engineers ready for comprehension questions (intacs-listed event; AUMOVIO).
- Named senior people with a recognisable track record (Avelabs/Luxoft background) who can sit the assessor interview.
- Evidence formats that drop straight into the OEM's CIA and review templates.

### What prevents switching
- **Supplier qualification:** new-vendor onboarding, purchasing approval, and existing framework contracts with KPIT, LTTS, Bertrandt and others. DATA GAP on the exact steps for a small ESP.
- **TISAX:** development service providers with OEM contact increasingly need a label, and handling OEM data or prototypes needs the Confidentiality label (KPMG, DQS) [Data, H]. Without one, there is no access to OEM ARXML/DBC files.
- **Startup risk:** two founders, no references, and liability for security defects (CYMOTIVE: the Tier 1 is liable to the OEM). Buyers will ask who carries the risk.
- **AI risk:**
  - Compliance with emerging AI laws (49%) and "liability allocation" (48%) are the top AI concerns (Dykema 2026).
  - Only 40% trust AI for development work (Capgemini).
  - OEM data could leak to LLMs (the "IP leakage" risk named at the intacs-listed event).
- **Tool licences and NDAs:** Vector, EB and ETAS licences are quote-based, and HSM firmware and debugging need silicon-vendor NDAs (Infineon forum). The startup may need seats provided by the customer.
- **Incumbent tool AI:** agentic configuration suggestions in Vector DaVinci 6.5 (Dec 2026) may make buyers wait (P3).
- **Cairo perception:** "offshore site which makes it always supplementary part not a fundamental part of the project" (Valeo Egypt, Glassdoor, P3).

## Key Insights for Positioning
1. **Use the assessor's frame, not the AI frame.** The newest assessor language is "is that use controlled?" and "can the author be held accountable". [Data, H source] [Opinion on how to use it] Position the offer as controlled AI with named, accountable engineers, and build in advance what assessors will ask for:
   - versioning of prompts and configuration
   - a named reviewer for each work product
   - engineers ready for comprehension questions
2. **Own the seam nobody owns.** The silicon vendor documents the MCAL, the BSW vendor documents its stack, the HSM firmware has its own documentation, and the docs then say "the customer then does the integration". Cross-vendor integration is the strongest differentiator against Vector's in-tool AI. [Opinion, M]
3. **Lead with the dated trigger.** R155/21434 flow-down and GB 44495 (in force since 2026-01-01) create deadlines. Production security (plant flashing, debug lock, key injection) has "no standardized approach". That gives the wedge an urgency the general "BSW in half the time" promise lacks. [Data H + Opinion]
4. **Mirror the buyer's vocabulary:** "weeks to untangle", "integration hell", "knowledge lives in experts' heads", "supplier security review", "in the required format", "ASPICE Level 2 capability", "Best-in-Class supplier". Avoid "AI-generated code" and "silver bullet".
5. **The competition is freelancers and FTE lines, not only ESPs.** Tier 1s fill security-BSW gaps with long-term German contractors, and job ads ask for 6-11+ years across the full Csm/SecOC/HSM/secure-boot stack. A fixed-price package will be compared with a senior freelancer's day rate. [Data M + Opinion]
6. **Tier 1s are more willing than OEMs to try new technology** (83% vs 43%, KPMG 2026), but they prefer "selective adoption". A one-ECU pilot beats a platform pitch. [Data, H]
7. **TISAX and a clear answer on liability must be in place before the first deal,** not added later. [Data H + Opinion]

## Data Gaps
- DATA GAP: First-person quotes from Tier 1 BSW/SW managers about ESPs and integration effort. LinkedIn is not indexed, and no conference transcripts (Vector Congress, escar) were found. Fill: 10-15 discovery interviews and the founders' own LinkedIn polls.
- DATA GAP: Kununu/Glassdoor views of ESP delivery quality. Nothing new beyond the Phase 3 snippets.
- DATA GAP: The exact wording of Csm/CryIf/HSM errors in vendor community threads. Infineon, NXP and ST forums are poorly indexed and fetches are blocked. Fill: browse the forums manually.
- DATA GAP: Quantified integration effort (person-weeks per ECU, especially for security BSW). Only "weeks to untangle" and anecdotes exist.
- DATA GAP: An official intacs or VDA QMC position on AI-generated evidence. Only one event agenda (Korea, 2026-10-23) and the AUMOVIO webinar were found, and the webinar PDF fetch failed, so it is snippet-only.
- DATA GAP: The exact supplier-qualification steps for a small ESP at German Tier 1s (purchasing, framework contracts, insurance minimums).
- DATA GAP: A measured shortage of AUTOSAR security engineers. Job ads show demanding profiles but not how long vacancies stay open.
- DATA GAP: How Tier 1s are handling GB 44495 in practice.

---
# Appendix: raw notes per round

## Round 1 raw findings
- [Data, H] intacs-listed Gate4SPICE event, Seoul, 2026-10-23 (VWAY, InTaek Kim), "Evaluating AI-Generated Development Work Products":
  - "Generative AI now shapes work products across every phase of the V-model"
  - "polished output no longer reliably signals process capability"
  - "is the artifact real engineering evidence, can the author be held accountable"
  - "the assessment axis has shifted from 'did they use AI?' to 'is that use controlled?'"
  - "are AI-specific risks (hallucinations, missing quantities, superficial traceability, IP leakage) under process control?"
  - four review axes, including "human verification & accountability", "tool reliability & control" and "confidentiality & IP compliance"
  - "a shift toward comprehension-testing interview questions"
  - Source: https://intacs.info/component/rseventspro/event/490-2026-10-23-gate4spice-event-communicating-agreed-work-ai-generated-work-products-onsite-kr
- [Data, M, snippet only; the PDF fetch failed on TLS] AUMOVIO webinar "AI & ASPICE: innovation driver or compliance risk?" (Dec 2025):
  - ASPICE expects "objective, traceable, and reproducible evidence".
  - AI outputs should be version-controlled and linked to the preceding process items, with human oversight for approval.
  - Assessors will likely expect documentation of the tool, configuration, prompts and reviewer.
  - It contrasts deterministic setups (fixed prompts, data and parameters, versioned outputs) with stochastic ones.
  - It lists "assessor interpretation of AI evidence and harmonization" as an open topic.
  - Sources: https://engineering-solutions.aumovio.com/wp-content/uploads/2025/12/AI_ASPICE_WEBINAR.pdf ; https://engineering-solutions.aumovio.com/?p=9773
- [Data, M] Magna Electronics job (undated): "develop AUTOSAR cybersecurity architecture for ADAS ECUs", covering HSM firmware, secure boot, secure storage, SecOC and IPsec on multicore MCU/SoC. https://builtin.com/job/cyber-security-sw-architect/3309508
- [Data, M] Infineon community thread "HSM lock" (2019-09, older than 12 months): "for HSM integration of this kind the debugger vendor will first have to ask NDA permissions from Infineon". HSM work is NDA-gated. https://community.infineon.com/t5/AURIX/HSM-lock/m-p/315572
- [Data, L, vendor marketing on LinkedIn] Reusing TC2xx crypto abstraction code on TC3xx can cause "throughput bottlenecks and IPC deadlocks" (migration pain). Via de.linkedin.com/in/anuprajdubey
- [Data, L] Market report: "shortage of engineers qualified in both embedded systems and cryptographic protocol implementation extends R&D timelines" (no data given). https://markwideresearch.com/cybersecure-vehicle-control-unit-gateway-systems-market
- [Data, M] Flow-down: OEMs require Tier 1 suppliers to be ISO 21434 compliant to support their own R155 compliance (cybersecurity360.it, an Italian consultancy). https://www.cybersecurity360.it/?p=46930
- [Data, M] A UK job ad, "Vehicle Cyber Security Compliance Engineer (UNECE R155)", requires 10+ years of experience. https://www.itjobswatch.co.uk/jv/Multinational-Company/Vehicle-Cyber-Security-Compliance-Engineer-UNECE-R155-Job-Leamington-Spa-Warwickshire-UK-4xjg5p
- Searches that returned no usable buyer voice: LinkedIn on Tier 1 BSW integration bottlenecks; Infineon/NXP/ST threads on Csm/CryIf (the forums are poorly indexed).

## Round 2 raw findings
- [Data, M, 2022-08-29, older than 12 months] CYMOTIVE (Bandel, Bokobza), on OEM-Tier 1 information exchange for R155 (written from the OEM side):
  - The Tier 1 needs "very clear and specific guidelines regarding the proper implementation of the security mechanisms".
  - "Lack of this part of the process can result in legal liability of the Tier 1 towards the OEM in case of a major mishap."
  - "A Tier 1 needs to provide reports, evidence and artifacts to the OEM in the required format"
  - "This process takes many months for successful completion and resources need to be allocated for it."
  - "There are endless issues during the supplier security review."
  - "There is too much information."
  - Source: https://cymotive.com/?p=2033
- [Data, M, 2026-05] GlobalPlatform SESIP procurement deck: repeating bespoke security assessments for each supplier and component is costly and inconsistent. A common supplier pitfall is "late discovery of cybersecurity gaps". https://globalplatform.org/wp-content/uploads/2026/05/15_SESIP-Procurement.pdf
- [Data, M, vendor case study, undated] UL SIS, German Tier 1:
  - Problems: "lacked software experience"; "Software was often not a priority in the company."; "The delivery processes for OEMs were not standardized"; "the company had to face poor product quality and faults" from "uncontrolled or late changes in the software, missing integration tests or verification faults".
  - Outcomes valued: "Repeated 'Best-in-Class' certification by OEMs", "Successful Automotive SPICE Level 3 assessments", "Low-friction increase in workforce by 100% within 1.5 years".
  - Source: https://ul.com/sis/resources/how-to-master-embedded-software
- [Data, M] Continental B&S paper (via Scribd, date unverified): "Some Basic Software modules are taken as off-the-shelf components from internal and external providers. Integration Cycles are more complex due to the high number of modules and the increased number of providers. Therefore the integration in each customer project takes more effort." https://www.scribd.com/document/806684707/Autosar-basic-software
- [Data, M, Japanese trade press, 2015-2016, older] MONOist: integration means reconciling the outputs of separate BSW, system and SW-C teams. Tailoring differs per ECU project, and upstream design changes force repeated rework. https://monoist.itmedia.co.jp/mn/articles/1606/15/news004_2.html
- Job ads (these show the skill profile, not proof of a shortage) [Data, M]:
  - Harman, "Software Engineer Autosar Security and HSM": "Develop and integrate Classic AUTOSAR Security Stack"; "Work with Hardware Security Modules (HSM)". https://jobsearch.harman.com/en_US/careers/JobDetail/Software-Engineer-Autosar-Security-and-HSM/31261
  - "AUTOSAR Security Lead", Bangalore, 2026-08-11, 6-11 years: "Strong hands-on expertise in AUTOSAR security, SecOC, Adaptive AUTOSAR Crypto, HSM, Secure Boot, and Root of Trust". https://www.hirist.tech/j/autosar-security-lead-1662347
  - Antal, "AUTOSAR Cybersecurity": CSM/CRY stacks, HSM firmware, secure boot; "Mandatory Skills: Embedded C, Autosar – BSW, cybersecurity & Automotive domain." https://www.antal.com/job/autosar-cybersecurity-autosar-cybersecurity
  - Magna: "Expert level AUTOSAR experience (MCAL, CAL, CSM, DCM, NVM, DEM, RTE, etc.)". https://themuse.com/jobs/magnainternational/cyber-security-sw-engineer
  - Freelance profiles (gulp.de, freelance.de): German freelancers list work integrating the CSM, Crypto, CryIf and HSM AUTOSAR security modules, and SecOC/FvM feature ownership (search-summary paraphrase). This suggests Tier 1s fill the gap with long-term contractors ("long-term contract basis", freelancermap). No profile or ad mentions KeyM.
- Failed: Kununu (search surfaced no ESP delivery-quality reviews; Kununu does not appear to be indexed for this) and ESP ramp-up frustration interviews (only vendor pages came back).

## Round 3 raw findings
- [Data, H, 2026-05-21] GlobalLogic CTO Automotive (Krzysztof Abramczyk), "Decoding AUTOSAR". This is an ESP's view, but it is the most quotable statement of the buyer's pain:
  - "There are millions of interdependent XML configuration lines in the Basic Software (BSW) and Runtime Environment (RTE)."
  - "A single parameter mismatch in memory mapping or network routing can take senior architects weeks to untangle."
  - "merging Software Components (SWCs) from multiple suppliers frequently leads to mismatched interfaces and resource conflicts"
  - AUTOSAR complexity "has transformed from a structural necessity into a severe bottleneck to Time-to-Market (TTM)"
  - On the limits of AI: "AI is not a shrink-wrapped silver bullet"; "LLM's when fed with too much information are likely to hallucinate".
  - Source: https://www.globallogic.com/insights/blogs/decoding-autosar-ai-workflow-sdv/
- [Data, M] AUTOSAR consortium workflow-improvement survey (the page now returns 404; snippet only): asks users about friction in "working with ARXML, comparing or merging changes, handling tool interoperability, or integrating specifications into AI-supported workflows". The standards body itself acknowledges the pain. https://www.autosar.org/news-events/workflow-improvement-survey
- [Data, H, 2026-01-16] SAE 2026-26-0628, BorgWarner PDS (Kulanthaisamy et al.): "there is a lack of standardized approach to ensure implementation of robust cybersecurity measures during ECU production". Key measures: "activation of cybersecurity protections in production units", "secure flashing at plant", "effective plant password generation", "securing the debug interface". https://saemobilus.sae.org/papers/automotive-cybersecurity-measures-ecu-production-2026-26-0628
- [Data, H] GB 44495-2024 has been in force since 2026-01-01 for M/N/O vehicles with at least one ECU (TÜV SÜD). Korean press (Apr 2025, older) described the industry as "on high alert" ahead of enforcement. https://www.tuvsud.com/en/knowledge-hub/technical-updates/consumer-products-and-retail-essentials/china-implements-vehicle-cybersecurity-technical-requirements
- [Data, H] TISAX:
  - KPMG lists "development service providers, engineering offices and consultancies with OEM contact" among the groups for which a label is increasingly mandatory.
  - The Confidentiality label is needed for handling OEM-sensitive data and prototypes, and OEMs set the required label combination per supplier (DQS).
  - Omnex blog, 2026-01-02: "Why TISAX has become a contract requirement for automotive suppliers".
  - Sources: https://kpmg.com/de/en/services/advisory/consulting/cyber-security/tisax-information-security-for-the-automotive-industry.html ; https://www.dqsglobal.com/en/explore/dqs-knowledge-center/tisax-explained ; https://blog.omnex.com/2026/01/02/why-tisax-has-become-a-contract-requirement-for-automotive-suppliers/
- [Data, L, vendor] PopcornSAR (Korea) markets PAIO as an "AI-native AUTOSAR design tool" (competitor signal). kr.linkedin.com/in/popcornsar

## Round 4 raw findings
- [Data, H, 2026-05] KPMG Global Tech Report 2026, Automotive (n=258):
  - 83% of Tier 1 suppliers are willing to take risks on emerging technology, versus 43% of OEMs.
  - 84% of Tier 1s favour "selective adoption".
  - Talent shortages restrict digital transformation for 46% of Tier 1s (38% of OEMs).
  - Source: https://assets.kpmg.com/content/dam/kpmgsites/xx/pdf/2026/05/global-tech-report-2026-automotive.pdf (via the autocarpro.in summary)
- [Data, M, 2026] Dykema 2026 Automotive Trends: the top AI concerns are compliance with emerging AI laws (49%) and "liability allocation" (48%). https://www.dykema.com/2026-Automotive-Trends-Report/artificial-intelligence.html
- [Data, H] TI MCAL integration guide: the silicon vendor ships the MCAL and the EB configurator, the BSW/RTE comes from "their chosen vendor", and "The customer then does the integration". Importing the MCAL into another vendor's tool (DaVinci) needs an ARXML export, a vendor module definition and a BSWMD file for each module. This documents the mixed-vendor integration seam. https://software-dl.ti.com/mcu-plus-sdk/esd/PLATFORM_SW_MCAL/AM263P/latest/src/Integration.html
