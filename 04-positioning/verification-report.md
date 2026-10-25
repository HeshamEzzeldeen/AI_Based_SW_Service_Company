# Verification Report: AI-native AUTOSAR security integration (sk-positioning, Deep)
*Generated: 2026-10-25 | Agent: V1*

Scope: `04-positioning.md`, `positioning-doc.md`, `positioning-statement.md`, `competitive-alternatives.md`, `market-category-analysis.md`, `messaging-implications.md`, checked against `raw/` (7 files) and `03-competitors.md`. No web research; raw files were not edited.

## Summary
- **Critical issues:** 1 (partly mitigated by added flags; open for a founder decision)
- **Warnings:** 11 (9 fixed, 2 open)
- **Info:** 10 (3 fixed, 7 notes)

Verdict: the numbers carried into the deliverables match the raw files. The main problem is founder-capability claims. Strategy, category, themes, best-fit profile and tagline are consistent across all files.

---

## Critical Issues

### C1. "ISO 21434 evidence included" goes beyond the founders' documented record
- **File(s):** all six deliverables (Moore, Onliness, elevator pitch, one-liners, Theme 2, messaging hierarchy item 5, attribute C)
- **Section:** positioning-doc Component 2 (attribute C), positioning-statement (all statements), messaging-implications (hierarchy item 5)
- **Problem:** `founder-input.md` says: "No 21434 cybersecurity-case or TARA authorship listed." The documented evidence work is ASPICE SWE.2 (Waled) and SWE.2/SWE.3 security design plus ASPICE quality control (Hesham). Even so, every buyer-facing statement promises "ISO 21434 ... evidence included", and the messaging adds "ASPICE SWE / SEC.1-4 evidence". Neither founder profile shows SEC.1-4 or SWE.1/SWE.4-6 ownership. No deliverable flagged this gap, although the same type of gap (end-of-line key provisioning) was flagged. "Evidence included" is a core differentiator and appears in the tagline, so this could mislead the positioning decision.
- **Fix applied (mechanical):** added the gap to the evidence column of attribute C and a Red Flag in `positioning-doc.md`. Added it to Key Flags (Red) in `04-positioning.md`, to Yellow Flags in `positioning-statement.md`, and to the new Yellow Flags section in `messaging-implications.md`.
- **Open, founder decision needed:** (a) confirm whether either founder has authored 21434 work products (TARA, cybersecurity case, CIA deliverables) that the profiles leave out; or (b) narrow the claim to "ASPICE SWE evidence plus the 21434 implementation-level work products traced to it" until a hire or partner covers TARA and the cybersecurity case; or (c) name the hire or partner in the offer. Wording in the Moore and Onliness statements was not changed, because it is a strategic choice.

---

## Warnings

### W1. "Vector and ETAS on Infineon" is not fully documented (OPEN)
- **File(s):** all deliverables
- **Problem:** in `founder-input.md` the Infineon projects (AURIX TC3xx, TRAVEO) are all on Vector MICROSAR. The two ETAS programmes (fuel-cell inverter; EPWT with ETAS HSM) have no target MCU listed. So "proven: Vector MICROSAR and ETAS RTA on AURIX TC3xx / TRAVEO" was an inference.
- **Fixed:** the "proven/delivered" statements now separate the two: attribute B in positioning-doc, the scope line in the positioning-statement header, and Value Theme 1 in the summary. A Data Gap was added to four files.
- **Still open:** the scope shorthand "Vector and ETAS on Infineon" remains in the Onliness condition, the validation notes, the competitive-alternatives legend, best-fit item 2, messaging hierarchy item 3 and summary Decisions. It also remains in the **buyer-facing** Infineon/ESP partner-directory one-liner ("on AURIX and TRAVEO (Vector MICROSAR, ETAS RTA) ... secure flashing"); secure flashing was done on the ETAS programme. **Recommendation:** ask Hesham for the MCU of the ETAS programmes, then either keep the wording or change it to "Vector MICROSAR on AURIX/TRAVEO; ETAS RTA + ETAS HSM".

### W2. Attribute A put all 5 programmes on AURIX/TRAVEO (FIXED)
- **File:** positioning-doc.md, attribute A
- **Problem:** "5 security programmes 2021-2026 on AURIX TC3xx and TRAVEO". Only 2 of the 5 programmes list an MCU.
- **Fix:** "(target MCU stated for two: AURIX TC3xx and TRAVEO)". The count of 5 is correct: ADAS, car-gate, lidar, fuel-cell inverter, EPWT.

### W3. Controlled AI was described as existing in the executive summary (FIXED)
- **File:** positioning-doc.md, Executive Summary item 1
- **Problem:** "AI agents do the bulk of the work under controls built to the questions assessors now ask" is present tense. Attribute F is "Not built" (founder-input).
- **Fix:** reworded as a plan, with an [Assumption] label. The other F/G mentions are already gated correctly ("proof point to build", "only once F exists", and the elevator-pitch note). The investor one-liner ("AI-produced") was flagged as a Yellow Flag in positioning-statement.md. It is not buyer-facing, but it should be presented as the model being built.

### W4. Attribute D's sign-off split read as past experience (FIXED)
- **File:** positioning-doc.md, attribute D
- **Problem:** "Waled: SWE.1-2, FuSa; Hesham: SWE.3-5, 21434" was presented as profile evidence. The profiles show Waled as SWE.2 owner (co-leading a team that includes FuSa) and Hesham on SWE.2/SWE.3 plus FuSa support. They show no SWE.1, SWE.4-5 or 21434 authorship.
- **Fix:** labelled "proposed split, not past roles", with the unproven part marked [Assumption].

### W5. The Moore target did not use the exact best-fit profile and the stack was unscoped (FIXED)
- **File(s):** positioning-statement.md, 04-positioning.md
- **Problem:** the target was "Tier 1 suppliers"; best-fit (Component 4) says "mid-size Tier 1". "On your existing vendor stack" contradicts the words-to-use rule ("on your Vector or ETAS stack", not "any stack") and the Onliness condition "must be scoped in copy".
- **Fix:** "mid-size Tier 1 suppliers" and "on your existing Vector or ETAS stack" in both files. The Onliness stress-test *draft* in positioning-doc was left as the draft it is.

### W6. The elevator pitch named a "gateway" ECU (FIXED)
- **File(s):** positioning-statement.md, 04-positioning.md
- **Problem:** founder-input lists a "car-gate ECU", not a gateway. "Gateway" implies a different, network-security-heavy ECU class.
- **Fix:** "ADAS, inverter and lidar ECUs". All three are documented security work (secure boot/SecOC; ETAS HSM security; secure boot design).

### W7. "Job ads and RFQs" language claim (FIXED)
- **File(s):** positioning-doc.md §5, market-category-analysis.md Implementation
- **Problem:** B1 states that no public RFQ documents were found. The vocabulary comes from job ads and freelance listings.
- **Fix:** reworded to "job ads and freelance project listings", with the note that no RFQs were found.

### W8. Required sections were missing (FIXED)
- **Problem / fix:**
  - positioning-statement.md had no Data Gaps section (added).
  - competitive-alternatives.md had no Data Gaps section (added, drawn from A1 and FESCARO gaps).
  - messaging-implications.md had no Yellow Flags or Data Gaps (both added).
  - 04-positioning.md had no Data Gaps or Sources (both added). Its "verification pending" line was updated.
  - All files now have Red Flags, Yellow Flags (Key Flags in the summary), Data Gaps and Sources.

### W9. Value-anchor arithmetic (FIXED)
- **File:** messaging-implications.md
- **Problem:** "EUR 95/h (80-120), about EUR 14-19k per month at 160 h" does not compute: 80 × 160 = 12.8k. A1 derives 14-19k from EUR 85-120/h.
- **Fix:** states the EUR 85-120/h basis explicitly and labels the security-rate figure as a third-party estimate.

### W10. Homepage count "5 of 9" vs raw "five of eleven" (FIXED by clarification)
- **File(s):** positioning-doc.md, market-category-analysis.md, messaging-implications.md, 04-positioning.md
- **Problem:** A3 Insight 1 says "Five of eleven competitors" and its table-stakes header says "11 homepage fetches". A3's own source list, however, shows 9 homepages fetched (VxLabs failed on DNS; the Cairo row is not a homepage). All five named firms are among those 9. "5 of 9 homepages" is therefore the defensible figure, and the inconsistency is in the raw file.
- **Fix:** kept "5 of 9" and added the reconciliation note in positioning-doc Component 2. The raw file was not edited.

### W11. The Onliness "Pass with conditions" leaves out one condition (OPEN)
- **File(s):** positioning-doc.md (stress test), positioning-statement.md (validation notes), 04-positioning.md
- **Problem:** the competitive part of the verdict holds. FESCARO, Vector, ETAS and Autocrypt bundle their own products, and eInfochips integrates on T&M without packaged evidence (fescaro-check). "We know of" is a hedge, but it is declared as a condition, which is acceptable. However, the "only" statement depends on "ISO 21434 / ASPICE evidence", and that is not fully within the founders' record (C1). The listed conditions (scope stacks; "we found"; build F/G) do not include it.
- **Recommendation:** add a fourth condition, "21434 evidence capability confirmed or covered by a hire/partner", or narrow the statement per C1. This was left to the orchestrator/founders because it changes a validation verdict.

---

## Info
- **Fixed:** CYMOTIVE (2022) citations in positioning-doc now carry ">12 mo". The VW/Porsche (Apr 2024) citation was already flagged.
- **Fixed:** the FESCARO strengths label in competitive-alternatives was split. 150+ ECUs and four profitable years are [Data, H]; the KOSDAQ listing (Dec 2025) is [Data, M], per fescaro-check.
- **Fixed:** the India rate "USD 25-45/h" in market-category-analysis was unlabeled. It is now labelled [Estimate, L-M; Phase 3], where it is marked unverified.
- **Numbers verified as matching the raw files:**
  - AUMOVIO −4,000 R&D roles, <10% R&D/sales; Bosch −13,000 (A1).
  - KPMG 84% "selective adoption" (A2).
  - Capgemini: 5% mature governance, 40% trust for development, 68% use/pilot agentic AI; 10-19% gains (B2/A1/Phase 3).
  - KPIT 68% fixed price (68.3% Q4 FY26).
  - GB 44495: new types 1 Jan 2026, all types 1 Jan 2028 (TÜV SÜD via B2).
  - Market sizes: IMARC USD 150.7B, Everest USD 240-260B, auto cyber USD 3.9-6.9B at 15-20%, AUTOSAR USD 3.5-7.9B (B1).
  - Freelancer EUR 85-120/h and EUR 14-19k/month (A1).
  - "2.5-3x productivity vs 10-19%" (Phase 3).
- **Consistent across all files:** the category label ("AUTOSAR security integration"; "Secure ECU package" as the Phase 5 offer name), the three value themes, the best-fit profile (after W5), the tagline ("Your ECU's security stack, working on target. Evidence included."), the investor frame, freemium = N/A, and the overall strength = Moderate.
- **Mental Ladder:** the ten-word form is exactly 10 words; Pass holds. **Moore:** Pass holds after W5. "Need" and "target" are inferred and are declared as such.
- **Single-source stats:** the Capgemini Oct 2026 survey supplies three separate statistics (5%, 40%, 68%). They are not presented as independent corroboration, so no duplicate-source issue.
- **Label drift:** the 6-18-month onboarding figure is [Estimate, M] in the deliverables but [Estimate, L-M] in Phase 3. Minor.
- **Alternative count:** "12 alternatives" in positioning-doc counts A1's 12. FESCARO/product vendors make it 13 in competitive-alternatives (13 rows). Cosmetic.
- **Value anchor:** it uses general DACH freelancer rates (EUR 85-120/h) for a "senior security freelancer", whose rates are "on request" and estimated at EUR 120-180/h (L). The anchor is therefore conservative; it is flagged in messaging Yellow Flags.
- **File titles:** the deliverable titles say "AI-native AUTOSAR security integration", while the positioning says not to lead with "AI-native". This is acceptable as an internal project name; drop it at Phase 5 naming.

## Verification Checklist
- [x] All quantitative claims labeled (after fixes)
- [x] No internal contradictions found (after fixes; W1 scope wording pending founder confirmation)
- [x] Confidence ratings consistent with evidence
- [x] Data gaps declared in all deliverables (after fixes)
- [x] Red/Yellow flags present in all deliverables (after fixes)
- [x] No stale data unmarked (after fixes)
- [x] No duplicate-source false corroboration
- [ ] Positioning statements match research data: open on C1 (21434) and W1 (ETAS MCU)
- [x] JTBD consistent with customer intelligence
- [x] Cross-deliverable coherence verified
- [ ] Validation tests genuinely pass: Onliness is conditional on C1 (W11)

## Fix Log
| # | File | Change |
|---|---|---|
| 1 | positioning-doc.md | Exec summary: controlled-AI sentence reworded as a plan [Assumption] |
| 2 | positioning-doc.md | Attr A: MCU stated for two of five programmes |
| 3 | positioning-doc.md | Attr B: Vector on AURIX/TRAVEO; ETAS RTA + ETAS HSM, MCU not stated |
| 4 | positioning-doc.md | Attr C: added the SWE.1/4-6, 21434 and SEC.1-4 gap |
| 5 | positioning-doc.md | Attr D: "proposed split, not past roles" + [Assumption] |
| 6 | positioning-doc.md | "5 of 9" reconciliation note vs A3 "five of eleven" |
| 7 | positioning-doc.md | CYMOTIVE ">12 mo" (2 places) |
| 8 | positioning-doc.md | "job ads and RFQs" → "job ads and freelance project listings" |
| 9 | positioning-doc.md | Red Flag added (21434/SEC.1-4); Data Gap added (ETAS MCU) |
| 10 | positioning-statement.md | Header scope line corrected (ETAS MCU) |
| 11 | positioning-statement.md | Moore: "mid-size Tier 1", "existing Vector or ETAS stack" |
| 12 | positioning-statement.md | Pitch: "gateway" → "lidar" |
| 13 | positioning-statement.md | Yellow Flags (+2) and Data Gaps section added |
| 14 | competitive-alternatives.md | FESCARO label split; Data Gaps section added |
| 15 | market-category-analysis.md | RFQ wording; India rate labelled |
| 16 | messaging-implications.md | Value-anchor arithmetic; Yellow Flags and Data Gaps added |
| 17 | 04-positioning.md | Moore (mid-size, Vector or ETAS); Theme 1 proven scope; pitch "lidar"; Red flag 21434; Data Gaps + Sources; verification link |

---

## Resolution (orchestrator, 2026-10-25, after founder input)
- **C1 → Resolved by founder decision.** Hesham chose to keep "ISO 21434 evidence included" and add a named 21434/TARA hire or partner. Every deliverable now marks the 21434 claim as conditional, and written copy says "ASPICE evidence" until the hire or partner is in place. Files updated: 04-positioning.md, positioning-doc.md (attribute C, Red Flag, Onliness Challenge 5 + verdict), positioning-statement.md, messaging-implications.md, raw/founder-input.md.
- **W1 → Resolved.** Hesham confirmed the ETAS RTA / ETAS HSM programmes ran on Infineon AURIX, so "Vector and ETAS on Infineon" is documented.
- **W11 → Resolved.** A fourth Onliness condition was added: claim 21434 evidence in writing only after the hire or partner is in place.
- **Final status:** 0 Critical open, 0 Warnings open.
