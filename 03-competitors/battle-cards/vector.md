# Vector Informatik Battle Card: AI-Native AUTOSAR BSW Delivery
*Skill: sk-competitors | Generated: 2026-10-24*

**Threat level: High** to the "AI configures BSW" message; **Medium** to cross-vendor security integration plus evidence [Opinion]. Vector is gatekeeper, supplier, potential partner and competitor at the same time.

## At a Glance
- **What they do:** Stuttgart stack and tool vendor: MICROSAR Classic BSW (incl. security modules), DaVinci Configurator, CANoe, VectorCAST; plus Vector Consulting Services (ASPICE gap analysis, assessments, 4.0 migration) and embedded integration services. [Data / Prior knowledge]
- **Scale:** 4,000+ staff (company) / 3,675 (Revelio, Sep 2025); Vector Group revenue EUR 1.16B (2023, >12 mo); private, foundation-owned [Prior knowledge]. AUTOSAR Core Partner since Jan 2025 or Jan 2026 (sources conflict: C1 says Jan 2026, the AUTOSAR press-release file is dated 15 Jan 2025; verify before citing). [Data, conflicting]
- **Price / model:** quote-based licence per module set, configurator seats, predefined packages; services attached to licences. **AI requires an "AI-enabled" licence + Embedded Hub account; customer brings its own OpenAI-compatible LLM endpoint (≥32k context); subscription-only from July 2027.** Prices: DATA GAP. [Data]
- **AI shipped / announced (2026):** DaVinci Configurator 6.4 AI chatbot (reads configuration, explains it; "preview of the 2027 version"); "smart modification" of configurations planned for 6.5 (Dec 2026); ECU SDK "EcuC-as-Code" with "AI agentic workflows that realize configuration use cases in code and resolve compile, runtime and validation errors", "Skills and MCP tools"; VectorCAST 2026 AI test creator. **No explicit security/crypto (CSM/CryIf/SecOC/HSM) automation mentioned.** [Data]
- **Best for:** any MICROSAR-based ECU where the buyer wants the vendor to stand behind the stack. [Opinion]

## Their Strengths (be honest)
- **Owns the ground truth:** BSW module definitions, validators, code generators, documentation and the agent loop with compile/runtime feedback. No one can automate MICROSAR configuration more reliably. [Data + Opinion]
- **Trusted default for hard security integration** (HSM, SecOC freshness, key provisioning on MICROSAR). "Nobody got fired for buying Vector." [Opinion]
- **Already on every approved list; licences and support create very high switching costs** ("retraining teams, rebuilding test assets, requalifying evidence"). [Data, commentary]
- **Can invest without quarterly pressure** and is building AI step by step on a clear roadmap. [Data + Opinion]
- **Sells ASPICE consulting and assessments itself**, so it competes for the evidence half too. [Data]

## Their Weaknesses (your openings)
- **Single-stack.** Mixed projects (EB tresos MCAL inside DaVinci, ETAS CycurHSM, MCU-vendor HSM firmware) need a neutral integrator; forum threads show tresos-generator errors inside DaVinci (2019-2021, >12 mo). [Data + Opinion]
- **Services are capacity-limited and premium**; they exist to pull licences, not to cut customer cost. [Assumption]
- **Its own AI disclaims accuracy:** "Always check the referenced sources", "not an authoritative source in itself". The customer still needs accountable engineers. [Data]
- **Subscription-only AI from July 2027** may annoy perpetual-licence customers and adds a new cost line. [Data + Opinion]
- **No visible security-stack automation** in the AI roadmap. [Data]

## How to Win Against Them
- **Don't fight Vector; ride it.** Position as the verified-AI integration partner that uses DaVinci's automation interface, MCP tools and EcuC-as-Code on the customer's licence. Pursue Vector CEEP/CEP certification (Intellias precedent). [Opinion]
- **Lead with:** cross-vendor security integration (Vector crypto stack + Infineon/Cypress HSM firmware or ETAS CycurHSM + OEM key management), verified on AURIX/TRAVEO, with 21434/ASPICE evidence. Vector does not sell this as a fixed-price package. [Opinion]
- **Talking point:** "Vector's agent configures MICROSAR. We make the whole secured ECU work across vendors and give you assessor-ready evidence and a named accountable engineer." [Opinion]
- **Price against Vector service days**, not against the licence. [Opinion]

## When They Win Over You
- **Single-vendor MICROSAR ECUs where the problem is configuration inside DaVinci.** Vector's own agent plus Vector support will beat you, especially after 6.5.
- Buyers who need the vendor's liability and first-line support on the stack.
- When the customer's licence or Vector's terms do not allow third-party or AI-driven use (DATA GAP; Gate 0).
- ASPICE consulting and assessments, where Vector is an authorised assessor brand.
- Any buyer with budget who wants zero perceived risk.

## Objections and Responses
- **"DaVinci's AI agent will do this for us."** Response: "For MICROSAR configuration, increasingly yes. We use it. What it doesn't do is the HSM firmware, secure boot chain, cross-vendor MCAL and the 21434/ASPICE evidence, verified on your hardware. That's our fixed-price scope." [Data + Opinion]
- **"We'd rather get security integration from Vector."** Response: "Reasonable for pure MICROSAR. If your HSM firmware or MCAL comes from another vendor, who owns the integration? We do, at a fixed price." [Opinion]
- **"Is your use of our Vector licence allowed?"** Response: must be answered with confirmed licence terms. Do not improvise. [Assumption: DATA GAP]

## Their Customers' Top Complaint
No public reviews exist for Vector, ETAS or EB tools on G2, Gartner Peer Insights, Capterra or PeerSpot. Proxy: forum posts on multi-vendor integration errors and quote-based, split licensing ("some actions need a Package licence, others a Configurator licence"). **This matters because:** the pain you can address is integration glue and licence complexity, not Vector's core product quality.

## Key Vulnerability
**Single-vendor scope.** Vector automates its own stack; it does not own the cross-vendor security integration or the customer-project accountability. [Opinion, supported by Data on roadmap scope]

## Churn Signals
- Stack migrations happen but are rare and painful (EB markets migration, which confirms the pain) — **rare**. [Data]
- Possible resistance to subscription-only AI from July 2027 — **watch**. [Opinion]
- No evidence of customers leaving Vector services for third parties (DATA GAP).

## Strategic Vulnerability
| Type | Description | Exploitability | Confidence |
|---|---|---|---|
| Product | Single stack; no security automation announced | Medium | Medium |
| Pricing | AI subscription adds cost and lock-in friction | Low-Medium | Medium |
| Operational | Capacity-limited services | Medium (overflow work) | Low (assumption) |
| Channel | Partner program (CEEP) gives access but also gives Vector visibility into your methods | n/a (risk to you) | Medium |

**Watch for:** 6.5 "smart modification" (Dec 2026); security modules added to the agent workflow; subscription price; Vector terms on third-party AI use; Vector certifying AI-native partners. [Opinion]

## Data Gaps

- The shared web-search budget ran out during research, so every research agent stopped early. Coverage of this competitor is partial.
- Paid analyst reports (Everest, ISG, Zinnov) were inaccessible. Only vendor-published excerpts were used.
- Employee-review sites (Glassdoor, AmbitionBox, Indeed) blocked direct access. Quotes are search snippets.
- No direct buyer (OEM/Tier 1) interviews yet. Win/loss claims here are hypotheses for the Validate phase.
- Effort and price figures are estimates. See `../pricing-landscape.md` and `../verification-report.md` (C1 correction).
- Full list: `../competitors-report.md`, Data Gaps & Research Limitations.

## Red Flags
- **Vector productises the core claim "AI agents configure BSW"** inside the tool every target buyer already licenses. A message built on that claim loses within 12-18 months. [Data + Opinion]
- **You depend on Vector's licence terms.** If third-party or AI use of customer licences is restricted, the delivery model shrinks to AI-assisted staff augmentation. [Assumption, DATA GAP]
- **This is the weakest battle card for the founders**: there is no head-to-head win on single-vendor MICROSAR configuration. The only winning moves are complement and partner. [Opinion]

## Yellow Flags
- Vector Consulting sells ASPICE services, which can create channel conflict if you also sell ASPICE evidence. [Opinion]
- Vector revenue figure is from 2023 (>12 mo).

## Sources
- raw/tech-stack-analysis.md §1.1, §5; raw/adjacent-competitors.md §8; raw/social-sentiment.md §1.4; raw/competitor-profiles.md §3; raw/gtm-analysis.md §1.10; raw/review-mining.md §3; raw/pricing-intelligence.md §3 (all 2026-10-24)
- https://www.vector.com/en/product/microsar-classic/davinci-configurator-new-generation/ (2026)
- https://help.vector.com/davinci-configurator-classic/en/latest/user-manual/ui-client/views/ai-agent-view.html (2026)
- https://help.vector.com/davinci-configurator-classic/en/6.3/user-manual/automation/automation.html (Mar 2026)
- https://www.vector.com/en/company/press/press-releases/vectorcast-2026-launches-ai-powered-requirements-based-test-creator/ (Mar 2026)
- https://www.vector.com/en/business-unit/consulting/consulting-services/transformation/automotive-spice/
- https://intellias.com/intellias-strengthens-embedded-software-expertise-through-vector-certification/ (Sep 2023, >12 mo)
- https://community.infineon.com/t5/AURIX/MCU01803-Invalid-XPath-error-by-Tresos-generator-for-TC33x/m-p/318684 (Jan 2021, >12 mo)
- https://en.wikipedia.org/wiki/Vector_Informatik
