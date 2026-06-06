# Danske Insider Threats — Kort version (IT-sikkerhed)
**Oprettet:** 2026-04-27  
**Formål:** Kort, kildeunderstøttet overblik med 4 prioriterede cases + ITM-mapping af resterende cases.

## Metode og ramme
Denne version bruger **Insider Threat Matrix (ITM)** som klassifikationsramme:  
[Motive (AR1)](https://insiderthreatmatrix.org/articles/AR1) · [Means (AR2)](https://insiderthreatmatrix.org/articles/AR2) · [Preparation (AR3)](https://insiderthreatmatrix.org/articles/AR3) · [Infringement (AR4)](https://insiderthreatmatrix.org/articles/AR4) · [Anti-Forensics (AR5)](https://insiderthreatmatrix.org/articles/AR5)

---

## 4 prioriterede, forskellige cases

### 1) Netcompany (2024) — læk + afpresning via kompromitteret kundeadgang
**Kort:** Gerningsmanden tilgik kode/adgangsdata via kompromitteret kundekonto og forsøgte afpresning.

| ITM-dimension | Mapping |
|---|---|
| Motive | [Personal Gain (MT005)](https://insiderthreatmatrix.org/articles/AR1/sections/MT005) |
| Means | [Delegated Access via Managed Service Providers (ME028)](https://insiderthreatmatrix.org/articles/AR2/sections/ME028) + [Access (ME024)](https://insiderthreatmatrix.org/articles/AR2/sections/ME024) |
| Preparation | Ikke offentligt dokumenteret |
| Infringement | [Data Loss (IF022)](https://insiderthreatmatrix.org/articles/AR4/sections/IF022) + [Exfiltration via Web Service (IF001)](https://insiderthreatmatrix.org/articles/AR4/sections/IF001) |
| Anti-Forensics | Ikke offentligt dokumenteret |

**Kilder:**
- [Version2](https://www.version2.dk/artikel/datatyveri-mod-netcompany-satte-it-danmark-paa-den-anden-ende-saadan-haandterer-du-insider-truslen)
- [DR](https://www.dr.dk/nyheder/indland/politiet-anholder-mand-i-sag-om-datatyveri-mod-netcompany)
- [TV2](https://nyheder.tv2.dk/live/krimi/2024-02-27-34-aarig-mand-sigtet-for-hackerangreb-mod-netcompany)

### 2) Københavns Kommune/CPR (2025) — intern datalæk til kriminelle
**Kort:** Studentermedhjælper med legitim adgang solgte CPR-relaterede persondata til kriminelle netværk.

| ITM-dimension | Mapping |
|---|---|
| Motive | [Third Party Collusion Motivated by Personal Gain (MT006)](https://insiderthreatmatrix.org/articles/AR1/sections/MT006) |
| Means | [Access (ME024)](https://insiderthreatmatrix.org/articles/AR2/sections/ME024) |
| Preparation | Ikke offentligt dokumenteret |
| Infringement | [Data Loss (IF022)](https://insiderthreatmatrix.org/articles/AR4/sections/IF022) + [Exfiltration via Messaging Applications (IF005)](https://insiderthreatmatrix.org/articles/AR4/sections/IF005) |
| Anti-Forensics | Ikke offentligt dokumenteret |

**Kilder:**
- [The Local](https://www.thelocal.dk/20250718/copenhagen-ex-public-employee-arrested-for-suspected-leak-of-address-data)
- [CPH Post](https://cphpost.dk/2025-07-16/news/round-up/ex-copenhagen-municipality-employee-arrested-for-selling-cpr-info-to-gangs-to-aid-murders/)

### 3) Tidligere IT-chef (Højesteret, 2018) — destruktiv sabotage efter fratræden
**Kort:** Tidligere IT-chef slettede centrale systemressourcer efter fratræden; Højesteret skærpede straffen.

| ITM-dimension | Mapping |
|---|---|
| Motive | [Revenge (MT023)](https://insiderthreatmatrix.org/articles/AR1/sections/MT023) |
| Means | [Unrevoked Access (ME021)](https://insiderthreatmatrix.org/articles/AR2/sections/ME021) + [Privileged Access (ME007)](https://insiderthreatmatrix.org/articles/AR2/sections/ME007) |
| Preparation | Ikke offentligt dokumenteret |
| Infringement | [Unauthorized Changes to IT Systems (IF014)](https://insiderthreatmatrix.org/articles/AR4/sections/IF014) |
| Anti-Forensics | Ikke offentligt dokumenteret |

**Kilder:**
- [Bird & Bird](https://www.twobirds.com/da/insights/2018/denmark/hoejesteret-slaar-haardt-ned-over-for-hacker)
- [Version2](https://www.version2.dk/artikel/saerlig-hackerdom-fra-hoejesteret-nu-ligger-det-fast-hacking-giver-lang-faengselsstraf)

### 4) Britta Nielsen/Socialstyrelsen (1993–2018) — langvarigt insiderbedrageri
**Kort:** Misbrug af finansiel godkendelsesadgang over årtier; 117 mio. kr. svindel; dom 6,5 år.

| ITM-dimension | Mapping |
|---|---|
| Motive | [Personal Gain (MT005)](https://insiderthreatmatrix.org/articles/AR1/sections/MT005) |
| Means | [Privileged Access (ME007)](https://insiderthreatmatrix.org/articles/AR2/sections/ME007) |
| Preparation | Delvist dokumentforfalskning i sagsmateriale |
| Infringement | [Misappropriation of Funds (IF016)](https://insiderthreatmatrix.org/articles/AR4/sections/IF016) |
| Anti-Forensics | Delvist dokumentforfalskning; fuldt teknisk forløb ikke offentligt |

**Kilder:**
- [DR (tema)](https://www.dr.dk/nyheder/tema/millionsvindel-i-socialstyrelsen)
- [DR (dom 6,5 år)](https://www.dr.dk/nyheder/indland/millionsvindel-i-socialstyrelsen-britta-nielsen-straffes-med-faengsel-i-65-aar)
- [Anklagemyndigheden](https://anklagemyndigheden.dk/da/dom-i-britta-nielsen-sag-staar-ved-magt)

---

## Mapping af resterende cases til ITM

| Resterende case | ITM-mapping (kort) | Kilder |
|---|---|---|
| Politiansat IT-medarbejder (140 kolleger) | Motive: mulig [Curiosity (MT018)](https://insiderthreatmatrix.org/articles/AR1/sections/MT018) / personligt motiv. Means: [Privileged Access (ME007)](https://insiderthreatmatrix.org/articles/AR2/sections/ME007). Infringement: [Installing Malicious Software (IF027)](https://insiderthreatmatrix.org/articles/AR4/sections/IF027) / [Data Loss (IF022)](https://insiderthreatmatrix.org/articles/AR4/sections/IF022). | [TV2 Østjylland](https://www.tv2ostjylland.dk/aarhus/politiansat-tiltalt-hackede-140-kolleger-i-dag-skal-han-i-retten), [DR](https://www.dr.dk/nyheder/seneste/tidligere-ansat-ved-politiet-tilstaar-hacking-af-140-kollegaers-telefoner) |
| SIRI masseadgang (2023) | Motive: uafklaret, mulig [Curiosity (MT018)](https://insiderthreatmatrix.org/articles/AR1/sections/MT018) eller [Lack of Awareness (MT008)](https://insiderthreatmatrix.org/articles/AR1/sections/MT008). Means: [Access (ME024)](https://insiderthreatmatrix.org/articles/AR2/sections/ME024). Infringement: potentiel [Data Loss (IF022)](https://insiderthreatmatrix.org/articles/AR4/sections/IF022). | [Nyidanmark/SIRI](https://www.nyidanmark.dk/da/Nyheder/2023/03/Databrud-i-SIRI) |
| Erling Smith, KK (17,7 mio.) | Motive: [Personal Gain (MT005)](https://insiderthreatmatrix.org/articles/AR1/sections/MT005). Means: [Privileged Access (ME007)](https://insiderthreatmatrix.org/articles/AR2/sections/ME007). Infringement: [Misappropriation of Funds (IF016)](https://insiderthreatmatrix.org/articles/AR4/sections/IF016). | [DR](https://www.dr.dk/nyheder/indland/tre-aars-faengsel-til-svindleren-i-koebenhavns-kommune), [Transparency DK](https://transparency.dk/svindler-fra-koebenhavns-kommune-skal-tre-aar-i-faengsel/) |
| Atea/Region Sjælland | Motive: [Third Party Collusion Motivated by Personal Gain (MT006)](https://insiderthreatmatrix.org/articles/AR1/sections/MT006). Means: [Access (ME024)](https://insiderthreatmatrix.org/articles/AR2/sections/ME024). Infringement: [Misappropriation of Funds (IF016)](https://insiderthreatmatrix.org/articles/AR4/sections/IF016) / bestikkelseslignende mønster. | [DR](https://www.dr.dk/nyheder/indland/it-leder-i-region-sjaelland-dommes-atea-bestikkelse), [Version2](https://www.version2.dk/artikel/alle-kendt-skyldige-atea-sag-strengeste-straf-paa-halvandets-aars-faengsel-1085546), [Østre Landsret](https://www.domstol.dk/oestrelandsret/aktuelt/2019/7/dom-i-atea-sagen/) |
| Pokerspiller/spyware | Ikke klassisk ansat-insider, men ITM-mønstret passer: Motive [Personal Gain (MT005)](https://insiderthreatmatrix.org/articles/AR1/sections/MT005). Preparation: [Software Installation (PR003)](https://insiderthreatmatrix.org/articles/AR3/sections/PR003). Infringement: [Installing Malicious Software (IF027)](https://insiderthreatmatrix.org/articles/AR4/sections/IF027). | [DR (tiltale)](https://www.dr.dk/nyheder/indland/tiltale-spiller-spionerede-modstandere-i-online-poker), [DR (endelig dom)](https://www.dr.dk/nyheder/seneste/pokerspiller-faar-tre-aars-faengsel-installere-spionprogram-hos-modstandere) |

---

## Kort konklusion (operativ)
1. **Højrisiko-klynger i materialet:** finansielt motiveret misbrug af privilegeret adgang, samt dataeksfiltration fra offentlige registre.  
2. **Kontrolsvigt der går igen:** utilstrækkelig adgangsbegrænsning, svag offboarding, og primært reaktiv opdagelse.  
3. **Praktisk prioritet:** styrk least privilege, SoD/4-øjne i betaling og registre, samt monitorering mod ITM-mønstre for data loss og misappropriation.
