# Faktatjek og dataopdatering, 2. oktober 2026

Denne fil dokumenterer, hvad der er rettet og opdateret i `index.html`, og hvor sikre tallene er.

## Sådan er der tjekket

| Sikkerhed | Hvad det betyder | Gælder for |
|---|---|---|
| **Primærkilde læst** | Tallene er læst direkte i selskabets egen PDF/fil | Google 2025- og 2026-rapporten (datatabellerne), Metas Llama-modelkort på GitHub |
| **Sekundært verificeret** | Tallene er krydstjekket i flere uafhængige nyhedskilder/databaser, men primær-PDF'en kunne ikke hentes fra arbejdsmiljøet | Microsoft FY25, Amazon 2025, Apple FY25, NVIDIA FY26, Tencent 2025, Mistral-LCA, IEA 2026, IATA, EDGAR |
| **Ikke verificeret** | Står uændret, men kunne ikke bekræftes | Se afsnittet "Åbne punkter" |

Netværkspolitikken i arbejdsmiljøet blokerede de fleste selskabers domæner, så tal i kategorien "sekundært verificeret" bør efterses i de linkede PDF'er, før de bruges i undervisning eller presse.

## Fejl der er rettet

| # | Hvad | Før | Efter | Kilde |
|---|---|---|---|---|
| 1 | **Googles tidsserie var forskudt et år.** 2023 var en kopi af 2022, og "2024" var i virkeligheden 2023-tallet. Changeloggen i HTML'en påstod fejlagtigt, at 14,2968 Mt var 2024. | 2023: 11,90 · 2024: 14,30 Mt | 2023: 14,92 · 2024: 15,94 · 2025: 18,85 Mt (omregnet serie fra 2026-rapporten) | Google Environmental Report 2025, s. 104, og 2026, s. 89 |
| 2 | Googles Scope 3 for 2024 manglede ca. 0,9 Mt | 11,16 Mt | 12,97 Mt (2026-rapportens omregning) | Samme |
| 3 | **Amazon blandede to metoder.** 2020-2021 er efter den gamle metode, 2022-2024 efter den nye. Faldet fra 71,5 til 65,1 Mt er derfor delvist et metodeskift. | Ingen note | Note i kildeteksten; 2023-2024 opdateret til 2025-rapportens omregnede tal (65,28 / 69,55 Mt) | Amazon Sustainability Report 2024 og 2025 |
| 4 | **NVIDIAs regnskabsår var vist et år for sent.** NVIDIA FY2025 sluttede 26. jan. 2025 og er i praksis kalenderåret 2024. | FY23-FY25 vist som 2023-2025 | Vist som 2022-2024, og FY26 som 2025 | NVIDIA Sustainability Report FY2025/FY2026 |
| 5 | **Alibabas regnskabsår ditto.** FY2025 = apr. 2024 – mar. 2025. | Vist som 2024-2025 | Vist som 2023-2024 | Alibaba ESG |
| 6 | Microsoft brugte 2025-faktaarkets serie; 2026-faktaarket har omregnet hele serien ("management's criteria") | Baseline 2020: 12,37 Mt | Baseline 2020: 12,88 Mt; FY25: 20,29 Mt | Microsoft 2026 Environmental Data Fact Sheet, Table 1B |
| 7 | Apples Scope 3 FY2024 passede ikke med totalen på 15,3 Mt | 15,11 Mt | 15,23 Mt | Apple EPR 2026 (via Tracenable) |
| 8 | **Cement-benchmark matchede ikke kilden.** Den citerede Global Carbon Project-datasæt dækker kun procesemissioner (ca. 1,6 Gt). | 2.600 Mt "proces + varme" | 1.610 Mt (proces), med note om ca. 2,5-2,7 Gt inkl. brændsel | Global Carbon Project / Andrew (Zenodo) |
| 9 | "International luftfart": IATA-tallet dækker alle flyselskaber, også indenrigs | "International luftfart" | "Luftfart (alle flyselskaber)" | IATA Chart of the Week, 28. nov. 2025 |
| 10 | Googles målbane gik til 0 i 2030, men Googles faktiske reduktionsmål er -50% ift. 2019 (resten skal neutraliseres med removals). Nu samme princip som Microsoft og Apple. | 2020 → 0 i 2030 | 2019 (10,35 Mt) → 5,18 Mt i 2030 | Google Environmental Report 2026 |
| 11 | Amazons målbane startede i 2020; The Climate Pledge er fra 2019 | Baseline 2020: 60,64 Mt | Baseline 2019: 51,17 Mt | Amazon |
| 12 | Anthropic-kortet viste Ai2's OLMo-tal (493 t), som ikke har noget med Anthropic at gøre | OLMo-tal under Anthropic | Flyttet til egen række "Ai2 (OLMo)" i fanen AI-selskaber | arXiv 2503.05804 |

## Nye data (2025-tal)

| Selskab | Nyeste total | Ændring | Kilde |
|---|---|---|---|
| Microsoft (FY25, jul. 2024 – jun. 2025) | 20,29 Mt CO2e | +25% på ét år, ca. +58% vs. 2020 | 2026 Environmental Data Fact Sheet |
| Google (2025) | 18,85 Mt (fuld GHGP) / 14,47 Mt ("ambition-based") | +18% på ét år, +82% vs. 2019 | Environmental Report 2026 |
| Amazon (2025) | 80,85 Mt | +16% på ét år, +58% vs. 2019 | Sustainability Report 2025 |
| Apple (FY25) | ca. 15,3 Mt brutto | stort set fladt vs. FY24, over 60% under 2015 | Environmental Progress Report 2026 |
| NVIDIA (FY26 ≈ 2025) | 10,71 Mt (Scope 3: 10,70 Mt) | Scope 3 næsten tredoblet siden FY24 | Sustainability Report FY2026 |
| Tencent (2025) | 5,97 Mt | lidt under 2024, over 2022 | ESG Report 2025 |
| IEA (2025) | 485 TWh datacenter-el, heraf 155 TWh AI-fokuseret | +17% / +50% | Key Questions on Energy and AI, april 2026 |

## AI-selskaber (ny fane og nye datakort)

* **Mistral AI** (nyt): Ingen årlig Scope 1+2+3. Livscyklusanalyse af Mistral Large 2 (med Carbone 4 og ADEME, juli 2025): 20,4 kt CO2e, 281.000 m3 vand, 660 kg Sb eq for træning + 18 måneders brug; 1,14 g CO2e og 45 ml vand pr. svar på 400 tokens. Udbygger compute fra ca. 44 MW (Essonne, 2026) mod ca. 1 GW i 2030.
* **xAI** (nyt): Ingen klimadata. Clean Air Act-sag (april 2026) om gasturbiner uden tilladelse ved Colossus 2.
* **OpenAI**: Ingen opgørelse eller klimamål. Eneste officielle tal: 0,34 Wh og ca. 0,32 ml vand pr. "gennemsnitlig forespørgsel" (Sam Altman, juni 2025).
* **Anthropic**: Ingen opgørelse eller klimamål. Har tilsluttet sig carbon removal-koalitionen Frontier (juni 2026), men ingen annoncerede aftaler om ren strøm.
* **Meta Llama** (primærkilde): Llama 3.1 træning 11.390 t CO2e, Llama 4 Scout+Maverick 1.999 t CO2e (lokationsbaseret; Meta angiver 0 t market-based).
* **Californien SB 253**: Scope 1+2 for amerikanske selskaber over 1 mia. USD omsætning skal indberettes senest 10. november 2026, og det kan give de første officielle tal for OpenAI, Anthropic og xAI.

## Tendens-emojis og standardvalg

Tendensen beregnes automatisk ud fra total Scope 1+2+3 fra første til seneste rapporterede år:

| Emoji | Betydning | Selskaber (2. okt. 2026) |
|---|---|---|
| 🔴📈 | Stigende (dårligt) og **valgt som standard** | Microsoft +58%, Google +101%, Amazon +33%, Meta +60%, NVIDIA +199%, Tencent +4% |
| 🟡📉 | Faldende, men ikke i mål (middel) | Apple -32%, Samsung -8%, Alibaba -15%, Baidu -6% |
| 🔬 | Ingen årstal, men åben livscyklusanalyse | Mistral AI (og Ai2 i AI-tabellen) |
| ⚪❔ | Ingen tal offentliggjort | OpenAI, Anthropic, xAI |
| 🟢 | På sporet mod netto-nul | Ingen endnu |

Bemærk: Efter reglen er ikke kun Apple, men også Samsung, Alibaba og Baidu faldende og derfor fravalgt som standard. Tencent er "stigende" over hele perioden (+4% fra 2022), selvom 2025 var lidt lavere end 2024. Knappen "Stigende" i filteret genskaber standardvalget.

## Åbne punkter

* **Meta 2025-tal** var ikke offentliggjort pr. 2. oktober 2026.
* **Samsung 2026-rapporten** (2025-tal) udkom 26. juni 2026, men tallene kunne ikke verificeres fra en troværdig kilde og er ikke lagt ind.
* **Baidu og Alibaba**: nyere tal er ikke fundet/verificeret.
* **Tencent 2025**: kun totalen er lagt ind, ikke fordelingen på scopes.
* **Microsoft Scope 3** er beregnet som total minus Scope 1 og 2 (Table 1B).
* **Amazon 2023 Scope 3** er beregnet som omregnet total minus Scope 1 og 2.
* Ikke efterprøvet: "Communications Earth & Environment: 32 elementer i en A100 GPU" (fanen AI's ressourceforbrug).
