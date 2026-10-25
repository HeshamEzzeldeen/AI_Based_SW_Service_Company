# Competitor Dossier: Vector Informatik
*Skill: sk-competitors | Generated: 2026-10-24*
*Depth: Deep | Threat level: **High** (highest structural threat to "AI configures BSW"; Medium to cyber-integration-plus-evidence services) | Synthesised from raw files A1, A2, B1, B2, B3, C1, C2, C3 and adjacent-competitors (no new web research)*

> **How to read this file.** Labels: **[Data]** = sourced finding, **[Estimate]** = calculation with stated basis, **[Assumption]** = unverified belief, **[Opinion]** = analyst judgment. Confidence (High / Medium / Low) is given on major claims. Items marked **(>12 months old)** pre-date Oct 2025 and may be stale. Vector is both a **competitor** (its services arm and its in-tool AI) and a **gatekeeper / possible partner** (its stack and licences). This dossier treats both roles.

---

## Snapshot

| Field | Value | Label / confidence |
|---|---|---|
| What they are | German automotive tool and embedded-software vendor: MICROSAR Classic BSW, DaVinci Configurator, CANoe, VectorCAST, plus Vector Consulting Services and embedded integration services | [Data] High |
| HQ / ownership | Stuttgart, Germany; private, foundation-owned | [Prior knowledge, unverified] Medium |
| Founded | 1988 | [Prior knowledge, unverified] Medium |
| Revenue | EUR 1.16B (Vector Group, 2023) | [Data, Wikipedia] **(>12 months old)**; 2025/26 DATA GAP |
| Headcount | 4,000+ at 33 locations (company) vs 3,675 (Revelio Labs, Sep 2025) | [Data] Medium (sources disagree) |
| Services revenue share | DATA GAP | — |
| AUTOSAR standing | Premium Partner since 2004, Premium Partner Plus since 2023, Core Partner (with DENSO and Huawei) | [Data] High (see date conflict below) |
| In-tool AI | DaVinci Configurator Classic 6.4 AI Assistant (shipped, preview); agentic ECU SDK / EcuC-as-Code; "smart modification" planned for 6.5 (Dec 2026); AI subscription-only from July 2027 | [Data, Vector pages fetched 2026-10-24] High |
| Moat type | Installed-base switching costs + IP (BSWMD, validators, generators) + ecosystem | [Opinion] High |
| Key vulnerability | Single-stack scope; services capacity-limited and premium; AI subscription change may anger perpetual-licence customers | [Opinion] Medium |
| Moat durability | 5+ years | [Opinion] Medium-High |

---

## 1. Company Foundation & Strategic Position

### Founding narrative and milestones
- Founded 1988 in Stuttgart [Prior knowledge, unverified]. Detailed founding narrative and leadership: DATA GAP this session.
- **Acquisitions:** ARCCORE (AUTOSAR stack vendor, with a dual open-source/commercial model) in July 2018 [Data, eeNews] **(>12 months old)**; StatInf's RocqStat WCET timing-analysis technology and team in Jan 2026 [Data, Wikipedia]. [Opinion] Vector buys adjacent technology to deepen its toolchain rather than to buy services capacity.
- **AUTOSAR consortium:** Premium Partner Plus since 2023 (Premium since 2004); became a **Core Partner** alongside DENSO and Huawei [Data]. **Date conflict:** C1 states Jan 2026, but the cited AUTOSAR press-release file name is dated "2025_01_15". [Assumption] The correct date is probably 15 Jan 2025. Verify before citing.

### Leadership and public influence
- DATA GAP this session (no leadership research). Vector's public influence comes through its products, its annual Vector Congress [Assumption: known event; exhibitor list not retrieved] and its AUTOSAR Core Partner role.

### Funding / ownership
- Private and foundation-owned [Prior knowledge, unverified]; large and profitable enough to invest without quarterly pressure [Data/Opinion, A1]. No external funding.

### IP portfolio and moat assessment
- **IP:** MICROSAR Classic BSW including security modules (Crypto stack, SecOC, CSM/CryIf, HSM firmware) [Data for the stack; security-module detail is Prior knowledge, unverified]; DaVinci Configurator Pro/Classic/Gen 6 and DaVinci Developer (ARXML-based, code generators) [Data]; CANoe and VectorCAST [Data/Prior knowledge]; RocqStat WCET [Data]. Patents: DATA GAP.
- **Moat assessment [Opinion, High]:** Vector owns the "ground truth" for configuring its stack: the BSW module definitions (BSWMD), validation rules, generators and the documentation corpus. ARXML itself is open, but valid configuration and generated C code only come out of the licensed tool. Switching costs are very high: moving off Vector means "the cost of retraining teams, rebuilding test assets, requalifying evidence" [Opinion of a commentator, btw.media]. A2 puts the buyer mindset as "nobody got fired for buying Vector" [Opinion]. Durability 5+ years.
- **Default-stack evidence [Data]:** Capgemini job ads (Mar 2026) list Vector DaVinci as the working tool for Classic AUTOSAR integration; job ads across the market list EB tresos, Vector DaVinci, CANoe, TRACE32 and HighTec as the de facto stack.

---

## 2. Product & Value Proposition Architecture

### Product and service suite
| Line | What | Evidence |
|---|---|---|
| MICROSAR Classic | Classic AUTOSAR BSW, including MICROSAR security modules | [Data]; security detail [Prior knowledge, unverified] |
| DaVinci Configurator Classic / Gen 6 | BSW configuration and generation; Automation Interface (Groovy/Kotlin, Gradle; docs v3.9.0 for DVCfg 6.3.0, 11 Mar 2026); FlatView APIs (6.2); ECU SDK and "EcuC-as-Code" with Git; Windows or Linux, on-prem or cloud; improved CLI | [Data, 2025-26] |
| DaVinci AI Assistant | Chat assistant answering from Vector docs, BSW package docs and Embedded Hub; reads the ECU configuration and answers project questions | [Data] **Shipped in 6.4 (preview)** |
| Agentic configuration | ECU SDK: "AI agentic workflows that realize configuration use cases in code and resolve compile, runtime and validation errors"; "Skills and MCP tools"; "Structured feedback from compilation and execution flows straight back to the agent"; human "supervising" | [Data] Announced; ECU SDK milestones reached with 6.4; depth of agent support DATA GAP |
| Smart modification | AI that modifies configurations with suggestions | [Data] **Planned for 6.5, Dec 2026** |
| VectorCAST 2026 (Mar 2026) | AI requirements-based test creator, bring-your-own-model; "AI-generated outputs are therefore subject to the same verification and quality controls as human-written code" | [Data] |
| Vector Consulting Services | ASPICE gap analysis (ASPICE4Check), authorised-assessor assessments (3.1 and 4.0), ASPICE 4.0 migration, training, coaching; security consulting | [Data] |
| Embedded integration services | MICROSAR introduction, development and integration support | [Prior knowledge, unverified; partly Data via CEEP description] |

**Conflicting data on what 6.4 can do:** C3 quotes the product page as saying the 6.4 chatbot "explains a configuration and applies small changes". B3 and the adjacent-competitor file, using the help page, say 6.4 **reads** the configuration and that change suggestions arrive in **6.5 (Dec 2026)**. [Opinion] Trust the help page: 6.4 is read-and-explain; AI-driven modification arrives with 6.5. Either way, modification is less than two months away. Confidence: Medium.

**Earlier data gap now closed:** A1 listed "GenAI in DaVinci" as a DATA GAP because its search budget ran out. C3, B3 and the adjacent-competitor agent later fetched Vector's pages and confirmed the AI features above.

### Key differentiators
- Owns the stack, the configurator and the stack's internal knowledge; buyers trust the vendor most for hard security integration (HSM, SecOC freshness, key provisioning) [Opinion, A1]. Confidence: Medium-High.
- **The only player found with an AI moat at the configuration layer**, because the agent loop runs against Vector's own validators and generators with compile/runtime feedback [Opinion, C3]. Confidence: High.
- Model-agnostic: bring your own OpenAI-compatible endpoint (Qwen or GPT named), at least 32k context, 64k+ recommended [Data].

### Limitations
- **No mention of security-stack automation** (CSM/CryIf/SecOC/HSM) in its AI features [Data: absence on fetched pages]. Confidence: Medium.
- Single-vendor scope: does not serve EB tresos or ETAS stacks, and does not automate cross-vendor glue such as MCU-vendor MCAL delivered as EB tresos plugins inside a DaVinci project [Data + Opinion].
- Vector's own docs warn AI answers "can be incomplete or inaccurate" and should be treated "not as an authoritative source in itself" [Data].
- Forum evidence shows recurring integration pain at the vendor boundary: an XPath validation error (MCU01803) when running tresos as a third-party generator inside DaVinci (TC3xx), MCAL generator failures in tresos+DaVinci integration [Data, Infineon community, 2019-2021, **>12 months old**].

### Integration ecosystem and API strategy
- Public Automation Interface (Groovy/Kotlin), CLI, EcuC-as-Code with Git, MCP tools and skills, Embedded Hub cloud account [Data].
- MATLAB/Simulink link, CANoe, VectorCAST [Data/Prior knowledge].
- [Opinion] Platform pattern: open enough for automation, but the highest-value AI features are licence- and subscription-gated and tied to Vector's cloud account. Technically, an outside integrator can drive DaVinci with its own agents; the open question is contractual.

### Pricing model, psychology and evolution
- **MICROSAR:** quote-based; request for quote per module set; licensing "can be discussed in parallel to ECU development"; also predefined packages with updates "without lead time and additional costs" [Data, Vector help].
- **Licence complexity:** some DaVinci Package Manager actions need a Package licence, others a Configurator licence; the tool recommends 16 GB RAM [Data].
- **Indicative price:** a full BSW stack plus security modules for one ECU project runs low-to-mid six figures EUR, with DaVinci seats extra [Estimate - unverified, practitioner hearsay, Low confidence]. Do not use in a pitch.
- **AI pricing evolution [Data]:** AI requires a licence "that allows AI features", an Embedded Hub account and token, and Project Space membership. The current build is "a preview of the 2027 version". **From July 2027 the AI Assistant is available only as a subscription.** AI subscription price: DATA GAP.
- **Psychology [Opinion]:** classic land-and-expand. Licences create lock-in, services attach to licence accounts, and AI becomes a recurring upsell on the installed base.

---

## 3. Target Customer Profile (Inferred)

### Primary and secondary segments
- **Primary [Data/Opinion]:** OEMs and Tier 1s that use MICROSAR on Classic ECUs; they hold the licences, tied to their projects [Assumption on licence holding].
- **Secondary [Data]:** engineering service providers who integrate MICROSAR for those customers (Capgemini, Intellias, Teoresi); Vector trains and certifies them through the CEEP programme.

### Firmographic, technographic and behavioural signals
- Buyers run DaVinci, CANoe and often VectorCAST; many also use EB tresos on the MCAL layer because MCU vendors ship MCAL configuration as tresos plugins [Data].
- Buyers increasingly want CI/CD, Git and Linux/cloud builds, which Gen 6 targets [Data].

### Pain points addressed (from messaging)
- Configuration complexity, slow integration, validation errors, ASPICE assessment readiness and ASPICE 4.0 migration [Data].

### Customer journey touchpoints
- Account sales via the licence relationship, help portal, Embedded Hub, Vector Congress, AUTOSAR consortium, CEEP partners [Data / Assumption for Congress].

---

## 4. Customer Voice & Market Sentiment

### Review analysis
- **Zero public reviews** for DaVinci, MICROSAR, ETAS RTA or EB tresos on G2, Gartner Peer Insights, Capterra or PeerSpot (3 query variants) [Data: absence]. The AUTOSAR tool market has no public review culture. Confidence: High that reviews are absent; therefore sentiment below is thin.
- **Praise (inferred):** default stack status, trust for difficult security integration [Opinion].
- **Complaints (forum proxies, Tier 3):** multi-vendor integration errors (tresos inside DaVinci), licensing opacity and split licences, version mismatches [Data, 2019-2025 forum threads, partly **>12 months old**]. The recurring pain is "integration glue", which is tedious and rule-bound [Opinion].
- HN practitioner sentiment toward AUTOSAR stacks generally is negative ("integration hell", "3 months vs 1 week" rewrite anecdote), but HN skews toward generalists who dislike AUTOSAR, and positive Vector/EB users are under-represented [Data + Opinion].

### NPS / satisfaction
- None public. DATA GAP.

### Analyst and industry perception
- [Opinion] Vector is seen as the default and safest choice. Its AI messaging is careful and engineering-led ("the human focuses on supervising"; AI output under "the same verification and quality controls as human-written code"), which matches what ASPICE assessors want to hear (intacs, Oct 2026: "is the AI use controlled?").
- Third-party claim: VxLabs Security (AI-TARA, with an office in Giza, Egypt) lists Vector among "trusted by" logos; the nature of the relationship is unknown [Data, vendor claim, unverified].

---

## 5. GTM Strategy & Revenue Engine

### Sales motion
- **Tool-licence-led enterprise sales** [Opinion, High]. Services attach to MICROSAR and tool accounts; capacity is used mainly to pull licences through, not to reduce customer cost [Assumption, A1].

### Acquisition channels and content
- Installed base and licence renewals; Vector Congress; AUTOSAR consortium leadership; help-portal and product content on ASPICE 4.0 [Data/Assumption].

### Partnership and channel programmes
- **Certified Embedded Engineering Partner (CEEP)**, with engineers trained as Certified Embedded Professionals (CEP) on Classic AUTOSAR plus Vector tools [Data].
  - Named partners: Intellias (Sep 2023), Teoresi (2024) [Data].
  - Benefits: access to Vector experts and technology updates; positioning for MICROSAR "introduction, development and integration support" [Data].
  - **Lead referral is not stated** [Data]. Fees not published [Data].
  - Precedent: Intellias (Ukraine-origin, with a Cairo hub) used Vector CEEP (Sep 2023), then the EB Compatibility Program (CES 2025), then Infineon PDH (Mar 2026) as a credibility stack in place of OEM references [Data]. Confidence: High that the path exists.

### Marketing positioning and messaging
- Vector's AI language: "Understand and configure your BSW and RTE configuration with the help of AI agents"; "the human focuses on supervising" [Data].
- [Opinion] This is almost exactly the founders' planned pitch line ("AI agents configure BSW, humans check"), delivered by the vendor inside the tool the buyer already pays for.

---

## 6. Strategic Vulnerabilities & Risks

| Vulnerability | Type | Evidence | Exploitability by founders | Confidence |
|---|---|---|---|---|
| Single-stack scope; does not automate cross-vendor integration (EB MCAL plugins, ETAS CycurHSM, MCU HSM firmware) | Product | Absence of cross-vendor claims; forum integration errors | **High** | Medium-High |
| AI features do not mention security-stack automation | Product | Fetched pages | **High** for the cyber wedge, until Vector adds it | Medium |
| Services are premium and capacity-limited | Operational | [Assumption] | Medium | Low |
| Subscription-only AI from July 2027 | Commercial | Vector help page | Medium: may push some Tier 1s toward vendor-neutral AI services | Medium |
| AI answers "can be incomplete or inaccurate"; customer brings own LLM | Technology | Vector docs | Medium: room for an independent verification layer | High |
| Channel conflict: Vector sells ASPICE consulting and integration services | GTM | Vector Consulting pages | Cuts both ways (risk to a partnership) | High |

### Competitive threats Vector faces
- Elektrobit's "integration-as-code" approach (about a year behind on AI) and ETAS; Chinese stacks (Neusoft Reach NeuSAR Copilot, iSoft) in China; AutoC, an unverified tool claiming natural-language configuration across DaVinci, tresos, ISOLAR and Chinese stacks [Data / unverified].
- Tier 1s driving MICROSAR through Vector's own MCP with general coding agents (Claude Code, Copilot) and internal skills, which reduces the need for both Vector services and external integrators [Opinion].

### Market and regulatory risks
- Zonal/central architectures mean fewer, more complex Classic ECUs; Adaptive and HPC growth sits outside MICROSAR Classic [Data/Opinion].
- Under ISO 26262-8 Cl. 11, an LLM that produces configuration is a high-impact tool; Vector's "same verification as human code" framing shows it knows this [Data + Opinion].

---

## 7. Future Trajectory & Growth Signals

### Product roadmap signals
- 6.5 (Dec 2026): AI configuration modification with smart suggestions [Data].
- July 2027: AI Assistant subscription-only; the current build is a "preview of the 2027 version" [Data].
- ECU SDK agentic workflows with compile/runtime feedback, MCP and skills [Data].
- VectorCAST AI test generation (Mar 2026) shows the same pattern spreading across the toolchain [Data].
- [Opinion, Medium] Within 12-18 months Vector is likely to offer agentic configuration across most MICROSAR modules, probably including security modules, inside the licensed tool.

### Market expansion indicators
- Cloud and Linux support for configuration, Embedded Hub accounts and Project Spaces suggest a move toward cloud-connected, subscription engineering services [Data + Opinion].
- ASPICE 4.0 consulting and assessments as a services growth line [Data].

### M&A likelihood
- **As acquirer: Medium-High** [Opinion], based on ARCCORE (2018) and RocqStat (Jan 2026). Targets would be technology (timing, verification, AI tooling), not services headcount.
- **As target: Very low** (foundation-owned, private) [Assumption].

### Platform / ecosystem ambitions
- [Opinion, High] Vector wants to own the AI layer inside the AUTOSAR toolchain: AI features gated by licence and subscription, tied to Embedded Hub, with MCP and skills coming from Vector itself.

---

## Red Flags
- **Vector is productising the founders' core pitch inside the tool buyers already license.** "AI agents configure BSW, human supervises" is on Vector's product page today, with AI configuration changes due in Dec 2026 [Data]. A message built on "AI generates BSW configuration" will lose to the vendor that owns the validators and generators. Confidence: High.
- **Vector controls access the founders depend on.** Terms for service-provider, subcontractor and automated/AI use of MICROSAR and DaVinci licences were not found. If the AI features must be bought by the customer by subscription, and third parties cannot run agents on customer licences, the delivery model is constrained [Data gap + Opinion]. Confidence that this is a real risk: Medium-High.
- **Vector also sells ASPICE consulting and integration services** to the same buyers, so a partnership comes with channel conflict [Data + Opinion].

## Yellow Flags
- Security-module automation could appear in a 2027 release; there is no public signal yet [Opinion].
- Revenue (2023) and headcount (Sep 2025) data are **more than 12 months old**; services revenue is unknown.
- AUTOSAR Core Partner date conflict (Jan 2025 vs Jan 2026).
- Conflict on whether 6.4 already "applies small changes".
- No public buyer reviews exist, so sentiment is inferred from forums and vendor messaging.
- VxLabs (Giza) claims Vector as a logo; if that is a real partnership, a Cairo competitor may already sit closer to Vector than the founders.

## Data Gaps
- **Vector licence terms for service providers, subcontractors and AI/automation use** (the highest-priority gap). **Fill:** ask Vector sales or a CEEP partner; ask one target Tier 1 how its MICROSAR licence treats subcontractors.
- AI subscription pricing and whether it is bought by the licence holder or can be bought by a service provider.
- Whether AI workflows will cover CSM/CryIf/SecOC/KeyM/HSM configuration, and when.
- CEEP fees, requirements, lead-referral practice, and whether Vector accepts AI-native or Egypt-based partners.
- Vector revenue 2025/26 and the services share; current headcount.
- MICROSAR licence prices (only hearsay ranges exist).
- Leadership, founding narrative and patents.
- Vector Congress exhibitor and partner list.
- Nature of the VxLabs "trusted by Vector" relationship.

## Sources
- Vector, DaVinci Configurator Gen 6 (fetched 2026-10-24): https://www.vector.com/en/product/microsar-classic/davinci-configurator-new-generation/
- Vector, DaVinci Configurator Classic: https://www.vector.com/en/product/microsar-classic/davinci-configurator-classic/
- Vector help, AI Assistant (fetched 2026-10-24): https://help.vector.com/davinci-configurator-classic/en/latest/user-manual/ui-client/views/ai-agent-view.html
- Vector help, Automation Interface (v3.9.0, 11 Mar 2026): https://help.vector.com/davinci-configurator-classic/en/6.3/user-manual/automation/automation.html ; https://help.vector.com/davinci-configurator-classic/en/latest/user-manual/automation/_attachments/AutomationInterfaceDocumentation.pdf
- Vector release notes 6.2 (2025-26): https://help.vector.com/davinci-configurator-classic/en/6.3/user-manual/ressources/release-notes/release-notes-dvcb-6.2.html
- Vector help, licensing and package delivery: https://help.vector.com/DaVinci-Package-Manager/current/en/Help/html/licensing_requirements_for_tool_actions.html ; https://help.vector.com/DaVinci-Package-Manager/current/en/Help/html/custom_package_vs_package_based_delivery.html
- Vector PR, VectorCAST 2026 AI test creator (Mar 2026): https://www.vector.com/en/company/press/press-releases/vectorcast-2026-launches-ai-powered-requirements-based-test-creator/
- Vector, ASPICE consulting: https://www.vector.com/en/business-unit/consulting/consulting-services/transformation/automotive-spice/
- Vector, Premium Partner Plus: https://www.vector.com/en/business-unit/software-platform/resources/vector-is-now-premium-partner-plus-pp-at-autosar/
- AUTOSAR, new Core Partners (file dated 15 Jan 2025): https://www.autosar.org/fileadmin/user_upload/2025_01_15_AUTOSAR-PR_New_Core_Partner.pdf
- Intellias, Vector certification (Sep 2023, >12 months old): https://intellias.com/intellias-strengthens-embedded-software-expertise-through-vector-certification/ ; Intellias CES 2025: https://intellias.com/shaping-the-future-of-sdvs-intellias-partnerships-with-vector-elektrobit-qnx-at-ces-2025/
- Teoresi, Vector partnership (2024): https://www.teoresigroup.com/partnership/vector/
- Wikipedia, Vector Informatik (revenue 2023, RocqStat Jan 2026): https://en.wikipedia.org/wiki/Vector_Informatik
- Revelio Labs, Vector headcount (Sep 2025): https://www.reveliolabs.com/companies/vector-informatik/employees
- MathWorks partner page: https://cn.mathworks.com/products/connections/product_detail/product_35766.html
- Capgemini job ad, Classic AUTOSAR integration with DaVinci (Mar 2026): https://careers.capgemini.com/job/Katowice-Software-Integration-Engineer/1282380001
- eeNews Europe, ST and ARCCORE (ARCCORE acquired by Vector Jul 2018, >12 months old): https://www.eenewseurope.com/en/st-arccore-in-joint-focus-to-cut-costs-in-autosar-development/
- btw.media commentary on Vector lock-in (snippet): https://btw.media/en/vector-informatik-must-make-vehicle-software-complexity-pay
- Infineon community integration threads (2019-2021, >12 months old): https://community.infineon.com/t5/AURIX/MCU01803-Invalid-XPath-error-by-Tresos-generator-for-TC33x/m-p/318684 ; https://community.infineon.com/t5/AURIX/MCAL-Generation-issue/m-p/318481
- CB Insights, Elektrobit vs Vector (unverified claims): https://www.cbinsights.com/compare/elektrobit-vs-vector-informatik
- AutoC blog (unverified): https://www.autoc-tool.com/en/blog/

---

## Implications for the founders

### What Vector will likely do in the next 12-24 months [Opinion unless noted]
1. **Ship AI configuration modification (6.5, Dec 2026)** [Data] and deepen ECU SDK agentic workflows during 2027.
2. **Convert AI to subscription revenue from July 2027** [Data], making AI a recurring upsell on the MICROSAR installed base.
3. **Extend agents to more modules, possibly the security stack.** Confidence: Medium.
4. **Grow ASPICE 4.0 consulting and assessments** and keep services tied to licence accounts.
5. **Keep the CEEP partner channel** as a way to scale MICROSAR integration without growing its own headcount. Confidence: Medium.

### Where the founders must NOT compete
- **"Our AI agents configure AUTOSAR BSW" as the headline message.** Vector owns the ground truth and ships the agent loop in the licensed tool. Expected durability of that message: under 1 year (C3).
- **Single-stack MICROSAR configuration** where the buyer's default is "call Vector" and Vector's own AI does the job.
- **ASPICE consulting and formal assessments** (ASPICE4Check, authorised assessments). Vector sells these, and competing here kills any partnership.
- **Building a rival configurator or generator.** Licensed BSWMD, validators and generators cannot be replicated.

### Where the founders can win
- **Cross-vendor integration:** Vector BSW plus EB tresos MCAL plugins plus ETAS CycurHSM or MCU-vendor HSM firmware, which no single vendor automates [Opinion based on Data]. Confidence: Medium-High.
- **Security implementation outcomes on specific targets:** HSM, secure boot, SecOC, Csm/CryIf/KeyM on AURIX TC3xx/TC4x and TRAVEO T2G, verified on hardware and linked to the TARA. Vector's AI does not mention security-stack automation [Data: absence].
- **Independent verification and evidence layer:** deterministic checks around Vector's own (self-declared fallible) AI, producing ISO 26262-8 / 21434 tool-confidence arguments and ASPICE-ready records. Assessors ask "is the AI use controlled?", and Vector does not verify outside its own stack.
- **Customer-project integration labour.** Vendors rarely do this at scale; Vector services are premium and capacity-limited [Assumption].
- **Use Vector's AI as an engine, not a rival.** Drive DaVinci through its Automation Interface, EcuC-as-Code and MCP with the customer's licence, inside the customer's environment.

### Partnership possibility
- **Vector CEEP / CEP certification: High value, Medium feasibility** [Opinion]. It is the most proven route for an emerging-market ESP to gain credibility without OEM references (Intellias precedent). Recommended first steps: CEP training for both founders, then a CEEP application once there is one MICROSAR reference. Position as a **delivery partner for MICROSAR security integration**, never as an ASPICE consultancy.
- **Gate 0 before building the delivery model:** confirm with Vector (or a CEEP partner) whether a third-party provider may run automation and AI agents on a customer's MICROSAR/DaVinci licence, and who must buy the AI subscription. If the answer is unfavourable, the model falls back to AI-assisted engineers on customer VDIs, with lower margins.
- **Subcontracting from Vector: Low-Medium** [Opinion]. Vector may need overflow capacity for security integration, but it has no public subcontracting programme, and lead referral is not a stated CEEP benefit.
- **Risk to manage:** a partnership gives Vector visibility into the founders' methods while Vector builds competing AI. Share delivery capability, not the verification harness or the configuration-pattern corpus.
- **Investor framing:** be explicit that Vector is both gatekeeper and competitor, show the Gate 0 licence answer, and show why the cross-vendor security and evidence layer survives Vector's AI roadmap. Investors in this space will know Vector's 2026-27 AI plans.
