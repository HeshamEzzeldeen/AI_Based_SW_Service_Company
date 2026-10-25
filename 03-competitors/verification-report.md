# Verification Report: AI-Native AUTOSAR BSW Delivery (sk-competitors, Deep)
*Generated: 2026-10-24 | Agent: V1 | No web research; raw files in `raw/` used as the source of truth*

**Files checked:** `../03-competitors.md`, `competitors-report.md`, `competitive-matrix.md`, `pricing-landscape.md`, 10 battle cards, 3 competitor dossiers (KPIT, Tata Elxsi, Vector).

## Summary
- **Critical issues:** 1 (numbers fixed; the price decision is left to the founders)
- **Warnings:** 11 (8 fixed, 3 open)
- **Info:** 10

---

## Critical Issues
The process pauses here for founder review.

### C1. Per-ECU cost figures were overstated about 5-8x, and the per-ECU price hypotheses rested on them
- **File(s):** `pricing-landscape.md` (§1.2, §8.2, Red Flags), `../03-competitors.md` (Pricing Landscape Summary), `competitors-report.md` (Pricing Snapshot, Opportunity 2, Founder Precedent), `competitive-matrix.md` (Differentiation 3). Origin: `raw/pricing-intelligence.md` §5.
- **Problem:** Raw A2 says per-ECU cost = "15-45 PM × loaded monthly rate (about 160 h × hourly rate from section 1)". It then used EUR 110k/PM (Germany), EUR 60k/PM (Eastern Europe) and EUR 25-35k/PM (India/Egypt). Its own basis gives:
  - Germany: EUR 85-130/h × 160 h = **EUR 13.6-20.8k/PM**
  - Eastern Europe: EUR 45-75/h × 160 h = **EUR 7.2-12k/PM**
  - India/Egypt: USD 25-45/h × 160 h = **EUR 3.6-6.5k/PM**. A2 itself also says India is "often sold as about USD 4-7k per FTE-month".
  
  The deliverables therefore said one new ECU costs **EUR 0.4-1.6M offshore and EUR 1.7-5M in Germany**. At the stated basis it is **about EUR 0.05-0.3M offshore and EUR 0.2-0.95M in Germany**.
  
  This changes a pricing conclusion. A2 and `pricing-landscape.md` §8.2 said the EUR 250-600k new-ECU hypothesis "lands at or below India T&M equivalent". Corrected, it sits **above offshore T&M cost and inside the German range**. Likewise, the EUR 60-150k security package was meant to be "half of offshore". Corrected offshore cost for 3-9 PM is about EUR 11-60k, so EUR 60-150k is at or above offshore cost and roughly at German cost.
- **Fixed by V1 (mechanical):**
  - Recomputed the §1.2 cost table and its "key point" from the stated basis.
  - Corrected the per-ECU figures in the summary, the report and the matrix.
  - Added a visible "V1 correction" note at each place where the EUR 60-150k, EUR 250-600k and EUR 80-200k hypotheses appear.
  - Replaced the precedent's "EUR 100-600k" with the actual hypotheses.
  - Left the raw file unchanged, as the source record.
- **Not fixed (founder decision):**
  - The price hypotheses themselves and the "half the cost" framing they were meant to support. The founders must re-derive per-ECU prices from their own past-project effort data.
  - The founders must also decide whether "half the cost" is still defensible against any baseline other than German onsite. At a corrected German cost of EUR 0.2-0.95M per new ECU, "half" means about EUR 0.1-0.47M.
  - Separately, the effort ranges (12-36 PM per ECU, 3-9 PM for security) are still unverified.

---

## Warnings

### W1. KPIT top-25 concentration quoted as 82-88% in some places and 85-88% in others (FIXED)
- **File(s):** `battle-cards/kpit.md` (3 places), `competitor-dossiers/kpit.md` (§5, inconsistent with its own Snapshot), `pricing-landscape.md` §6.
- **Problem:** Raw A1 gives 82-88% (ICRA, dcf-analysis). C1 gives about 87% (ICICI) and 85-87.8%. The report and summary use 82-88%.
- **Fix applied:** Standardised on "~82-88%", which covers all raw sources.

### W2. KPIT fixed-price share given as "68% of revenue" without a period (FIXED)
- **File(s):** `competitor-dossiers/kpit.md` Red Flags, `pricing-landscape.md` (whitespace and Red Flags), `competitive-matrix.md` Gap Analysis, `../03-competitors.md` Key Competitors table.
- **Problem:** Raw: 65.4% of FY26 revenue and 68.3% in Q4 FY26 (59.6% a year earlier). Writing "68% of revenue" overstates the full-year share.
- **Fix applied:** Each instance now names the period ("68.3% in Q4 FY26; 65.4% FY26").

### W3. Threat levels for Elektrobit and ETAS/ESCRYPT disagreed between battle cards and report (FIXED by clarification)
- **File(s):** `battle-cards/elektrobit.md`, `battle-cards/etas-escrypt.md` vs `competitors-report.md` / `../03-competitors.md`.
- **Problem:** Both cards said "Medium-High"; the report and summary say **M**.
- **Fix applied:** The card headlines now state "Medium overall (as in the report)". They keep their scoped judgments: EB rises to Medium-High within 12-24 months; ETAS is Medium-High for the cyber wedge on credibility. A note was added under the report's Key Players table. No rating was changed.

### W4. Vector "AUTOSAR Core Partner since Jan 2026" stated as fact in the battle card (FIXED)
- **File(s):** `battle-cards/vector.md`.
- **Problem:** The Vector dossier correctly flags a date conflict: C1 says Jan 2026, but the cited AUTOSAR press-release file is dated 2025_01_15.
- **Fix applied:** The card now says "Jan 2025 or Jan 2026 (sources conflict; verify)".

### W5. Data Gaps sections missing (PARTLY FIXED)
- **File(s):** `../03-competitors.md`, `competitive-matrix.md` and `pricing-landscape.md` had no Data Gaps section. None of the 10 battle cards has one: gaps appear only inline as "DATA GAP" and in Yellow Flags.
- **Problem:** The summary said "read the data gaps" but had no section or link. Web-search budget exhaustion was mentioned only in the Method line.
- **Fix applied:** Added Data Gaps sections to the summary (top 8 gaps plus the budget-exhaustion and HTTP 403 note, linked to the report's full 17-item table), the matrix and the pricing landscape. All content was taken from existing deliverable and raw statements.
- **Open:** The battle cards still lack a dedicated Data Gaps section. Suggested fix: add a 2-4 line section to each, collecting its inline DATA GAP items.

### W6. Egypt automotive rate labelled [Data] although the raw file labels it an estimate (FIXED)
- **File(s):** `../03-competitors.md`, `competitors-report.md` Pricing Snapshot, `competitive-matrix.md` basis notes.
- **Problem:** Raw A2 labels the Egypt automotive rate (USD 25-40 or 25-45/h) as [Estimate - unverified] from one generic source. The deliverables placed it under [Data, M].
- **Fix applied:** Relabelled it [Estimate, unverified]. The 25-40 vs 25-45 range difference exists inside A2 itself; see Info.

### W7. Key Players tables carried no claim labels (FIXED)
- **File(s):** `../03-competitors.md` Key Competitors table, `competitors-report.md` Key Players table.
- **Problem:** Most cells mix sourced figures (revenue, staff) with judgments (moat, strength, threat) without labels.
- **Fix applied:** Added a label note under each table: figures are [Data] unless marked; moat, strength/weakness and threat cells are [Opinion].

### W8. Stale data not marked in the summary and report (FIXED)
- **File(s):** `../03-competitors.md`, `competitors-report.md`.
- **Problem:** Vector's EUR 1.16B revenue is from 2023 (more than 18 months old). The Bertrandt 800-1,200 job cuts were first reported in Sep 2024 (raw B1). Neither was marked.
- **Fix applied:** Both are now marked as more than 18 months old. The Bertrandt note says the Dec 2025 results confirm the restructuring.

### W9. Duplicate-source corroboration (OPEN)
- **File(s):** `competitors-report.md` Risk 2 "[Data, A1/A2/C2, H]"; `../03-competitors.md` Key Finding.
- **Problem:** KPIT's fixed-price, ">80% of new deals" and AI claims are cited across three raw files. All of them trace back to the same two secondary articles (Multibagg, May 2026; Analytics India Mag, Feb 2026). Two other single-source claims are also presented as separate pieces of evidence: "cybersecurity budgets reopening" (AIM only) and "ER&D −24-25%" (AIM only). Neither is false corroboration of something dubious, since both are company statements. Still, three raw files do not make three independent sources.
- **Suggested fix:** Cite the underlying sources (Multibagg, AIM) rather than the raw-file IDs. Before any pitch use, verify against KPIT's own investor presentation.

### W10. "Credible measured AI gains are 10-19%" rated High (OPEN)
- **File(s):** `competitors-report.md` Risk 3 and Red Flags, `pricing-landscape.md`, `../03-competitors.md`.
- **Problem:** Per raw B3, 17-19% is self-reported by Capgemini survey "high-value adopters" and about 10% is Bain. Only METR is a measured RCT, and it found developers 19% *slower*. "Measured" overstates the evidence, and "H" is generous for a survey-based range.
- **Suggested fix:** Say "surveyed / reported AI gains of 10-19%" and rate it Medium.

### W11. Summary "Biggest risk" confidence bundles a Low-Medium estimate under High (OPEN)
- **File(s):** `../03-competitors.md` Executive Summary item 4; `competitors-report.md` Executive Summary item 4.
- **Problem:** Item 4 is labelled [Data + Estimate, H]. It includes the 6-18-month qualification gap, which the report itself rates [Estimate, L-M].
- **Suggested fix:** Split the confidence: Vector productisation [Data, H]; qualification gap [Estimate, L-M].

---

## Info
- **Links:** all 22 relative links in `../03-competitors.md` Full Deliverables and Dossiers resolve to existing files. `02-niches.md` exists and supports the non-solicitation claims (Avelabs: both founders; Luxoft: Waled). A link to this report was added.
- **ER&D −24-25%:** correctly described as a global figure from KPIT management in the summary, report and KPIT dossier. The Tier 1 in-house card said "OEM ER&D spend"; it now says "global auto ER&D spend ... not a European measurement" (fixed).
- **Vector dates are consistent across all files and match raw:** 6.4 assistant shipped as a preview; 6.5 smart modification in Dec 2026; AI subscription-only from July 2027. The "6.4 applies small changes" conflict (product page vs help page) is documented consistently.
- **KPIT figures match raw:** FY26 USD 724.8M (+4.8% USD, +1.3% cc); Q1 FY27 USD 176.8M (−0.6% YoY USD); headcount 12,724-13,000; revenue per employee about USD 53-57k. The +8.9% (INR) vs −0.6% (USD) conflict is resolved consistently.
- **Egypt rate range:** the pricing landscape and Avelabs card use USD 25-40/h; the summary, report and matrix use 25-45/h. Both ranges appear in raw A2 (§1 table vs §1.2 ladder). Harmonise when better data exists.
- **Founders' moat durability:** the summary merges the report's "harness 2-4 yr [Estimate]" and "security specialisation 3-5 yr [Opinion]" into "2-5 yr". This is acceptable but loses the split.
- **Valuation multiples:** the pricing landscape says "AI-native >3x vs 1-2x traditional" (Livingstone, latter an Assumption); the report says "services 1-3x". Both come from C2 and are consistent once read in context.
- **Coverage:** Capgemini Engineering, Bertrandt and Akkodis appear in the report and matrix without battle cards. This is allowed (threat M/L), and a note was added under the summary table. Every battle-card competitor appears in the report's Key Players table, and every matrix column has a report profile.
- **Stale-data threshold:** the pricing landscape and cards flag anything older than 12 months, which is stricter than the 18-month protocol. Fine.
- **Raw file not edited:** `raw/pricing-intelligence.md` §5 still contains the per-PM error behind C1. Treat its EUR 1.7-5M / 0.9-2.7M / 0.4-1.6M totals as superseded.

---

## Fix Log (files changed by V1)
| File | Change |
|---|---|
| `pricing-landscape.md` | §1.2 table and key point recomputed (C1); correction note added; §8.2 hypotheses annotated; Red Flag annotated; KPIT T25 82-88%; KPIT fixed-price periods; Data Gaps section added |
| `../03-competitors.md` | Per-ECU cost corrected and hypothesis annotated (C1); Egypt label; KPIT 68.3% (Q4 FY26); Vector 2023 stale mark; table label note; Data Gaps section; link to this report |
| `competitors-report.md` | Pricing Snapshot corrected (C1); Opportunity 2 and Walton precedent annotated; Egypt label; Vector stale mark; Bertrandt stale mark; Key Players label/threat note; contradiction-resolved entry for C1 |
| `competitive-matrix.md` | Egypt label; KPIT fixed-price periods; per-ECU hypothesis annotated; Data Gaps section |
| `battle-cards/kpit.md` | T25 82-88% (3 places) |
| `battle-cards/vector.md` | Core Partner date conflict stated |
| `battle-cards/elektrobit.md`, `battle-cards/etas-escrypt.md` | Threat headline aligned with report (scoped ratings kept) |
| `battle-cards/tier1-in-house.md` | ER&D wording (global, KPIT claim) |
| `competitor-dossiers/kpit.md` | T25 82-88% (§5); fixed-price period in Red Flags |

No strategic conclusion, threat rating or recommendation was changed. The per-ECU price hypotheses were annotated, not replaced.

---

## Verification Checklist
- [ ] All quantitative claims labeled: mostly. Tables are now covered by label notes; battle-card body text is largely labelled.
- [ ] No internal contradictions found: C1 and W1-W4 fixed; Egypt range variance remains (Info).
- [ ] Confidence ratings consistent with evidence: W10 and W11 open.
- [ ] Data gaps declared in all deliverables: battle cards still lack a dedicated section (W5).
- [x] Red/Yellow flags present in all deliverables
- [x] No stale data unmarked (after W8 fixes)
- [ ] No duplicate-source false corroboration: W9 open.
- [x] Battle cards consistent with report (after W3 clarification)
- [x] Matrix aligned with profiles
- [x] Pricing landscape consistent with profiles (after C1 / W1 / W2 fixes)
- [x] Opportunities backed by multi-source evidence. Opportunity 1 has 8 evidence items across A3, C3, B2 and C2; Opportunities 2-4 cite at least 2 deliverable sources each.

---

## Post-verification resolution (2026-10-24)

- **C1 (price decision):** The founders chose to proceed. Price hypotheses are marked as placeholders, to be set in Offer (Phase 5) and Money (Phase 7) from the founders' own effort data with an explicit "half the cost" baseline.
- **W5 (resolved):** Added a Data Gaps section to all 10 battle cards.
- **W9 (resolved):** The KPIT evidence note in competitors-report.md now states that the claims trace to two secondary articles and must be verified against KPIT's investor presentation.
- **W10 (resolved):** Reworded to "surveyed/reported AI gains of 10-19%" and downgraded to Medium confidence across deliverables.
- **W11 (resolved):** Split the confidence in Executive Summary item 4: Vector productisation [Data, H]; qualification gap [Estimate, L-M].
