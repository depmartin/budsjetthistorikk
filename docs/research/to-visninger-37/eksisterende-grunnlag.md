# #37: eksisterende primærgrunnlag og minste komplette visningssnitt

Kontrollert 23. oktober 2026 mot main `542316088cbca39e35d7b8f26cdd0aee0e96161c`. Dette er dokumentfunn og forslag til senere aksept, ikke funksjonsbygging eller en utført aksept av V1–V10. Ingen originaler, tidligere leveranser, produktkode eller GitHub-objekter er endret. #10 står fortsatt åpen for faktisk driftsaksept.

## Anbefalt første snitt

**Samordning 23. oktober:** Dette delnotatet vurderer først O1/O2-grunnlaget og første snitt. Den parallelle undersøkelsen har nå bevart [hele Innst. 95 S-grenen](forgrening.md), en [autentisk komitéendring](komiteendring.md) og [flere vedtaksrunder/år](konto-aar.md). Formuleringene nedenfor om det O1/O2 ikke bevarer gjelder disse tidligere leveransene; kildeportene og den samlede nåværende statusen står i [oversikten](README.md) og [testmatrisen](testmatrise.md).

Velg **hele Innst. 81 S (2024–2025), hele vedtak 210 og hele vedtak 211**, og kontoene 1429/1, 1429/22 og 1429/60 for budsjettåret **2024**. Ta med Prop. 16 S som kildebelagt foregående dokument: strukturer dens 1429-del, men vis samtidig hele proposisjonens kilde-/kontoinventar og merk resten som ustrukturert i piloten. Vis den andre grenen til sak 100889/Innst. 95 S med sitt eget omfang og faktisk kildestatus. Hele proposisjonen skal kunne åpnes; den skal ikke merkes som fullstendig strukturert dokumentvisning når bare 1429 er strukturert.

Dette gir en nyttig, liten ende-til-ende-leveranse for begge innganger uten å kreve generell proposisjonsimport først. Den krever likevel nye, separate forslags-/innstillingsobservasjoner og en eksplisitt dokument-/kontoavgrenset eksport. O2b er et godt bevisgrunnlag, men er ikke denne funksjonen. Komitéendring, alternative forslag og flerårig kontinuitet trenger andre autentiske kilder før de kan få positiv aksept. V2s årsdekning og V6/V7 oppfylles ikke av 210-kjeden alene. Kildegrunnlag: [V1–V10](../../to-visninger.md), [O1](../omtale-o1/README.md), [O2b](../omtale-o2b/README.md) og originalinventarene nedenfor.

## Lest mandat og kontrakt

AGENTS med arbeidsflyt, issue tracker, begrepsregler, ansvarsdeling, krav, kildefunn, observasjonsformat, datakontraktens B2/B3/B8/B9/O2-grenser, ADR 0003/0004/0010 og O1/O2a/O2b er grunnlaget. Hele de lokalt hentede #37/#32/#1 og kommentarene i `work/ticket-context/issue37.json`, `issue32.json` og `issue1.json` er lest. #32-kommentaren om PR #39 bekrefter O2b flettet til denne main; eldre tidsbundne formuleringer om «kandidat» i O2b-notatet er ikke nåværende mergestatus. Autoritative målkrav er [to-visninger.md](../../to-visninger.md), ikke en antatt utvidelse av pilotmandatet.

[Observasjonsformatet](../../observasjonsformat.md), [ADR 0003](../../adr/0003-felles-belopsobservasjoner.md), [datakontrakten](../../datakontrakt.md) og [GLOSSARY](../../../GLOSSARY.md) skiller talltype, forslagsrolle, behandlingsrunde, beløpsbetydning, kildeversjon og hendelse. Forslag/tilråding blir egne kildeobservasjoner; differanser blir avledede sammenligninger. Ingen av dem blir ekstra vedtatte hendelser. [ADR 0010](../../adr/0010-saksdokumenter-og-frosset-v2.md) avgrenser B8 til saksmetadata, og [ansvarsdelingen](../../ansvarsdeling.md) krever separate adaptere for nye kilder. Gamle parser-/tolkningsbetydninger, ID-er, råbyte, B5-kontrollgrunnlag, schema 5, frozen-v 1/v 2, gamle JSON-/Excel-filer og standardvalg er kompatibilitetskrav.

## Kilde- og kapabilitetsmatrise

Originalenes eksakte URL-er, HTTP-forsøk, tidsgrunnlag, byteantall og SHA-256 finnes i eksisterende [O1-manifest](../omtale-o1/source-manifest.json), [støttemanifest](../omtale-o1/supporting-manifest.json), [B8-fixturmanifest/sidevogner](../../../tests/fixtures/b8/README.md) og [B6-sidevogn](../../../tests/fixtures/b6/40034048.json). Originalene gjenbrukes; ingen nye «samlede» kildehasher konstrueres. Hashene nedenfor ble kontrollert direkte fra lokale originalbyte i denne undersøkelsen.

| Primærkilde og versjon | Bevart representasjon og SHA-256 | Hva den beviser | Implementert nå / rest for #37 |
| --- | --- | --- | --- |
| Prop. 16 S (2024–2025), tilrådd 22.11.2024, statsbudsjettet 2024 | [Full PDF, 12 sider](../omtale-o1/originals/prop16s.pdf), `677716056269c07b8ec81bcae91d814b975123791635548281038d9beb3aa5db` | Hele proposisjonen, 15 tabellkapitler, 37 eksakte endringsgrupper og fullmakter II–VI. | Hele bytegrunnlaget bevart. O2b strukturerer enkelte 1429-seksjoner og side 3 som representasjonsbelegg; ingen generell beløpsadapter eller helproposisjonsvisning. |
| Samme Prop., kapittel 2 | [Del-HTML](../omtale-o1/originals/prop16s-ch2.html), `258d26e6d324bde709bf3d1cb660d7eb6f4248f537d4b0c77e095f17697cf8df` | Postomtale, herunder 1429/1, /22 og /60; også andre kapitlers omtale. | P1, P22 og PN er strukturert av den avgrensede adapteren. Delrepresentasjon må ikke kalles komplett HTML. |
| Samme Prop., forslag til vedtak | [Del-HTML](../omtale-o1/originals/prop16s-ch4.html), `ff1c53688a155c2cb9d8d37a8d40550e56b5c5c1d2d171c30519ef49227eca5e` | To bevilgningstabeller og fullmaktsdelene. | PT/PT22 er beleggseksjoner for to poster; ingen selvstendige regjeringsforslagsbeløpsobservasjoner er importert. |
| Innst. 81 S (2024–2025), familie- og kulturkomiteen 09.12.2024 | [Hele HTML](../omtale-o1/originals/inns81s.html), `e7069d74e911fb868812bb34f68b41d210b4e33035c1317cbedd296ac1101e95`; [hele PDF, 2 sider](../omtale-o1/originals/inns81s.pdf), `5a29d0553991759d8ddc234899647e9e6b5e1f2885bf13edccfb26105a6be496` | Hele dokumentinventaret nedenfor, samlet komités støtte/tilråding, seks eksakte tabellbeløp og stikkordsfullmakt. | K1/K22/KS/KT er strukturert tekst. KT inneholder I og II; det betyr ikke at egne komitébeløpsobservasjoner eller /60-fullmaktsobjekt finnes. Sammendragets /60 har ikke egen O2b-seksjon. |
| Plenumsreferat 16.12.2024, sak 25 | [Bevart HTML](../omtale-o1/originals/votering-161224.html), `22170a60f769e89642b2e52525899903020de25938aa2b566ea28d11f85fb2e5` | `#2024-12-16-25` navngir Prop. 16 S kap. 1429/Innst. 81 S, gjengir I og II og dokumenterer enstemmig vedtakelse. | V er strukturert belegg; plenumsreferatet er ikke en ny beløpskilde som skal gi ekstra vedtatte hendelser. |
| Vedtak 210/40034048, sak 100927, 16.12.2024 | [XML-utdrag](../../../tests/fixtures/b6/40034048.xml), 6 058 byte, `2a540261f110b761a0213516c8ad72844d0285744ca0f1cdd4cb1afce06f0850` | Del I: to vedtatte postendringer med før-/etterbeløp for 2024. | Seks eksisterende beløpsobservasjoner, to `step_id`. Utdrag av fullrespons, ikke ny komplett API-respons. Forelder/byteposisjon står i sidevognen. |
| Vedtak 211/40034049, samme sak/dato | [XML-utdrag](../../../tests/fixtures/b8/40034049.xml), 1 692 byte, `5f253a556d2ac512570899252b396bc38f068de5f4bd6820178e7de8ce41f3eb` | Del II: samtykke til «kan overføres» på 1429/60 i 2024. Type ANNET. Ingen beløpsrad. | B8 bevarer fullteksten. Eget kildebelagt fullmaktsledd er nødvendig i komplett dokumentvisning; ingen tredje beløpshendelse. [Sidevogn](../../../tests/fixtures/b8/40034049.json) viser byteutdrag fra fullrespons. |
| Saks-API 100927 | [Komplett XML](../../../tests/fixtures/b8/sak-100927.xml), 12 383 byte, `2ee25b327b78772523d56317c752e35f5134eef60db9536f6dea3c94ad8fed27` | Prop. 16 S **kap. 1429**, Innst. 81 S, referater og `sammekilde` 100889. | B8 saksberikelse er implementert; referanser er ikke automatisk postbevis. |
| Saks-API 100889 | [Komplett XML](../../../tests/fixtures/b8/sak-100889.xml), 15 888 byte, `3a8f0918a3fcce90bf2c93f3ce972c3de7277c76e27e5ef563d6c43384cf2af2` | Samme Prop. 16 S **unntatt kap. 1429**, Innst. 95 S, referater 18.12.2024 og motsatt `sammekilde`. | Faktisk forgrening, men Innst. 95 S-fulltekst og dens postvise resultat er ikke bevart/undersøkt av O1/O2. Slike resultater må ikke arves fra 81 S. |

[B8s kontrolluttrekk](../b8/source-observations.json) angir presise navneromsbundne lokatorer for alle saksreferanser. I begge saksoriginaler er `/detaljert_sak/henvisning` kapittelavgrensningen; `/publikasjon_referanse_liste/publikasjon_referanse[1]` peker til proposisjonen, `[3]` til den respektive innstillingen, `[4]` til behandling og `[5]` til votering. `/sak_relasjon_liste/sak_relasjon[1]` har `relasjon_type=sammekilde` og den andre saks-ID-en. Proposisjonens eksport-ID er nil, ikke manglende dokumentidentitet. Referansene 4 og 5 har samme eksport-ID, men ulike URL-er; de må ikke kollapses. De konkrete XML-lokatorene har prefikset `/detaljert_sak` også der det er forkortet i denne teksten.

## Hele Innst. 81 S og vedtak 210/211: autentisk fasit

Hele den tosidige innstillingen er lest både fra bevart HTML og ny tekstuttrekking fra den hashkontrollerte PDF-en. Dokumentets eneste kapittel er **1429 Riksantikvaren**. Følgende inventar omfatter også omtale og fullmakt uten bevilgningstabellrad; «alle» betyr ikke bare 210s to poster.

| Del/lokator i full HTML | Konto/år, rolle og kildens beløpsutsagn | Hva som skal vises |
| --- | --- | --- |
| Tittel, `#m1`, `#m1_1`; PDF s. 1 | Prop. 16 S kap. 1429; endringer i statsbudsjettet **2024**, dokument i sesjon **2024–2025**. | Dokumentidentitet og budsjettår separat. Ingen årskonvertering fra sesjonen. |
| `#m1_1_1 > div.krnl_chapter > p`; PDF s. 1 venstre | 1429/1, komiteens **gjengivelse av regjeringen**: +3 mill. kroner til stillinger, finansiert fra /22; videre anslått +2,8 mill. som følge av lønnsoppgjøret 2024; samlet foreslått +5,8 mill. | Hele originalavsnittet, avrunding og forslagsrolle. 3 mill. gjelder konsulent-/stillingsomdisponering, ikke hele tabelløkningen. Resten 2 796 000 ved subtraksjon er en beregning, ikke et eksakt kildeobservert lønnsbeløp. |
| `#m1_1_2 > div.krnl_chapter > p`; PDF s. 1 venstre | 1429/22, samme gjengivelsesrolle: −3 mill. omdisponeres til /1. Omtalen sier «kulturmiljøforvaltning». | Egen tekst, uttrykkelig mottakerkonto og kildepresisjon. Ikke egen ekstra vedtatt komponent. |
| `#m1_1_3 > div.krnl_chapter > p`; PDF s. 1 | 1429/60, gjengivelse: posten **ble økt med 5 mill. i RNB**, knyttet til Vega; grønt næringsfond **10 mill. totalt**, fordelt **5 mill. i 2024 og 5 mill. i 2025**; usikkert om midler utbetales 2024. Forslag om «kan overføres». | Alle beløps-/årsutsagn som historisk/fremtidig kontekst, med henvisning til underliggende RNB-grunnlag som hull. 10 mill. er fondets omtale, ikke nytt 2024-delta; 5 mill. for 2025 beviser ikke egen 2025-bevilgning/vedtak. Ingen null ved uteblitt utbetaling. |
| `#m2 > div > p`; PDF s. 1 høyre | Navngitte medlemmer fra Ap, H, Sp, FrP, SV og V støtter regjeringens forslag. Ingen ny beløpsangivelse. | **Samlet komité** som avsender. Støtte er egen relasjon, ikke ny tabellobservasjon eller vedtakelse. |
| `#m3`, innledende avsnitt; PDF s. 2 | «Komiteens tilråding fremmes av en samlet komité.» Ingen særskilt alternativ eller mindretall i dokumentet. | Kontrollert fravær i akkurat hele Innst. 81 S, ikke generell fraværsstatus for andre dokumenter eller fellesdebatt. |
| `#m3` → romertall `i` → `table/tbody`, rader 1–5; PDF s. 2 | Kapittelrad 1; /1 rader 2–3: **+5 796 000**, fra **160 243 000** til **166 039 000**; /22 rader 4–5: **−3 000 000**, fra **32 185 000** til **29 185 000**, kroner, budsjettår 2024. | Seks eksakte kildefelt med talltype `komiteforslag`, rolle `tilraading`, samme to konti, egne kildepekere. Tabellens rå post 22-navn er «Flerårige prosjekter kulturminneforvaltning, kan overføres». |
| `#m3` → `div[data-strtngt-romertallseksjon-romertall='ii']`; PDF s. 2 | Stikkordsfullmakt: KLD kan **i 2024** tilføye «kan overføres» til 1429/60 Kulturminnekompetanse i kommunene. **Ingen beløpsverdi.** | Eget fullmakts-/tekstledd, tilråding, ingen bevilgningsobservasjon som delta. |
| Sluttunderskrift; PDF s. 2 | Oslo, familie- og kulturkomiteen **09.12.2024**, Grunde Almeland leder og ordfører. | Dokument-/behandlingstid, ikke ny økonomisk hendelse. |

Vedtaks-XML har navnerom `http://data.stortinget.no`. Begge utdrag har hovedlokator `/stortingsvedtak_oversikt/stortingsvedtak_liste/stortingsvedtak[1]`; feltene `id`, `sak_id`, `stortingsvedtak_nummer`, `stortingsvedtak_dato_tid`, `stortingsvedtak_type` og `stortingsvedtak_tekst` binder identitet, dato, type og tekst. Både **210** og **211** er **ANNET** i kilde-API-et. Bevilgningsinnholdet i 210 viser hvorfor BUDSJETT alene er et utilstrekkelig kildefilter. Begge gjelder sak 100927 og 16.12.2024.

210s dekodede HTML romertall I har én tabell, kapittel 1429, /1 og /22 og akkurat de seks eksakte beløpene ovenfor. I B3s lagrede lokatorregime er /1-delta `table[1]/tr[3]/td[4]`, før/etter `table[1]/tr[4]/td[3]`; /22-delta `table[1]/tr[5]/td[4]`, før/etter `table[1]/tr[6]/td[3]`. De forskjellige beløpsfeltene i samme fra-/til-celle er egne `amount_field`-verdier. Disse er ikke HTML-`tbody`-radnumrene fra innstillingen. 211s dekodede romertall II har bare undertittel og samtykkeavsnittet; ingen beløp, tredje postendring eller saldo oppstår. Kilder: [210-original](../../../tests/fixtures/b6/40034048.xml), [211-original](../../../tests/fixtures/b8/40034049.xml) og [plenumsoriginal](../omtale-o1/originals/votering-161224.html), `#2024-12-16-25`.

### Originalt forslag → tilråding → vedtak, uten konstruert komitéendring

| Konto/budsjettår | Prop. 16 S regjeringen, før / endring / etter | Innst. 81 S samlet komités tilråding | 210 endelig vedtak | Tillatt avledet sammenligning |
| --- | --- | --- | --- | --- |
| 1429/1,2024 | 160 243 000 / +5 796 000 / 166 039 000 | De samme tre verdiene | De samme tre verdiene | Forskjell forslag–tilråding = 0 og tilråding–vedtak = 0 for hvert av de tre sammenlignbare feltene; fortsatt egne kildeobservasjoner. |
| 1429/22,2024 | 32 185 000 / −3 000 000 / 29 185 000 | De samme tre verdiene | De samme tre verdiene | Samme nullforskjeller. Ingen kildebelagt komitéendring eller alternativt beløp. |
| 1429/60,2024 | Forslag V nr. 3 om stikkord | Tilråding II om stikkord | 211 samtykker til stikkordet | Tekst-/fullmaktssammenligning; ingen numerisk null eller oppdiktet beløpsrad. |

Prop.-lokatorene er `prop16s-ch4.html`, første `table/tbody/tr[43]` (kapittel), `[44–45]` (/01) og `[46–47]` (/22), PDF s. 8. Forslagets stikkordsfullmakt er V nr. 3, PDF s. 10, HTML `/html/body/main/div/div[3]/div[3]/div/div/div[5]`, med `p#kap2-p60` som innledningsavsnitt. Omtale er `#kap2-p24`, `#kap2-p25`, `#kap2-p26` i kapittel 2-HTML. Fullstendige XPaths for de avgrensede O1-passasjene finnes i [passages.json](../omtale-o1/passages.json).

Det er kildebelegg for nysalderingskontekst, men **de ekte eksisterende 210-observasjonene har `round='uavklart'`**. Datakontraktens rundevalg krever uttrykkelig tittel eller kildebegrunnet `Interpretation(round=..., round_evidence=...)`. Et nytt sammenligningslag må bruke et eksplisitt versjonert kildegrunnlag for slik klassifikasjon og bevare de gamle observasjonene/ID-ene. Kalenderdato alene er ikke rundegrunnlag. O1s kjede gir ikke opprinnelig budsjett, RNB-vedtak eller helårsbalanse.

## Hele Prop. 16 S: synlig inventar utover 1429

Bevart full PDF har 12 sider: innledning/endringsomtale s. 1–6, forslagets bevilgninger s. 7–9, fullmakter s. 10–11 og bakside s. 12. Kapittel 2- og forslag-HTML er delrepresentasjoner av den samme navngitte proposisjonen; full HTML for innledning/tilråding er ikke bevart som egne O1-responser. PDF-en bevarer disse delene. O2b kontrollerer HTML/PDF-samsvar for P1, ikke for hele dokumentet. Kilde: [full original](../omtale-o1/originals/prop16s.pdf) og [manifest](../omtale-o1/source-manifest.json).

### Eksakte forslagstabeller I

Alle beløp nedenfor er **regjeringsforslag**, kroner, budsjettår 2024, med feltene før/endring/etter. Fortegnet følger originalens «økes/reduseres». Dette er en manuelt kildekontrollert undersøkelsestabell, ingen utført import eller nye vedtatte hendelser. HTML-lokator: forslag-HTMLs første tabell = **U**, andre = **I**; radnummer er 1-basert i respektiv `tbody`, og den etterfølgende raden har fra-/til-beløpet. Absolutte tabellstier er `/html/body/main/div/div[3]/div[3]/div/div/div[1]/div[1]/table` og tilsvarende `div[2]/table`. Rå postkoder 01/02/03/04/06/07/09 bevares separat fra kanonisk kode.

| Konto | Før kr | Endring kr | Etter kr | HTML-rader; PDF-side |
| --- | ---: | ---: | ---: | --- |
| 1400/01 | 322 816 000 | +5 937 000 | 328 753 000 | U2–3; s. 7 |
| 1400/21 | 102 806 000 | −8 800 000 | 94 006 000 | U4–5; s. 7 |
| 1400/71 | 94 355 000 | +18 056 000 | 112 411 000 | U6–7; s. 7 |
| 1400/76 | 107 394 000 | −2 000 000 | 105 394 000 | U8–9; s. 7 |
| 1410/21 | 440 016 000 | −380 000 | 439 636 000 | U11–12; s. 7 |
| 1410/70 | 56 263 000 | +380 000 | 56 643 000 | U13–14; s. 7 |
| 1411/01 | 40 350 000 | +830 000 | 41 180 000 | U16–17; s. 7 |
| 1412/70 | 144 164 000 | −5 023 000 | 139 141 000 | U19–20; s. 7 |
| 1420/01 | 883 920 000 | +21 497 000 | 905 417 000 | U22–23; s. 7 |
| 1420/21 | 637 574 000 | −2 500 000 | 635 074 000 | U24–25; s. 7 |
| 1420/23 | 165 801 000 | +59 965 000 | 225 766 000 | U26–27; s. 8 |
| 1420/61 | 333 800 000 | −183 800 000 | 150 000 000 | U28–29; s. 8 |
| 1420/62 | 80 625 000 | −50 000 000 | 30 625 000 | U30–31; s. 8 |
| 1420/69 | 111 732 000 | −14 400 000 | 97 332 000 | U32–33; s. 8 |
| 1420/74 | 6 464 997 000 | −246 200 000 | 6 218 797 000 | U34–35; s. 8 |
| 1420/75 | 416 350 000 | −15 000 000 | 401 350 000 | U36–37; s. 8 |
| 1420/80 | 180 942 000 | +2 500 000 | 183 442 000 | U38–39; s. 8 |
| 1423/01 | 39 667 000 | +549 000 | 40 216 000 | U41–42; s. 8 |
| 1429/01 | 160 243 000 | +5 796 000 | 166 039 000 | U44–45; s. 8 |
| 1429/22 | 32 185 000 | −3 000 000 | 29 185 000 | U46–47; s. 8 |
| 1471/01 | 263 050 000 | +65 217 000 | 328 267 000 | U49–50; s. 8 |
| 1471/21 | 120 706 000 | +3 400 000 | 124 106 000 | U51–52; s. 8 |
| 1474/01 | 266 000 | +7 000 | 273 000 | U54–55; s. 8 |
| 1481/01 | 2 798 000 | −1 300 000 | 1 498 000 | U57–58; s. 8 |
| 1481/22 | 120 000 000 | −20 000 000 | 100 000 000 | U59–60; s. 9 |
| 1482/01 | 67 459 000 | +3 461 000 | 70 920 000 | U62–63; s. 9 |
| 1482/73 | 4 041 235 000 | −2 500 000 | 4 038 735 000 | U64–65; s. 9 |
| 4400/02 | 518 000 | −518 000 | 0 | I2–3; s. 9 |
| 4400/03 | 39 231 000 | −1 416 000 | 37 815 000 | I4–5; s. 9 |
| 4420/04 | 58 745 000 | +29 069 000 | 87 814 000 | I7–8; s. 9 |
| 4420/06 | 39 249 000 | +17 751 000 | 57 000 000 | I9–10; s. 9 |
| 4420/07 | 9 928 000 | −3 300 000 | 6 628 000 | I11–12; s. 9 |
| 4420/09 | 39 545 000 | +13 145 000 | 52 690 000 | I13–14; s. 9 |
| 4420/40 | 1 069 000 | −700 000 | 369 000 | I15–16; s. 9 |
| 4420/85 | 1 000 000 | +4 600 000 | 5 600 000 | I17–18; s. 9 |
| 4471/03 | 71 835 000 | +58 165 000 | 130 000 000 | I20–21; s. 9 |
| 4481/01 | 1 908 518 000 | +303 020 000 | 2 211 538 000 | I23–24; s. 9 |

Dette er **37 postgrupper, 111 eksakte beløpsfelt, 15 kapitler**: 27 utgiftsposter i 11 kapitler og 10 inntektsposter i 4 kapitler. 1429-utvalget dekker bare 2 av de 37 postgruppene. Et fremtidig «alle forslagstabellposter»-uttrekk skal avstemmes mot denne listen og originalen; adapterens egne funn er ikke en uavhengig nevner. Observerbar null på 4400/02 etter endringen er forskjellig fra manglende konto/ledd.

### Fullmakter, øvrige kontoreferanser og omtale

Forslag-HTMLs felles prefiks **F** er `/html/body/main/div/div[3]/div[3]/div/div`. Hele fullmaktsseksjonen må bevares, ikke bare pengebeløpet.

| Del | Konto og originalt omfang | Beløpstype/år | Lokator |
| --- | --- | --- | --- |
| II Bestillingsfullmakt | 1420/21, kjøp av pukkellaksefeller | Samlet ramme for nye bestillinger og gammelt ansvar **8 mill. kroner**; samtykke i 2024 til fremtidige år. Ikke 2024-bevilgningsdelta. | F`/div[2]`, `#kap2-p57`; PDF s. 10 |
| III Tilsagnsfullmakter | 1420/61 og /62 | Samlede rammer **601,0 mill.** og **266,3 mill. kroner**, nye tilsagn + gammelt ansvar; 2024. | F`/div[3]`, `#kap2-p58`, tredje tabell/tbody rader 2–3; PDF s. 10 |
| IV Fullmakt til å inngå forpliktelser | 1420/postene **39,69,79**, oppryddingstiltak | Samlet ramme **16,3 mill. kroner** for nye forpliktelser + gammelt ansvar; 2024, fremtidige år. Ingen fordeling av rammen på de tre postene. | F`/div[4]`, `#kap2-p59`; PDF s. 10 |
| V Stikkordsfullmakt nr. 1–3 | 1420/66,1420/87 og 1429/60 | Tilføye «kan overføres» **i 2024**, uten beløpsverdi. | F`/div[5]`, `#kap2-p60` og nummerert liste; PDF s. 10 |
| VI nr. 1 forskuttering | 1471/01 mot 4471/03, oppdragsprosjekter | Inntil **25 mill. kroner**,2024; bindende avtale/sikkerhet før full finansiering innbetales. | F`/div[6]`, `#kap2-p61` og liste; PDF s. 11 |
| VI nr. 2 regnskapsføring | Samme oppdragsprosjekter | Forskuddsutbetalinger på mellomværende; rapporteres når inntekter kommer inn. Ingen ny tallfestet bevilgning. | Samme seksjon, nr. 2; PDF s. 11 |
| Kapittel 2,1400/21 | Rammeoverføring til **1533/45** Eiendommer utenfor husleieordningen | Omtalt **10,8 mill. kroner** til rassikring Øvre Storwartz; mottaker har ingen egen forslagstabellrad i dette dokumentet. | Kapittel 2-HTML `#kap2_ch1_ch2`; PDF s. 1 |
| Stikkord i 1474/01 | «kan nyttes under postene **50 og 70**» | Kontoreferanser, ingen selvstendige endringsbeløp for 1474/50 eller/70. | Forslagstabell U54; omtale PDF s. 4 |

Postene 1420/66,/87 og 1429/60 mangler endringstabellrad, men inngår i både omtale og fullmakt. Videre er 1420/39,/79,1533/45,1474/50,/70 uttrykkelige kontekst-/fullmaktsreferanser uten egne endringstabellrader. Et kontoinventar som teller alle eksplisitte kontoreferanser, også disse rollene, har her **45 unike kontoer**:37 endringstabellposter +3 stikkordsposter +5 øvrige referansekontoer. Rollene skal vises; tallet 45 betyr ikke 45 bevilgningsendringer eller 45 sikkert relaterte vedtak.

Omtalen s. 1–6 har også avrundede begrunnelser, komponent-/omdisponeringsbeløp og henvisninger til tidligere runder og andre perioder. Eksempler med vesentlig klassifikasjonsfare er 1420/61 og /62s reduksjon mot økte tilsagnsfullmakter, 1420/74s 2024-utbetalinger for støtteåret 2023,1429/60s 2024/2025-fond og 1471s regnskapsavslutning 2023/fremtidig RNB2025. Disse må bevares som tekst-/beløpsutsagn med sine roller, ikke normaliseres til ett gjettet budsjettår eller ekstra deltaer. De er ikke generelt strukturert av O2b. De 37 presise tabellgruppene over er derfor ikke en påstand om full semantisk strukturering av alle beløpsutsagn i proposisjonen. Kilde: [PDF s. 1–6](../omtale-o1/originals/prop16s.pdf), [kapittel 2-HTML](../omtale-o1/originals/prop16s-ch2.html).

## Faktiske gamle filer: utført readonly kontroll

Ekte lokale filer er tilgjengelige i `outputs/o2b-210-begge-poster-7e70506/` og `outputs/o2a-210-post1-52f0545/` i hovedarbeidsområdet. Ingen filer er regenerert eller overskrevet. Undersøkelsen leste alle seks B-par (`begge`, `post1`, `post22`, `tomt`, `offline`, `syntetisk-forslag`) og de to A-parene (`omtale-210-post1`, `offline-gjenlest`). JSON ble validert med eksisterende `report_from_json` og underliggende B8-leser. XLSX ble åpnet readonly; de faktisk lagrede ordnede tekststykkene i `Omtalegrunnlag` ble sammenføyd og var **eksakt identiske med JSON-filen**. Antall faktiske rader i `Beløpsobservasjoner`, arkstruktur, Historikk-verdier og filhasher ble kontrollert. Det ble ikke kjørt `read_excel`, fordi den eksisterende leseren lager en midlertidig rekonstruksjon ved kildefilen; denne undersøkelsen krevde ren lesing. Ingen bred testsuite eller ny visuell render er utført her.

| Ekte uttak | Valgte beløpsrader i XLSX | Seksjoner / relasjoner i frosset grunnlag | Faktisk rapport-ID |
| --- | ---: | --- | --- |
| B begge og B offline | 6 | 11 /13 | `ef508e79e8f55993893250ff96f9f1ac6b55138dfb58b634fdc3cec51b3b42ab` |
| B post 1 | 3 | 11 /13 | `978b86d0701fc4c030e9f5fbf738e1187bcca3c76fff112f366cff8abb043174` |
| B post 22 | 3 | 11 /13 | `51d209382fcb5fa69fc7ac38687a3a965b7754c4d11d44a0b2197e6088c24a22` |
| B tomt, med merket syntetisk forslag | 0 | 11 /14 | `17ebed652bfc42eebf8f863706d6de6918fb0422b1cb3f84324a62187e273e87` |
| B syntetisk-forslag | 6 | 11 /14 | `d8f29ff8f136d5eeb01303ccc8cd5e34c126b809391980f34cbc9f29b5347485` |
| A opprinnelig og A offline | 3 | 8 /6 | `22e216820b2b2d17fd43016d8be437a8cbdfaf4cbd8920b871aec0acd55d7143` |

Alle parenes hasher var uendret etter lesingen og samsvarte med [O2b-verifikasjonen](../omtale-o2b/verification.json). B `begge.json` har SHA-256 `96dbe2c089272a661a6c37b4e1eaee5a10d78629720916c55705ba16aff7397d`, `begge.xlsx` `34dea0f68eb3a1ec6eb33d5bf56bc7d04c519cb7f0be8a14d22897576a5aec84`. A `omtale-210-post1.json` har `bd5666408115ce448a1c3ecf84242cade4c668ef507842e81eb5465c3bca7129`, XLSX `3fc3f731970dccb47ce773e37a48c42be2c9b10cf7525c82826c6436fc7965e3`. Andre par har egne bevarte hasher i samme manifest; offline-XLSX behøver ikke være byteidentisk med opprinnelig XLSX for å ha samme frosne grunnlag.

B `Historikk!A1:M3` har faktisk 13 kolonner og to postrader. `J2:L2` er 160243000/5796000/166039000; `J3:L3` er 32185000/−3000000/29185000. Post 22-navnet i hovedvisningen er kulturminneforvaltning, mens P22/K22 bevarer kulturmiljøforvaltning. Hovedvisningens kontrolltekst sier fortsatt at postvis forslagstilknytning ikke er bevist av **saksrelasjonen**; O2b-beviset finnes separat i omtalerelasjonene. Dette er ikke en ny numerisk forslagssammenligning.

### Identiteter som nye innganger skal bevare

Den ekte B-leveransen binder vedtak 210 til revisjon `a5eee5e8-e9cc-4d8b-96d9-aa1da83ef3e7`. UUID-en er denne leveransens bevarte revisjonsidentitet, ikke en utgiver-ID utledet fra XML. Andre genuint nye prøveimporter kan ha annen revisjons-UUID; en gjenlesing av denne eksporten skal ha den samme.

| Konto | Eksisterende hendelsesgruppe (`step_id`) | Endring / før / etter: eksisterende observasjons-ID-er |
| --- | --- | --- |
| 1429/1 | `9d75b6fc6a75b0862d1a55488a042ee63775366453309d00b0b06b382f8e8740` | `4ace7b42e5c7c522655ef3d8e18f832290b63d829bf8634810bad37f42b2be96` / `06c25431aec719ed34478b89ee4e6f17751cce932221cae90e436850d86952b9` / `f22283ad6cdeef6edfc78e01c498d1f56ce9b230a16376eee379a3a0e9d2780a` |
| 1429/22 | `d197ef77481e0d11a6154184469a69460f6be8260cf8fe95159e46b729ad0c16` | `d736250e6b842c25f8ad55e52dd5f82fd7be491d4e84bb7d63cddf413c10a2dd` / `e3fb685f7c234609c5451b89ef0901ca27b7b6228f9c6d9f9f7adf1c37a08da6` / `8f2ff2a8ca4818c8b0aae65019058dcdffa943764b480fa71f1401b095de81b7` |

O2b har én P1-seksjon `0de17d658739884ac8c865c8169460c191969f9ed2bf19a659aa6d62a352d5c9`, med relasjon til begge hendelser; lønnsforklaringen avgrenses til /1. Flere seksjoner, filtrering eller bytte av inngang skal ikke kopiere P1 eller skape et nytt `step_id`. Seksjonene og 13 dokumenterte relasjoner er alle `ikke_faglig_godkjent`; teknisk kildeverifikasjon er ikke faglig kontrollavgjørelse. De eksakte ID-ene kommer fra den faktisk leste eksporten, ikke fra eksempelgenerering.

## Minste komplette fremtidige akseptutvalg

Dette avsnittet er **forventet senere atferd**, ikke noe eksisterende O2b-filer allerede leverer. Ingen nye eksportfeltnavn eller lagringsschema besluttes her. Nye adapteres kildeidentiteter skal bindes til originale dokumentversjoner og lokatorer; dokument-/kontoutvalgene skal velge fra det samme grunnlaget.

Første positive snitt bør gi hele Innst. 81 S/210/211 med egne kildebeløp for Prop. 16 S 1429-delen, innstillingens tilråding og 210, og fullmaktskjeden Prop. V nr. 3→Innst. II→211. For de to tabellpostene er det seks eksakte felt **per stadium**, totalt **18 kildebeløpsobservasjoner** hvis hvert av de tre dokumentenes før/endring/etter-felt importeres én gang. Bare seks er vedtaksobservasjoner og de beskriver fortsatt **to vedtatte beløpshendelser**. Gjengivelse, omtale, avrundede komponentutsagn og plenumsbelegg føres som egne tekst-/utsagnsopplysninger med kildepeker; de kopierer ikke tilrådingstabellens eller 210s numeriske observasjoner. Antall utsagn må avstemmes separat fra 18-feltfasiten. Fullmakten er et separat dokumentert behandlingsledd og teller aldri som tredje beløpshendelse.

| Observerbar forventningsrad | Dokumentinngang | Konto-/årsinngang | Felles avstemming |
| --- | --- | --- | --- |
| Hele Innst. 81 S | Viser 1429/1,/22,/60, full sammendrags-/merknads-/tilrådingstekst, seks eksakte tabellfelt, alle kontekstbeløp og fullmakt II. | Velg disse tre kontoene og 2024; finn samme Innst.-versjon og de samme lokatorene, med kildeinventaret synlig. | De samme seks komitéfelt-ID-ene, tre kontoer i dokumentinventaret, to tabellgrupper og én stikkordsfullmakt. Ingen rolle-/beløpsarv til /60. |
| Hele 210 og 211 | 210 viser akkurat to poster/seks beløpsfelt; 211 viser 1429/60/fullmakt og ingen beløpsrad. | Velg /1 og /22: seks vedtaksfelt/to hendelser. Velg /60:211 og omtale; ingen gjettet bevilgningsverdi. | Samme 210-revisjon/observasjons-/step-ID-er og 211-kildereferanse ved begge innganger. |
| Prop.-del 1429 | Viser tydelig **delvis strukturert Prop. 16 S**: to eksakte tabellgrupper, 1429/60-fullmakt og fulltekstlenke. Restinventaret 37 grupper/45 referansekontoer/fullmakter er synlig med korrekt rollesplitt. | De valgte 1429-kontoene finner samme Prop.-versjon, de seks nye forslagsfelt-ID-ene og fullmakt V nr. 3; kontofilter fjerner ikke globalt restinventar. | Ingen påstand om at to strukturerte tabellgrupper er hele Prop. 16 S. Andre poster er ikke 0. |
| Sammenligning 1429/1 og /22 | Vis Prop.→Innst.→210 for 2024 med kilde, dato, rolle og hver før-/endrings-/etterverdi. | Samme tre stadier for de valgte kontoene; nullforskjell vises som avledet kontroll på hvert par av like felter. | 18 eksakte kildefelt/totalt, herav 6 vedtaksfelt/to vedtatte hendelser. Beregningene refererer inngangs-ID-er og øker ikke hendelsesantallet. |
| Filtrer /1,/22,begge,tomt | Samme dokumentbasis og globalt inventar beholdes. | Valgt numerisk fremtidig trestadieutvalg gir 9/9/18/0 felt, herav 3/3/6/0 vedtaksfelt og 1/1/2/0 valgte beløpshendelser. | Hele grunnlaget har 18 eksakte felt, 6 vedtaksfelt/to hendelser. Skillet mellom valgt og globalt gjelder også uavklart relasjon. |
| Naviger begge veier | Innst.→/22,2024→Innst. og 210→/1,2024→210. | /60,2024→211→/60,2024. | Samme ID-er, lokatorer, tekst, rolle, status og eksakt kildeversjon ved retur; ingen ny registrering på grunn av navigasjon. |
| Forgrening | Fra Prop. åpnes 100927/81 S **kap. 1429** og 100889/95 S **unntatt 1429**. | 1429 treffer 81 S-kjeden; en ikke 1429-konto viser 95 S-referansen med bevart fulltekst/postbevis fra [grenundersøkelsen](forgrening.md), men synlig ennå ikke implementert strukturering i første snitt. | Begge referansesett består. Like eksport-ID-er eller lik Prop. betyr ikke lik postrelasjon eller vedtatt resultat. |
| Årsforløp 2024, og valgfritt 2025 | Behandlingsleddenes kontekst står synlig. | 2024: opprinnelig budsjett/RNB/øvrige runder har hull uten egen kontrollert kilde. 2025: post 60s omtale er fremtidig kontekst, ikke bevis for 2025-vedtak eller kontokontinuitet. | Ingen godkjent årsbalanse eller automatisk join mellom like kontonumre over år. Ingen hull erstattes av null eller kopi av nysalderingens førbeløp. |

### Konkrete testmatriseinnslag før senere bygging

| Krav | Positiv autentisk prøve / negativ prøve | Forventet kontroll gjennom faktisk skrevet og gjenlest JSON og Excel |
| --- | --- | --- |
| V1 | Hele Innst. 81 S, 210, 211; Prop. som eksplisitt delvis strukturert forelder. | Sammenlign med **originalinventar**, ikke adapterens egen radliste: tre innstillingskontoer, seks eksakte felt, alt sammendrag inkl./60, samlet komité og II. Manglende/ustrukturerte deler vises. Prop. 37 grupper og fullmakter holdes synlige globalt. |
| V2/V5 | 1429-utvalg 2024; opprinnelig budsjett/RNB og eventuelle øvrige dokumenter ikke funnet i avgrenset inventar. | Hullliste med kontrollert kilde-/periodedekning, ikke komplett årslinje. Førbeløpene i nysalderingen blir ikke rekonstruert opprinnelig budsjett. Innst./vedtak som mangler i en merket feilprøve er ukjent, ikke 0 eller antatt identisk. |
| V3/V9 | Begge innganger, konto-/dokumentfilter, gjentatt eksport og mange-til-mange P1. | Samme versjoner/ID-er og feltverdier ved retur; valgte/globalt antall adskilt; 18 fremtidige eksakte kildefelt, 6 eksisterende vedtaksfelt/to hendelser i hele pilotgrunnlaget. Omtale-/relasjonsantall kan endres uten beløpsinflasjon. |
| V4 | De to autentiske saksoriginalene og nå bevart 95 S-gren. | 100889/95 S får ikke 1429-relasjon eller beløp via felles Prop.; 100927/81 S får ikke øvrige konti. Kildedekning og ennå ikke implementert 95 S-strukturering skilles. Begge referatlenkene består selv med lik eksport-ID. |
| V5 | Originalens kroner, avrundet omtale og fullmakter. | 160243000+5796000=166039000 og 32185000−3000000=29185000 er lokale kontroller. Avrundet 2,8/5,8 mill. erstatter ikke eksakte felt; beregnet 2796000 blir ikke lønnsobservasjon. 8 / 601 / 266,3 / 16,3 / 25 mill.-rammer blir ikke deltaer. |
| V6 | 210 har **ingen positiv prøve** på komitéendring/mindretallsalternativ. | Bevar kontrollert fravær i 81 S. Syntetisk alternativ kan teste rollevern, men skal merkes og kan ikke lukke V6. En annen autentisk kilde må gi eget alternativ-ID, avsender, komitéendring og separat vedtakelsesbevis før positiv V6-aksept. |
| V7 | Ekte 2024/2025-tekst for /60, men uten kontinuitetsbevis; tydelig merket syntetisk prøve med like kontonumre. | Separate konto-/årsforløp/ukjent kontinuitet. Oppgaveflytting, omnummerering, deling/sammenslåing trenger gyldighet, kilder og omfang; verken Vega-omtale eller lik konto gir bevis. |
| V8 | Original→begge utvalg→nye faktiske JSON-/Excel-par→faktisk gjenlesing. | Samme kilder, råbeløp/enhet, originaltekst/hierarki, lokatorer, roller, beløpsbetydning, beregningsinnganger, fullmakter og status. Lange tekster/formeltegn og kildepekere bevares. Nye 18-feltsuttak er ennå ikke produsert; dagens 8 ekte par er bare pilot-/kompatibilitetsbeviset ovenfor. |
| V9 | 211 uten beløp; flere tekster og replisert dokumentlenke. | To formelle vedtak 210+211 er forskjellig fra to **beløpshendelser** i 210. 211, forslagstabeller, referat og dokumentlenker gir 0 nye vedtatte beløpshendelser. |
| V10 | Manglende, korrupt, motstridende eller feilet omtale/historisk Excel; tomt kontofilter. | Autentisk ny offisiell vedtaksprøve skal fortsatt oppdages via ordinær innlesning, bevares, lagres og eksporteres. Globale feil består ved 0 rader. Ekte gamle A/B og B6/B8/B9 må gjenleses med uendrede ID-er/betydninger. Nye adaptere er frivillig tillegg; #10 er åpen. |

## Gjenstående adapterarbeid og hva dette notatet ikke beviser

Kildebelegg finnes allerede for to uendrede eksakte forslag–tilråding–vedtak-kjeder, hele Innst. 81 S-inventaret, fullmaktskjeden til 211 og den reelle forgreningen. Det mangler implementert import av egne regjerings-/komitébeløpsobservasjoner, komplett dokumentinventar med maskinlesbare dekningsstatuser, kildebelagte fulle fullmaktsledd, dokumentstyrt utvalg og samme sammenligningsutvalg fra konto/år. De generiske beløpsfeltene finnes i [AmountObservation](../../../innlesning/observations.py); det alene betyr ikke at en ny dokumentadapter eller en forslagsvisning finnes. O2bs [strukturering](../../../innlesning/omtale.py) og [rapportbygging](../../../analyse/omtale_begge.py) er konkret avgrenset til 210 og to poster.

Full Prop.-strukturering er et mulig senere komplett snitt med 37 eksakte tabellgrupper og II–VI, ikke inngangskrav for den foreslåtte Innst. 81 S-piloten. En senere helårsleveranse trenger uttrykkelig inventar for årets relevante proposisjoner, innstillinger og vedtak, også ANNET og vedtak uten proposisjon. Dagens bevarte dokumentkjede og faktisk leste filer gir ingen generell årsdekning, faglig startsaldo, kontokontinuitet eller driftsgodkjenning. Nye primærkilder og en positiv komitéendringsfasit undersøkes separat før de blir testfasit; syntetiske illustrasjoner må fortsatt merkes som syntetiske.
