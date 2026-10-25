# Founder Input: Unique Attributes (Phase 4, Component 2)
*Recorded 2026-10-25 from the founders' LinkedIn profile exports (shared in session) and Hesham's reply.*

Status: COMPLETE. Founder statement: "if any missing experience we will hire the needed expert."
Founders did not answer the guarantee question (attribute 3) or the narrow-entry question explicitly. Defaults used: the narrow entry follows the Phase 2 decision (H is the first offer inside I); the guarantee is left to Phase 5 (offer design) and is not claimed in positioning.

## Hesham Ezz Eldeen: what the profile shows [Data, founder-supplied, H]
- About 10 years in embedded SW; 9.5 years at Avelabs (May 2017 to now); now Staff II Embedded SW Engineer and Cyber Security Architect.
- **Certification:** Vector Certified Embedded Professional, AUTOSAR Classic - Security.
- **Listed top skills:** SM2, Chinese crypto algorithms, ETAS.
- Projects (client names are Avelabs' customers; see the confidentiality flag below):
  | Period | ECU / programme | Role and scope | Stack / target |
  |---|---|---|---|
  | Jul 2025 - now | EPWT ECU (customer "Hande") | Cyber security architect: reviews customer security requirements; writes requirements to ETAS for HSM features; owns SWE.2 design of secure flashing, secure boot, secure diagnostics, secure logging, secure storage, secure debugging; supports SWE.3; supports HSM integration in bootloader and host | ETAS HSM |
  | Apr 2023 - Jun 2025 | US OEM fuel-cell inverter ECU via a Tier 1 | BSW technical lead: ETAS stack configuration and integration (COM, Diag, NvM, partial networking, mode management, OS, RTE); OEM security requirements (ETAS HSM, secure boot, message authentication, secure diagnostics, secure flashing); ETAS bootloader; CDDs; FuSa support | ETAS RTA stack + ETAS HSM + ETAS bootloader |
  | Nov 2022 - Mar 2023 | German OEM lidar ECU via a Tier 1 | Bootloader integration, secure boot design, DoIP configuration | n/a |
  | Jun 2022 - Nov 2022 | UK luxury OEM car-gate ECU | Technical SW lead for HSM integration and security AUTOSAR configuration: HSM updater, secure boot, crypto stack | Vector MICROSAR, Infineon TRAVEO, IAR, Ozone |
  | Sep 2021 - May 2022 | US OEM ADAS ECU | Technical lead, secure boot: host bootloader to HSM communication, crypto stack, HSM integration, secure boot for OTA, HSM updater | Vector MICROSAR, Infineon AURIX TC3xx, Tasking, Lauterbach |
  | Apr 2021 - Sep 2021 | same ADAS ECU | Product owner, CAN message authentication team: crypto stack, SecOC, FVM, KeyM integration, HSM configuration | Vector MICROSAR, AURIX TC3xx |
  | 2017 - 2021 | same ADAS ECU | Led diagnostics (DEM/DCM, UDS), AUTOSAR integration (COM, DBC, Ethernet, XCP, RTE), communication team (NvM, CDDs, power modes); ASPICE quality control of team work | Vector MICROSAR, AURIX TC3xx |

## Waled Ezz Eldin Ahmed: what the profile shows [Data, founder-supplied, H]
- 12+ years embedded (automotive since 2017, telecom before); now Architect / Principal Embedded SW Engineer at Luxoft Egypt (Oct 2022 to now).
- Luxoft: radar platform, camera-based ADAS project, a components platform. SW architecture design and modelling (Enterprise Architect); design-concept documents; co-leads the SW team (Communication, Diagnostics, NvM, DLT, Functional Safety); **complete ASPICE SWE.2 owner**; change-request and problem analysis (FTA, fishbone).
- Avelabs 2017-2022 (5 yrs 8 mo): AUTOSAR 4.3 DIO (MCAL) module implementation; CAN, LIN, FlexRay, Ethernet; AUTOSAR and non-AUTOSAR products across design, development and test.
- Telecom 2014-2017: system integration engineer (1.5 yrs), multicore DSP, RTOS.

## Both
- 11-14 years of sales, marketing and accounting in the family trading business before engineering [Data, founder-supplied]. This is relevant to founder-led selling, not to positioning.

## Mapping to the proposed unique attributes
| # | Attribute | Status today | Basis |
|---|---|---|---|
| 1 | Cross-vendor integration | **Partly proven.** Shipped on **Vector MICROSAR and ETAS RTA** stacks, **ETAS HSM**, Infineon **AURIX TC3xx and TRAVEO** (ETAS programmes on AURIX, confirmed by Hesham 2026-10-25). Not shown: EB tresos, NXP HSE, Renesas ICU-M, AURIX TC4x CSRM | Hesham's projects |
| 2 | Security BSW on target | **Proven.** Crypto stack, SecOC, FVM, KeyM, HSM integration and HSM updater, secure boot (incl. OTA), secure flashing, secure diagnostics; SWE.2 for secure logging, storage, debugging. Key provisioning at end-of-line: not stated | Hesham's projects |
| 3 | Evidence included (+ guarantee) | **Skills proven, offer not designed.** Waled owns ASPICE SWE.2; Hesham did SWE.2/SWE.3 security design and ASPICE quality control. No 21434 cybersecurity-case or TARA authorship listed. Guarantee: not answered (Phase 5). **Founder decision 2026-10-25: keep "21434 evidence included" and add a named 21434/TARA hire or partner** | Both profiles + founder answer |
| 4 | Assessor-controlled AI | **Not built.** Aspirational until the harness and provenance log exist | n/a |
| 5 | Named, accountable reviewers | **Proven people, ready to name.** Two senior engineers with 10-12+ years | Both profiles |
| 6 | Published accuracy metrics | **Not built.** Needs the benchmark | n/a |
| 7 | Fixed price + AI pass-through | **Business-model choice,** not a capability. Fixed price alone is table stakes (KPIT) | Phase 3/4 research |

**Additional attribute found in the profiles:** SM2 / Chinese crypto algorithms listed as a top skill. China's GB 44495 applies to all existing vehicle types from 1 Jan 2028, and Chinese programmes commonly require SM2/SM3/SM4 support in the crypto stack [Opinion, M; the SM-algorithm requirement was not verified this phase]. This is a rare, relevant skill for the carry-over retrofit trigger.

**On "we will hire experts for missing areas":** hiring is a valid plan, but under the no-aspirational-positioning rule a stack or MCU family goes into the positioning only after the team has delivered on it. First hires that would widen attribute 1 the most: EB tresos + NXP S32K3/S32G HSE, and Renesas RH850 ICU-M / AURIX TC4x CSRM.

## Flags raised by this input
- **Red: client names.** The named OEMs and Tier 1s are Avelabs' and Luxoft's customers. Naming them in marketing, or approaching them, may breach NDA and non-solicit clauses. Positioning uses anonymised descriptions ("US OEM ADAS ECU") until legal review.
- **Yellow: individual vs company track record.** The experience belongs to the founders as employees, not to the new company. Buyers and assessors will credit the people, but supplier qualification asks for company references.
