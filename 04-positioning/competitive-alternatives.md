# Competitive Alternatives Map: AI-native AUTOSAR security integration (Cairo)
*Skill: sk-positioning | Generated: 2026-10-25 | Mode: Deep*

*Source: `raw/alternative-mapping.md` (A1, 12 alternatives with full detail and URLs), `raw/fescaro-check.md`, Phase 3 battle cards. Labels: [Data]/[Estimate]/[Opinion], H/M/L. Switching-cost ratings are [Opinion, M].*

## The Job to Be Done
"Get this ECU's security software configured, integrated and working on our target MCU, with the evidence our OEM and the assessor will accept, by the SOP or type-approval date, without blowing headcount or budget." [Opinion, M; reconstructed from A1/A2]

It has four parts that buyers often hire different alternatives for: (1) configure and integrate the BSW on the chosen stack; (2) make the ECU secure across stack and silicon (Csm/CryIf, SecOC, KeyM, HSM, secure boot, key provisioning); (3) produce ASPICE and ISO 21434 evidence; (4) absorb the pre-SOP peak. The buyer wants a **secured, evidenced ECU baseline on time, and someone accountable if it is wrong**, not "AI" and not hours.

## Direct Competitors
| Alternative | Hired for | Strengths | Shortcomings | Switching triggers |
|---|---|---|---|---|
| **Stack vendor services** (Vector, ETAS/ESCRYPT, EB) | Security + stack integration on their own stack | Own the code and HSM firmware; "nobody gets fired for calling Vector"; Vector agentic configuration [Data, H] | Single-stack; premium German rates; queues; Vector AI messaging silent on security [Data/Opinion, M] | Queue too long for SOP; mixed-vendor seam nobody owns; consultant price |
| **Large ESPs** (KPIT, Tata Elxsi, LTTS, Capgemini, DXC/Luxoft) | Programme-scale integration; fixed-price work packages | Scale, approved status, TISAX; KPIT 68% fixed price + AI; ISG Leaders [Data, H] | Small security packages below threshold; AI gains kept as margin; no published AI metrics [Opinion, M] | Ramp-up delays; attrition of named engineers; rate pressure |
| **Security product vendors with services** (FESCARO, Autocrypt, wolfSSL) | Their own HSM firmware + engineering + TARA | Integrated product + service; FESCARO 150+ ECUs, operating profit four years running [Data, H]; KOSDAQ-listed Dec 2025 [Data, M] | Integrate their own products, not the customer's chosen stack; FESCARO Korea-centric, no fixed price seen [Data/Estimate, M] | Customer already standardised on Vector/ETAS HSM |
| **Cairo ESPs** (Avelabs/Arrow, Swift Act, Brightskies) | Low-cost AUTOSAR + 21434 capacity | Same Cairo cost and talent; Arrow channel [Data, M] | T&M; no AI story [Data, M] | Need for fixed price or faster calendar |
| **AI-TARA / compliance tools** (ThreatZ/VxLabs, Ketryx, C2A) | 21434 documents faster | 70-90% claimed doc savings (unaudited) [Data, M] | No implementation [Data, M] | Documents don't close the implementation gap |

## Adjacent Alternatives
| Alternative | Hired for | Strengths | Shortcomings | Switching triggers |
|---|---|---|---|---|
| **Senior security freelancer** (GULP, Hays, freelancermap) | A named skill gap for 6-12 months | Fast; EUR 85-120/h (≈EUR 14-19k/month at 160 h) [Data, M; Estimate, M]; real SecOC/HSM supply | Sells hours, not an outcome or evidence; knowledge leaves; scarce ("rate on request"); AÜG risk [Data/Opinion, M] | Freelancer leaves mid-project; unavailable at crunch; procurement blocks direct freelancers |
| **Body leasing** (Akkodis, Alten, Ferchau, Bertrandt) | Onsite capacity under frame contracts | On approved lists; proximity [Data, M] | German cost; distressed; quality depends on the person [Data, M] | Frame renewal; cost-cutting rounds |
| **Captive centres** (Valeo Cairo, BGSW, AUMOVIO RO/IN) | Same job at cost | Same cost base; IP inside; hold the licences [Data, H] | Booked through SOP; being cut; security experts at HQ [Data, H] | Hiring freeze + SOP crunch; new MCU family the captive hasn't done |
| **MCU vendor reference SW** (Infineon, NXP, Renesas) | Security bring-up on the silicon | Free, silicon-exact [Data, M-H] | Reference ≠ production; NDA docs; no evidence [Data, M] | Demo works, production integration doesn't |
| **DIY: coding agents + Vector MCP / PAIO** | Speed up the internal team | Already licensed; cheapest marginal cost [Data, H] | 10-19% gains; no controlled-AI evidence; little security training data [Data, H; Opinion, M] | Assessor asks "how is AI use controlled?"; agent-generated config causes a late bug |

## Manual / Status Quo
| Alternative | Hired for | Strengths | Shortcomings | Switching triggers |
|---|---|---|---|---|
| **Work harder / slip** | Avoid spend and supplier onboarding | No PO, no 6-18-month onboarding [Estimate, M] | "Weeks to untangle" one mismatch; expert burn-out [Data, H] | OEM escalation; missed sample milestone; the one expert leaves |
| **Cut or defer security scope** | Protect the SOP date | Saves time now | R155 / GB 44495 flow-down makes it contractual; VW/Porsche dropped models rather than re-engineer (Apr 2024) [Data, H, >12 mo] | OEM RFQ makes SecOC/secure boot mandatory; China market entry |
| **Accept the audit finding** | Keep shipping | ASPICE is not pass/fail; findings are survivable [Data, M] | Hits supplier rating and sourcing; claimed type-approval delays [Data, L] | A finding that blocks a nomination |

## Your Unique Attributes vs. Each Alternative
*A = security BSW on target; B = works on the customer's stack (Vector + ETAS on Infineon today); C = evidence included; D = named engineers sign; F/G = controlled AI / published metrics (to build).*

| Alternative | What they offer | Where [Company] wins | Where they win |
|---|---|---|---|
| Security freelancer | One expert's hours | C, D, fixed-scope outcome, no knowledge walk-out | Trust in "our" person; onsite; no supplier qualification |
| Stack vendor services | Deep stack knowledge, own HSM | B (seam across vendors), price, availability | Code ownership, defect fixes, brand safety |
| Large ESPs | Scale, approval, fixed price | Small-package fit; C + D bundled; F/G once built; AI pass-through | Approved-supplier status, TISAX, references, scale |
| FESCARO / product vendors | Own HSM + services | B (customer's chosen stack), EU focus, ASPICE SWE evidence | Product IP, 150+ ECU references, company track record |
| Cairo ESPs | Cost + capacity | Fixed-price package; C + D; AI leverage | Company history, Arrow channel, headcount |
| AI-TARA tools | Documents | A (implementation on target) | Price per seat, speed on documents |
| Captive centre | Same job internally | Flex for peaks; security specialism | Politics, IP inside, licences |
| DIY with agents | Internal speed-up | Security depth; C + D; F once built | Cost, control, "we built it" |
| MCU reference SW | Free bring-up | Production-grade integration + evidence | Free |
| Status quo (work harder / defer / accept finding) | No spend | Deadline met, finding avoided | Zero procurement effort |

## Switching Cost Analysis
| Alternative | Technical | Contractual | Emotional | Net switching barrier |
|---|---|---|---|---|
| Security freelancer | L | L | L-M | **Low: first displacement target** |
| Status quo: work harder | L | L | M | Low-Medium (admitting the team can't make it) |
| Status quo: defer scope / accept finding | L | L | L-M | Low once a deadline bites |
| MCU reference SW | L | L | L | Low (complement, not rival) |
| Captive centre | L | L | **H** | Medium (politics: pitch overflow, never replacement) |
| DIY with agents | L-M | L | M-H | Medium (sell the evidence layer to them instead) |
| Body leasing | L-M | M-H | M | Medium |
| Cairo ESPs | M | M | L-M | Medium |
| AI-TARA tools | M | M | L | Medium (partner: TARA feeds implementation) |
| FESCARO / product vendors | M-H | M | M | Medium-High where their HSM is already chosen |
| Large ESPs | M | H | M | High (MSAs; go in as subcontractor) |
| Stack vendor services | H | H | H | High (go in on top of their stack, not against it) |

## Key Positioning Insights
1. **Position against the freelancer and the status quo first.** They have the lowest switching barriers, and the freelancer cannot sell an outcome, evidence or accountability [Opinion, M].
2. **Nobody owns the seam.** MCU vendors pass integration to stack partners, stack and HSM vendors cover only their own products, freelancers cover only themselves [Data, M + Opinion, M]. That seam is the position.
3. **Ride on the stack vendors, don't fight them.** Their switching barriers are High on all three axes; their AI makes configuration cheaper, which helps a package seller [Opinion, M].
4. **Large ESPs and staffing firms are the first channel,** not the first enemy: they hold approval and TISAX, and small security packages fall below their threshold [Opinion, M].
5. **The 2026 cost cuts are a switching trigger:** headcount freezes with fixed SOPs favour outcome-priced packages [Data, H + Opinion, M].

## Red Flags
- FESCARO shows that bundled "security implementation + compliance" exists; the founders' claim is narrower (customer's stack, fixed price, ASPICE + 21434 evidence). Keep the wording precise [Data, M].
- Against every direct competitor, the founders lose on company track record, approval and TISAX today [Opinion, H].

## Yellow Flags
- DIY with agents rises to a High threat by 2027-28 (Phase 3) [Opinion, M].
- Freelancer security rates are a third-party estimate (EUR 120-180/h, L); real rates are "on request".
- How often buyers choose each alternative is inferred, not measured.

## Data Gaps
- Freelancer rates specific to AUTOSAR security (profiles say "auf Anfrage"); 2026 billing rates for Akkodis, Alten, Ferchau, Bertrandt.
- Vector/EB/ETAS professional-services day rates and lead times.
- Captive-centre internal transfer rates.
- No named SOP slip caused by BSW/security integration; no public switching stories.
- FESCARO's MCU/stack support list and whether it integrates third-party AUTOSAR security BSW.
- No first-hand reports of coding agents on BSW/ARXML.

## Sources
- `raw/alternative-mapping.md` (full per-alternative detail and URLs, 2026-10-25); `raw/fescaro-check.md`; Phase 3 battle cards in `../03-competitors/battle-cards/`.
- Key: AUMOVIO R&D cuts (S&P AutoTechInsight) https://autotechinsight.spglobal.com/news/5286328/aumovio-plans-strategic-realignment-of-global-r-d-activities-move-to-result-in-loss-of-4000-jobs ; freelancer rates https://www.freelancermap.de/blog/stundensatz-it-freelancer/ ; NXP HSE forum https://community.nxp.com/t5/S32K/Support-Request-for-HSE-Firmware-Installation-Secure-Key-Storage/td-p/2181791 ; VW/Porsche R155 (Fortune, Apr 2024) https://www.fortune.com/europe/2024/04/16/volkswagen-porsche-killing-old-models-new-eu-cybersecurity-rules-opportunity-for-chinese-rival-byd
