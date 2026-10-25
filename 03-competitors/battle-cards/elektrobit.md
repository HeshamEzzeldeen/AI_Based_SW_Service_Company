# Elektrobit (EB, Aumovio) Battle Card: AI-Native AUTOSAR BSW Delivery
*Skill: sk-competitors | Generated: 2026-10-24*

**Threat level: Medium now** (overall rating in competitors-report.md), **rising to Medium-High within 12-24 months** as integration-as-code becomes AI-assisted [Opinion]. EB is about a year behind Vector on AI configuration but is turning integration labour into a product.

## At a Glance
- **What they do:** Erlangen stack vendor: EB tresos Classic AUTOSAR BSW and configuration tooling, plus integration services on its own stack. Part of Aumovio (Continental's spun-off automotive business, 2025). [Data / Prior knowledge]
- **Ownership:** one CB Insights snippet says "acquired by SDVerse, Dec 2025"; **unverified and likely wrong** (a 2026 source still calls EB a Continental subsidiary). [Data, conflicting]
- **Scale:** DATA GAP; ~3,500+ staff [Prior knowledge, unverified].
- **Price / model:** "upfront pricing for predictable budgets or volume-based pricing that scales with production"; global concept licences across projects (HL Mando case); claims "up to 50% savings via licensing" and "up to 30% lower BSW cost when migrating". Prices DATA GAP. [Data, vendor claims]
- **AI / automation:** "Integration-as-code": reusable integration rules and high-level APIs as version-controlled logic, "laying the groundwork for future AI-assisted software configuration". Oct 2026 Microchip pre-integrated MCAL on EB tresos (Asia two-wheelers, North America first). **No shipped AI agent.** tresos "Unattended Wizard" is deterministic, not GenAI. [Data]
- **Best for:** buyers on EB tresos stacks, and almost everyone at the MCAL layer (many MCU vendors ship MCAL configuration as tresos plugins). [Data]

## Their Strengths (be honest)
- **Owns a major BSW stack and is often unavoidable at the MCAL layer**, even in Vector projects. [Data]
- **Names the same pain you sell against** ("a single parameter change cascades into hours of rework", "knowledge lives in experts' heads", "CI/CD remains aspirational") and is productising the fix. [Data, EB vendor page]
- **Pre-integration deals with silicon vendors** (Microchip) shrink the integration work per ECU. [Data]
- **Migration offer** (up to 30% lower BSW cost) competes for stack decisions at the start of projects. [Data, vendor claim]

## Their Weaknesses (your openings)
- **AI configuration is "future", not shipped.** [Data]
- **Single-stack services**; licences come first. [Opinion]
- **Parent reorganisation (Aumovio)** and unclear ownership signals may slow decisions. [Assumption]
- **Practitioner friction:** tresos install and plugin issues; tresos generator errors inside DaVinci; MCAL version mismatches (forum posts, 2019-2025; several >12 mo). [Data, Tier 3]

## How to Win Against Them
- **Lead with:** mixed-stack integration where EB MCAL meets a Vector or ETAS BSW and an HSM from a third vendor. This is where forum pain clusters. [Data + Opinion]
- **Build on EB's APIs**, not against them: if integration-as-code becomes AI-callable, your agents should drive it. [Opinion]
- **Talking point:** "EB makes its own stack scriptable. We make your whole ECU, across vendors, integrate and pass assessment." [Opinion]

## When They Win Over You
- Pure EB tresos ECUs where EB's own services and pre-integrated MCAL cover the job.
- Two-wheeler and price-sensitive Asian programmes using Microchip pre-integration.
- Stack-selection decisions at programme start (EB sells migration and licence savings; you don't sell a stack).
- Once EB ships AI-assisted configuration inside tresos.

## Objections and Responses
- **"EB integration-as-code will automate this."** Response: "For EB modules, eventually. Your ECU also has a Vector crypto stack and an Infineon HSM. Who integrates those, and who signs the evidence?" [Opinion]
- **"We'll just ask EB support."** Response: "EB support covers EB. Cross-vendor errors like tresos generators failing inside DaVinci are what we fix, at a fixed price." [Data + Opinion]

## Their Customers' Top Complaint
"no AUTOSAR release version" selectable after install; support recommended "basic training first" (NXP Community, tresos install thread). **This matters because:** EB tooling friction is real but minor; the bigger opening is multi-vendor integration errors.

## Key Vulnerability
**AI configuration not shipped, single-stack scope.** A 12-24 month window before EB matches Vector. [Data + Opinion]

## Churn Signals
- Tooling and integration friction — **occasional** (forum evidence, thin). [Data]
- Stack migrations driven by licence cost — **occasional**; EB is usually the destination, not the source. [Data]

## Strategic Vulnerability
| Type | Description | Exploitability | Confidence |
|---|---|---|---|
| Product | AI-assisted configuration not yet shipped | Medium (time-limited) | Medium |
| Organisational | Parent reorganisation; ownership signals unclear | Low | Low |
| Ecosystem | Pre-integration with silicon vendors reduces per-ECU integration work | n/a (risk to you) | Medium |

**Watch for:** AI assistant in tresos; more silicon pre-integration deals; EB partner program terms for AI-native integrators; ownership clarification. [Opinion]

## Data Gaps

- The shared web-search budget ran out during research, so every research agent stopped early. Coverage of this competitor is partial.
- Paid analyst reports (Everest, ISG, Zinnov) were inaccessible. Only vendor-published excerpts were used.
- Employee-review sites (Glassdoor, AmbitionBox, Indeed) blocked direct access. Quotes are search snippets.
- No direct buyer (OEM/Tier 1) interviews yet. Win/loss claims here are hypotheses for the Validate phase.
- Effort and price figures are estimates. See `../pricing-landscape.md` and `../verification-report.md` (C1 correction).
- Full list: `../competitors-report.md`, Data Gaps & Research Limitations.

## Red Flags
- Stack vendors (EB, Vector) are turning integration into executable, AI-callable product. The per-ECU integration-service market you depend on may shrink. [Data + Opinion]

## Yellow Flags
- EB ownership (SDVerse claim) unresolved.
- tresos API and command-line capability not verified this session.
- Forum evidence partly from 2019-2021 (>12 mo).

## Sources
- raw/competitor-profiles.md §5; raw/adjacent-competitors.md §9; raw/tech-stack-analysis.md §1.3; raw/forum-mining.md Theme 1; raw/review-mining.md §3; raw/social-sentiment.md §1.4; raw/pricing-intelligence.md §3 (all 2026-10-24)
- https://www.elektrobit.com/?p=47945 (integration-as-code, ~2026)
- https://www.microchip.com/en-us/about/news-releases/products/elektrobit-and-microchip-collaborate-on-pre-integrated-autosar-solutions (15 Oct 2026)
- https://www.eetasia.com/elektrobit-microchip-pre-integrate-autosar-software-for-automotive-platforms/ (Oct 2026)
- https://elektrobit.com/?p=27049 ; https://www.elektrobit.com/?p=46314 (licensing, HL Mando)
- https://community.nxp.com/t5/S32K/EB-tresos-installation-guide/td-p/1837889
- https://community.infineon.com/t5/AURIX/MCAL-Generation-issue/m-p/318481 (Dec 2019, >12 mo)
- https://www.cbinsights.com/compare/elektrobit-vs-vector-informatik (SDVerse claim, unverified)
