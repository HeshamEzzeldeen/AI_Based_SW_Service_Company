# Competitor Check: FESCARO
Status: Complete. 8 of 8 search/fetch calls used. Written 2026-10-25.

Labels: [Data] / [Estimate] / [Opinion], with confidence H/M/L. Flagged: data older than 12 months.

## 1. Scope: what FESCARO actually sells
- [Data, H] Infineon lists FESCARO as a "PREFERRED Partner" design house. The listing describes an "all-in-one solution for automotive cybersecurity": certification consulting, TARA, HSM solution, engineering and testing, applied to up to 7 vehicle types and 150+ ECUs. Source: https://www.infineon.com/cms/en/partner-network/microcontroller-partners/preferred-design-houses/fescaro/ (page date not visible).
- [Data, H] Its own site lists automotive services (one-stop regulatory compliance, CSMS consulting, TARA, "Cybersecurity solution (HSM)", cybersecurity engineering, cybersecurity testing, Security Gateway) and IT platforms (CSMS portal, KMS, VSOC-style threat management, SUMS, certification management). It also lists an SDV controller, V2X security and EV-charger security. The site names no MCU vendors or AUTOSAR modules. Source: https://www.fescaro.com/en/ (fetched 2026-10-25).
- [Data, M] The HSM product is "FAST HSM", HSM firmware for ECU firmware integrity. Sister products are FAST IDS and FAST VTI. Source: https://simplywall.st/stocks/kr/software/kosdaq-a0015s0/fescaro-shares (2025-2026).
- [Data, M] It has run mass-production tests on about 155 controllers and 60 semiconductor types. This suggests multi-vendor chip support rather than Infineon only. Source: https://www.koreaherald.com/article/10541258 (2025-07-28).
- [Data, M] A 2023 release says FESCARO built HSM-compatible software that let a global OEM meet security requirements without replacing existing chips. Source: https://www.businesswire.com/news/home/20231123354338/de (2023-11-23, OLDER THAN 12 MONTHS).
- [Data, M] Its CTO wrote that OEMs now require Secure Debug, Secure Flash and SecOC from controller developers, and that this drives demand for its KMS. Source: https://www.koreaherald.com/article/10428259 (2025).
- [Estimate, M] FESCARO's delivery is product-led. It integrates its own HSM firmware and KMS into customer ECUs, and its engineering and consulting services sit around that product. No source shows it configuring or integrating third-party AUTOSAR Classic security BSW (Csm/CryIf/SecOC/KeyM from Vector MICROSAR, EB tresos or ETAS RTA-CAR) as a service separate from its own product.
- DATA GAP: There is no public list of supported MCUs, AUTOSAR stacks, or AUTOSAR modules (Csm/CryIf/SecOC/KeyM). "60 semiconductor types" is not broken down by vendor.

## 2. Pricing model
- DATA GAP: No pricing is published.
- [Estimate, L] The likely model is product licence/royalty for FAST HSM, IDS and KMS, plus project fees for consulting and testing. Quarterly revenue (KRW 4-6.5bn) is lumpy, which fits project billing. No fixed-price offer was seen.

## 3. Customers, geography, size, funding
- [Data, H] Founded 2016, headquartered in Suwon, Korea. Only Korean addresses appear on its site. Source: fescaro.com.
- [Data, H] Revenue was KRW 14.3bn (~$10M) in 2024, up from KRW 1.9bn in 2021, with operating profit in four consecutive years. It had raised about KRW 30bn before its IPO. Source: Korea Herald 2025-07-28.
- [Data, M] It listed on KOSDAQ in December 2025. The offer priced at KRW 15,500, valuing the company at about KRW 149.8bn (~$105M), and retail subscription was 1,430:1. The stock later traded far below its IPO price (one snapshot shows KRW 6,750 and -37% since IPO; dates of the quotes vary). Sources: https://finder.techleap.nl/news/feed/fescaro-ipo-draws-1-430-1-competition-ratio-collects-3-6t-in-deposits ; https://simplywall.st/stocks/kr/software/kosdaq-a0015s0/fescaro-shares ; https://www.google.com/finance/quote/0015S0:KOSDAQ
- [Data, M] Quarterly revenue from Jun-2025 to Mar-2026 was about KRW 4.06bn, 4.53bn, 4.84bn and 6.55bn. Source: Google Finance snapshot (snapshot date unclear).
- [Data, M] Customers: KG Mobility (UNECE R155 work, 2021-2023), parts makers supplying SsangYong, Hyundai and "overseas automakers", plus tractor and construction-equipment makers (EU CRA). Investors include Hyundai Technology Investment. Sources: Korea Herald 2025-07-28; https://www.cbinsights.com/compare/fescaro-vs-osr-enterprises
- [Opinion, M] Its business is Korea-centric, with Hyundai-group-adjacent and KGM supply chains. It mentions "overseas automakers" and plans to sell abroad through an online platform. No EU or US office was found.

## 4. AI claims
- [Data, M] None were found on its site or in the Korea Herald profile. The CSMS Portal (July 2025) is described as "automated" (process abstraction, ALM, virtual SOC), not as AI or agents.

## 5. Other "security integration as a package" sellers seen
- [Data, H] Vector: MICROSAR HSM firmware is certified to ISO/SAE 21434 (2025-06), and vHSM covers SecOC and secure boot and plugs into any AUTOSAR BSW. This is a product, sold with Vector's own services. Sources: https://www.electropages.com/2025/06/hsm-firmware-ecus-has-been-successfully-certified-according-isosae-21434 ; https://www.newelectronics.co.uk/content/news/vector-hsm-firmware-for-ecus-certified-according-to-isosae-21434
- [Data, H] ETAS/ESCRYPT: CycurHSM 3.x is integrated into Infineon AURIX TC4x (2024-04) and has long been paired with Renesas RH850. It is again a product plus vendor services. Sources: https://infineon.com/cms/jp/about-infineon/press/market-news/2024/INFATV202404-098.html ; https://www.renesas.com/en/about/press-room/renesas-electronics-and-escrypt-collaborate-state-art-combined-hardwaresoftware-solution-high-level
- [Data, M] Autocrypt sells an HSM software module with its own CryIf, Crypto Driver and FBL manager for AUTOSAR Classic. It is product-led. Source: https://autocrypt.io/products/hsm/
- [Data, M] eInfochips (an ESP) has a case study of Vector HSM and CS-module integration plus SecOC deployment on an ADAS ECU. This is the closest match to "third-party stack integration as a service", but no fixed price or evidence package was seen. Source: https://einfochips.com/automotive-cybersecurity/ (date not checked).
- [Data, M] wolfSSL wolfHSM is an open-source HSM layer with an AUTOSAR shim (AURIX TC3xx, RH850; NXP S32G "coming soon"). It is a cheap alternative product, not a service. Source: https://wolfssl.com/products/wolfhsm/
- Not checked within budget: NXP/Renesas/ST design partners, and Embitel's security services (seen in results, not opened).

## Verdict
[Opinion, M] FESCARO weakens the absolute claim "no competitor sells this" but does not invalidate the narrow wedge. It sells a bundled offer (consulting, TARA, its own HSM firmware, engineering and testing) across many controllers and chip types, so "bundled security implementation plus compliance evidence" is not unique. The other parts remain unshown in any public source:
- (a) a fixed price;
- (b) neutrality across vendor stacks, meaning integration of other vendors' AUTOSAR security BSW (Vector/EB/ETAS Csm/CryIf/SecOC/KeyM) rather than its own HSM/KMS products;
- (c) ASPICE SWE evidence in addition to ISO 21434/R155 artefacts;
- (d) AI-agent delivery with published accuracy metrics;
- (e) EU/US presence. FESCARO is Korea-centric.

The HSM vendors (Vector, ETAS, Autocrypt, FESCARO) all sell their own stack with services attached. ESPs such as eInfochips integrate third-party stacks, but on T&M without packaged evidence.

**Suggested wording:** "Security vendors such as Vector, ETAS, Autocrypt and FESCARO bundle their own HSM firmware with services. We found no provider that sells fixed-price, stack-neutral integration of the customer's chosen AUTOSAR security BSW (Csm/CryIf/SecOC/KeyM, HSM, secure boot, key provisioning) with ISO 21434 and ASPICE evidence included." Drop "no competitor sells this". Name FESCARO as the closest bundled alternative in Korea and on Infineon platforms.

## Data gaps
- FESCARO MCU/stack support list, and whether it integrates third-party AUTOSAR security BSW.
- FESCARO pricing and contract model, and its revenue split by product versus service.
- Named overseas OEM customers and any EU/US entity.
- Content of https://www.koreaherald.com/article/10632567 (in results, not read).
- NXP/Renesas/ST design-partner offers, Embitel, and Autocrypt services were not checked.

## Sources
- https://www.infineon.com/cms/en/partner-network/microcontroller-partners/preferred-design-houses/fescaro/
- https://www.fescaro.com/en/
- https://www.koreaherald.com/article/10541258 (2025-07-28)
- https://www.koreaherald.com/article/10428259
- https://www.businesswire.com/news/home/20231123354338/de (2023-11-23)
- https://simplywall.st/stocks/kr/software/kosdaq-a0015s0/fescaro-shares
- https://finder.techleap.nl/news/feed/fescaro-ipo-draws-1-430-1-competition-ratio-collects-3-6t-in-deposits
- https://www.google.com/finance/quote/0015S0:KOSDAQ
- https://www.cbinsights.com/compare/fescaro-vs-osr-enterprises
- https://autocrypt.io/products/hsm/
- https://wolfssl.com/products/wolfhsm/
- https://einfochips.com/automotive-cybersecurity/
- https://www.electropages.com/2025/06/hsm-firmware-ecus-has-been-successfully-certified-according-isosae-21434
- https://infineon.com/cms/jp/about-infineon/press/market-news/2024/INFATV202404-098.html
