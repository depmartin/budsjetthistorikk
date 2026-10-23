# Prop. 16 S: begge behandlingsgrener og hele endringstabellen

Kontrollert 23. oktober 2026 under #37. Avgrenset kildeundersøkelse, uten implementering, import til produktlager, Git- eller GitHub-endringer. Rapporten gjelder budsjettåret **2024**, dokumentene i sesjonen **2024–2025**, og den observerte, **beriktigede** Innst. 95 S. #10 står åpen. Gamle originaler, ID-er, tolkninger og eksportformater beholdes. Ny offisiell vedtaksinnlesning skal fortsatt fungere uavhengig av omtale og historisk saldo.

## Resultat og anbefalt leveransegrense

Hele Prop. 16 S har **37 uttrykkelige endringstabellposter i 15 kapitler**. Det er kontrollert i den uendrede O1-originalen, ikke overtatt som et forhåndstall. To poster tilhører Innst. 81 S/kap. 1429. Innst. 95 S har de øvrige **35**, med samme eksakte delta, før og etter, og **én ekstra post: 1420/32, +270 mill. kroner**. Dens tilråding og endelige vedtak har dermed **36 endringstabellposter i 14 kapitler**. Ingen av de 35 felles postene har en annen beløpstrippel. Alle 36 er avstemt mot faktisk API-original, offisiell vedtaksside og plenumsreferat. [Maskinelt belegg med hver rad, råfelt og lokator](originals/forgrening/inventory.json).

Dermed er helheten **37 foreslåtte og 38 vedtatte postendringer**, ikke 37 vedtatte endringer og ikke 111/114 hendelser når før-/delta-/etterfeltene telles. Fullmaktene kommer i tillegg som egne tekst-/fullmaktsledd. En full dokumentvisning må også inventere beløpsutsagn utenfor endringstabellen; tallet 37 beskriver bare denne tabellens postgrupper.

Kildegapet som gjaldt søstergrenen er nå fylt for dokumentkjeden, hele tilrådingens endringstabell og de fem fullmaktsvedtakene. **Anbefalt mål er ett uttrykkelig avgrenset helsnitt for denne proposisjonen og begge grener**, med samtlige originaler og synlige statuser også for ustrukturert tekst. Omfanget er likevel større enn én fersk byggkontekst dersom all postomtale, fullmaktsstrukturering, begge utvalg og faktisk JSON-/Excel-gjenlesing skal utvikles samtidig. Små komplette delutvalg er foreslått nedenfor; helvisning må vente på en egen, eksplisitt helinventarport.

## Faktisk bevaring, tider og versjoner

[Transportmanifestet](originals/forgrening/manifest.json) bevarer faktisk forespurt/endelig URL, start-/sluttid i UTC, HTTP-status, responsheadere, responsbyteantall og SHA-256. `Set-Cookie` er utelatt fra transportmetadata; responskroppene er uendret. Seks vellykkede nye responser ble hentet 23. oktober 2026 kl. **10.47.23–10.48.00 UTC**. Første forsøk ga fem DNS-feil uten responsbyte; de står i samme manifest **uten oppfunnet dokumenthash**. Henting brukte offentlig tilgang og `User-Agent: Mozilla/5.0`.

| Bevart respons | Byte | SHA-256 |
| --- | ---: | --- |
| [Innst. 95 S, full HTML](originals/forgrening/inns95s.html) | 283 123 | `ae61227fa83adf04fb45956b1bd714a75592bbc1d6c70da300e554afef806aa6` |
| [Innst. 95 S, full PDF](originals/forgrening/inns95s.pdf) | 382 025 | `7a78167c7eafc500938e4ac39d8ed9febec1f6e7e6ce337acc4b7a58d0d14635` |
| [Sak 100889, faktisk API-svar](originals/forgrening/sak-100889.xml) | 15 910 | `435985bb9cc454d32f4b5c2e0df1e07ef48146dfdb2bf4a456db4df091f00859` |
| [Sak 100889, nettside](originals/forgrening/sak-100889.html) | 74 624 | `279943f8df41d5ae940284c11fd6773b52921f45e093265c046c55b888a2026b` |
| [Plenumsreferat, voteringsdelen 18.12.2024](originals/forgrening/votering-181224.html) | 4 800 053 | `88553153fd4011b6b3aa041c7899701bd7f7a938f2ad1984aecd4c441d24a9d9` |
| [Endelige vedtak for sak 100889](originals/forgrening/vedtak-100889.html) | 215 031 | `f58ec94336da10d04046e09683bf83d6a72d3a2ddbf42a7b106f194472ef72f3` |

Offisielle innganger: [innstillingens HTML](https://www.stortinget.no/no/Saker-og-publikasjoner/Publikasjoner/Innstillinger/Stortinget/2024-2025/inns-202425-095s/?all=true), [PDF](https://www.stortinget.no/globalassets/pdf/innstillinger/stortinget/2024-2025/inns-202425-095s.pdf), [saks-API](https://data.stortinget.no/eksport/sak?sakid=100889), [saksside](https://www.stortinget.no/no/Saker-og-publikasjoner/Saker/Sak/?p=100889), [vedtaksside](https://www.stortinget.no/no/Saker-og-publikasjoner/Vedtak/Vedtak/Sak/?p=100889) og [voteringsreferat](https://www.stortinget.no/no/Saker-og-publikasjoner/Publikasjoner/Referater/Stortinget/2024-2025/refs-202425-12-18/voteringer#181224-13). Den siste lenken returnerte faktisk `https://www.stortinget.no/no/saker-og-publikasjoner/publikasjoner/referater/stortinget/2024-2025/refs-202425-12-18/?m=17`. Lenkeankeret fra eldre B8 er bevart som forespurt URL, men er ikke funnet som HTML-ID i den nye representasjonen. Derfor brukes faktisk XPath til sak 13 nedenfor.

**Beriktigelsen er en del av dokumentidentiteten.** Både HTML-tittelen og PDF-en sier «Beriktiget». Den eldre [bevarte HTML-responsen fra 22.10](originals/forgrening/inns95s-20261022-reused.html) har 283 141 byte/SHA-256 `1f159a3ca1df3e0bc35617644d0b36f7c92fd5684947f6eca5510595af533a03`. Den er gjenbrukt byteidentisk fra `work/p13-p2/work/residuals/i95.html`; opprinnelig metadata oppgir bare dato, URL, status, hash og byte, ikke presis hentetid eller headere. [Gjenbruksmanifestet](originals/forgrening/reused-inns95-manifest.json) angir dette. Alle fire hovedseksjoners normaliserte tekst er identisk mellom disse to HTML-responsene. Ulike hele HTML-hasher beviser her ingen faglig rettelse mellom 22. og 23. oktober.

Den uberiktigede utgaven og selve rettelsesmeldingen er **ikke bevart/funnet i dette snittet**. Det er derfor ukjent hva beriktigelsen endret. PDF-metadata har opprettelse `D:20241210161841Z` og modifikasjon `D:20241212110900+01'00'`; dette er filmetadata, ikke et selvstendig rettelsesbevis. Leveransen kan uttrykkelig målrette den bevarte beriktigede versjonen, men skal ikke hevde rekonstruert versjonshistorikk.

Innstillingens HTML oppgir fem sider. PDF-en har åtte fysiske sider: fem innholdssider, to tomme sider og en avsluttende trykkside. Innholdsside 1–5 er rendret og visuelt kontrollert i [de fem PNG-ene](originals/forgrening/pdf-page-1.png); de viser hele tabellforløpet og fullmaktene. `inns95s-pdf.txt` er avledet pypdf-tekst, ikke original og ikke fasit for spaltenes leserekkefølge.

O1s seks originaler er **gjenbrukt uendret**, med kontroll mot O1s opprinnelige manifest. Det inkluderer full Prop. 16 S-PDF, delrepresentasjonene HTML kapittel 2 og 4, full Innst. 81 S og voteringsreferatet 16.12.2024. Ingen ny proposisjonshelimport er gjort. Full PDF og delvis HTML skal fortsatt ha forskjellige representasjonsstatuser. [O1](../omtale-o1/README.md) og [hashkontrollen](originals/forgrening/verification.json).

## Dokument- og vedtaksinventar

| Ledd | Offisiell identitet / dato / rolle | Kildebelagt omfang |
| --- | --- | --- |
| Regjeringen | Prop. 16 S (2024–2025), 22.11.2024; nysalderingsforslag for 2024; O1-hashene | Hele endringstabellen: 37 poster/15 kapitler. Forslag I–VI. |
| Gren A | Sak 100927; familie- og kulturkomiteens Innst. 81 S (2024–2025), 09.12.2024 | Bare kap. 1429: to endringstabellposter og post 60-fullmakt. |
| Gren A, endelig | 210/40034048 og 211/40034049, 16.12.2024, sak 100927 | 210: 1429/1 og /22. 211: 1429/60 «kan overføres». O1/B8-bevis beholdes. |
| Gren B | Sak 100889; energi- og miljøkomiteens **beriktigede** Innst. 95 S (2024–2025), 10.12.2024 | Alle kapitler/poster i Prop. 16 S **unntatt 1429**; 35 opprinnelige endringstabellposter + 1420/32. |
| Gren B, endelig | 359–364 / 40034220–40034225, 18.12.2024, sak 100889 | 359: 36 endringstabellposter; 360–364: fem separate fullmaktsvedtak. Alle seks har API-type **ANNET**. |

Det nye saks-API-svaret bevarer `/detaljert_sak/henvisning`, `id=100889`, `sak_sesjon=2024-2025`, komiteen og fem publikasjonshenvisninger. Under `/detaljert_sak/publikasjon_referanse_liste/publikasjon_referanse[1]` er Prop. 16 S' `eksport_id` fremdeles nil, mens etikett og regjeringen-URL er til stede. Henvisning 3 identifiserer `inns-202425-095s`; henvisning 5 peker til voteringen 18.12.2024. Relasjonen til 100927 er `sammekilde`. Ingen av disse metadataene alene er postvis vedtaksbevis.

De seks komplette vedtaksobjektene er trukket **byteidentisk** fra det allerede bevarte sesjonssvaret med SHA-256 `c5f3b90046d23a0e4cacb24f681a01d7e5fd4468ab68fc3d646dc832bb9a4b42`, 7 479 943 byte, URL `https://data.stortinget.no/eksport/stortingsvedtak?sesjonid=2024-2025`, hentet 22.10.2026 kl. 07.04.03.260568 UTC. Det er et annet faktisk HTTP-svar enn den eldre O1/B6-forelderen `9cfeaef…`; transportidentitetene er ikke erstattet eller slått sammen. Hele forelderen er allerede bevart tapsfritt i [årsagentens gzip-arkiv](originals/aar/session-2024-2025.xml.gz), med [transportmetadata](originals/aar/session-2024-2025.meta.json).

| Formelt nummer / API-ID | Romertall i Innst. 95 S | Utdragets byte / SHA-256 |
| --- | --- | --- |
| 359 / [40034220](originals/forgrening/40034220.xml) | I | 64 868 / `d4c473bf1ee95ec3edacce490586c0df5ec233d356e4c236fd9d765704b00490` |
| 360 / [40034221](originals/forgrening/40034221.xml) | II | 1 867 / `5523b3b70066f58a19c2a57dad37c4b83d601b28cbfbbcc8afb07c99f275cfd1` |
| 361 / [40034222](originals/forgrening/40034222.xml) | III | 4 954 / `cdc501f41586cfda1116f280f940c508314556c1e18552a68de842aae53ad162` |
| 362 / [40034223](originals/forgrening/40034223.xml) | IV | 1 889 / `9225b91c98f49b7b4f3006285848b0ca6021c335a220393be8dbc514787a53eb` |
| 363 / [40034224](originals/forgrening/40034224.xml) | V | 2 270 / `216186f2993d0844c81ac3a46f995df2a262a0afb930e2f44da27134aebc0fd6` |
| 364 / [40034225](originals/forgrening/40034225.xml) | VI | 2 715 / `e41f0de65ee6aeb438005af7b4f1230ad1268e7c5545bc8b027cae20b0e14dcd` |

Hvert utdrag har egen JSON-sidevogn med eksakt foreldremetadata, objektordinal, byteposisjon, objektlengde og egen hash. Utdragsoppskriften er `parent[0:317] + parent[start:end] + parent[7479886:7479943]`, med **null innsatte byte eller linjeskift**. For 359 er `start=2172545`, `end=2237039`; øvrige grenser står i sidevognene. XML-lokator med navnerom `http://data.stortinget.no` er `/stortingsvedtak_oversikt/stortingsvedtak_liste/stortingsvedtak[1]`; `id`, `sak_id`, nummer, dato og dekodet tekst bindes samlet. Utdragene er delvise sesjonsprøver, aldri nye fullstendige HTTP-svar.

## Kontoinventar og faktiske lokale avvik

Tabellen nedenfor teller **postgrupper i endringstabellen**. Detaljer med rå kontokode, formål, delta, før-/etterbeløp og egne XPaths for Prop., Innst., API, vedtaksside og plenumsreferat finnes i [inventory.json](originals/forgrening/inventory.json). Det er et forskningsuttrekk, ikke en implementert produktadapter.

| Kapittel | Prop. 16 S, endringstabellposter | Innst. 95 S / vedtak 359 |
| --- | --- | --- |
| 1400 | 1, 21, 71, 76 | Samme fire |
| 1410 | 21, 70 | Samme to |
| 1411 | 1 | Samme |
| 1412 | 70 | Samme |
| 1420 | 1, 21, 23, 61, 62, 69, 74, 75, 80 | Samme ni **+ 32** |
| 1423 | 1 | Samme |
| 1429 | 1, 22 | **Ingen**; Innst. 81 S / 210 |
| 1471 | 1, 21 | Samme to |
| 1474 | 1 | Samme |
| 1481 | 1, 22 | Samme to |
| 1482 | 1, 73 | Samme to |
| 4400 | 2, 3 | Samme to |
| 4420 | 4, 6, 7, 9, 40, 85 | Samme seks |
| 4471 | 3 | Samme |
| 4481 | 1 | Samme |
| **Totalt** | **37 poster / 15 kapitler** | **36 poster / 14 kapitler** |

1420/32 har **812 765 000 → +270 000 000 → 1 082 765 000 kroner** i Innst. 95 S og 359. I Innst.-HTML er den `#m4`, romertall I, første tabell, `tbody/tr[29]` med før-/etterrad `[30]`; PDF side 3. Det finnes ingen tilsvarende rad i Prop. 16 S' endringstabell. Manglende regjeringsforslag for denne raden er derfor **kildeforankret fravær i det undersøkte dokumentet**, ikke et forslag med null i delta eller null i nivå.

Innstillingens sammendrag nevner 1420/66 og /87 som endringer selv om de ikke har bevilgningsendringsrad; de gjelder stikkordsfullmakt V. En parser som bare bruker første tabell, mister dette innholdet. På samme måte skal 1420/39 og /79 i fullmakt IV og 1429/60 i søstergrenen bevares uten å lage ekstra bevilgningshendelser.

## Fullmakter og fordeling mellom grenene

[Romertallsbevisene](originals/forgrening/romertallsbevis.json) bevarer hele tilrådings-/plenumsseksjonen og hver dekodet API-seksjon med kildens hash, XPath og full råtekst/HTML. Prop.-lokatorene finnes i O1s kapittel 4-HTML og full PDF side 10–11; Innst. 95 S-fullmaktene står på trykt side 4–5. Følgende er inventar, ikke en påstand om at fullmaktsbeløp kan summeres som bevilgning:

| Prop. 16 S | Konto / innhold / år | Behandlingsgren og endelig identitet |
| --- | --- | --- |
| II | 1420/21: pukkellaksefeller; bestillingsramme 8 mill. kroner; fullmakt i 2024 for fremtidige år | Innst. 95 S II → 360/40034221 |
| III | 1420/61: samlet tilsagnsramme 601,0 mill.; 1420/62: 266,3 mill.; nye tilsagn og gammelt ansvar, 2024 | Innst. 95 S III → 361/40034222; to rammer, ett formelt vedtak |
| IV | 1420/39, /69 og /79: samlet forpliktelsesramme 16,3 mill.; materiell/tilskudd, 2024 og fremtidige år | Innst. 95 S IV → 362/40034223; rammen skal ikke fordeles tre ganger |
| V punkt 1–2 | 1420/66 og /87: tilføye «kan overføres», 2024 | Innst. 95 S V → 363/40034224; to tekstpunkter, ingen bevilgningsdeltaer |
| V punkt 3 | 1429/60: tilføye «kan overføres», 2024 | Innst. 81 S **II** → 211/40034049 |
| VI punkt 1–2 | Norsk Polarinstitutt: forskuttering i oppdragsprosjekter, ramme 25 mill.; 1471/1 mot 4471/3; separat regnskapsfullmakt om mellomværende; 2024 | Innst. 95 S VI → 364/40034225; inntekts-/utgiftskonto og regnskapsvilkår beholdes sammen |

Dette er fem fullmaktsromertall i Prop. 16 S, fordelt på **seks formelle fullmaktsvedtak** i to grener. Teller man atomiske innholdspunkter/rammer, er det ni (1+2+1+3+2), men det er en uttrykkelig inventarkonvensjon, ingen kildeobservert hendelsestotal. Romertall er lokalt i dokumentet: Prop. V punkt 3 blir Innst. 81 S II. Romertall alene kan derfor ikke være en global koblingsnøkkel.

## Omtale, avsender og vedtakelsesbevis

Innst. 95 S `#m1` og `#m2` sier uttrykkelig at alle kapitler/poster unntatt 1429 behandles, men at bare kontoer med merknader omtales videre. Fravær av eget postavsnitt for noen av de 35 postene betyr dermed ikke manglende behandling. Visningen må kunne vise en felles komitémerknad og presis henvisning til proposisjonen uten å produsere oppdiktet, individuell komitéomtale.

`#m3` har navngitt samlet komité og egne avsnitt om lønnsoppgjør, 1420/62, /74, /75 og 4481/1, samt uttrykkelig støtte til de foreslåtte endringene. Avsnittet om skogvern har **Ap, Sp og SV** som avsender og foreslår 1420/32 +270 mill. kroner. Høyres kritikk av nye satsinger i nysalderingen og FrPs merknader om CO₂-kompensasjon/industrien har sine egne avsendere. Det er ingen separat alternativ endringstabell i den komplette bevarte innstillingen. Komitégruppenes tekster skal ikke tilskrives samlet komité eller gjøres til vedtatt begrunnelse.

`#m4` sier at **tilrådingen fremmes av en samlet komité**, og har 1420/32 i tilrådingstabellen. Hele plenumsblokken for sak 13 gjengir Innst. 95 S / Prop. 16 S, unntatt kap. 1429, alle seks romertall og resultatet **enstemmig vedtatt**. I den faktisk hentede representasjonen er blokken:

`/html/body/div[2]/div/main/div[2]/div/div[4]/div/div/div/div/div/div/div[1]/div[14]`

Full blokk, rå HTML og kildehash står i [passages.json](originals/forgrening/passages.json). De 36 beløpstriplene er kontrollert også mot denne blokken og det uavhengig bevarte API-grunnlaget. Forbindelsen til 359 bygger på sak-/dokumentidentitet, konkret tilråding, gjengitt ordlyd, vedtakelsesbevis og formelt vedtak samlet; den er ikke utledet av likt beløp alene. Den enstemmige vedtakelsen gjør fortsatt ikke Ap/Sp/SVs begrunnelsesavsnitt til Stortingets egen ordlyd.

## Kontroller, synlige gap og foreslått testmatrise

[Utført offline kontroll](originals/forgrening/verification.json) dokumenterer seks nye responsers faktiske hash-/bytekontroll, seks uendrede O1-originaler og fire O1-støttefiler, seks komplette vedtaksobjekter fra den bevarte gzip-forelderen, unike postnøkler, alle før+delta=etter-kontroller, og eksakt avstemming av de 36 postene mellom Innst./API/vedtaksside/plenum. Råoriginaler, tabelluttrekk og byteoppskrifter er bevart for etterprøving; den midlertidige forskningshjelperen ligger lokalt i `work/kontroller-forgrening-37.py` og er ikke produktkode eller del av leveransen. PDF-side 1–5 er visuelt kontrollert. Bibliotekversjoner står i inventory.json. Ingen produkttest, JSON-/Excel-visning eller ny faglig godkjenning er hevdet utført.

| Aksept | Autentisk prøve og konkret kontroll | Status før bygging |
| --- | --- | --- |
| V1, helinventar | Prop. 37 endringstabellposter, alle 15 kapitler, romertall I–VI, full PDF og delvis HTML; 95 har 36/14 og fullmakter II–VI; 81 har 2/1 og post 60 | Råkilder og tabellinventar bevart. Generell strukturering av all tekst/alle beløpsutsagn og omtalerelasjoner gjenstår. |
| V4, forgrening | 1429/1, /22 og /60 skal bare gå via 100927/81/210–211; øvrig Prop.-innhold via 100889/95/359–364 | Dokument- og kontoomfang kildebelagt. Syntetisk feilruting skal avvises; globalt inventar skal bestå under filter. |
| V3, begge veier | Dokument→1420/32/2024→samme 95-versjon; konto→Prop.16/95/359→konto; tilsvarende 1429/22 og post60 | Produktnavigasjon og identitetsbevaring er uprøvd. Manglende Prop.-rad32 skal synes. |
| V5, talltyper | 35 identiske forslag/tilrådinger gir beregnet forskjell 0 med eksplisitt grunnlag; 1420/32 har manglende Prop.-stadium; fullmaktsrammer holdes separat | Tabellgrunnlag kildebelagt; beregnet forskjell er ingen ny vedtatt hendelse. |
| Roller | Ap/Sp/SV-omtale32; samlet tilråding; H/FrP-merknader; enstemmig vedtakelse; 95 har ikke egen postomtale overalt | Kildetekster bevart. Krever egne kildebindinger ved senere omtalestrukturering. |
| V8–V10, faktisk leveranse | Samme 38 unike vedtatte postendringer i hele valgt snitt, seks fullmaktsvedtak separat, fullstendige kilder/statuser i faktisk skrevet og gjenlest JSON/Excel | Ikke utført. Gamle B1/B2/O2a/O2b-filer og ID-er må regresjonskontrolleres uendret. |
| Versjoner/feil | Marker «Beriktiget», to HTML-responshasher med like seksjonstekster, gammel B8-respons og nytt svar; DNS uten hash; feil/manglende kilde viser gap | Belegg bevart. Rettelseshistorikk er uavklart; intet oppfunnet versjonslikhet eller nullpåfylling. |

**Reelle gjenværende gap:** Hele dokumentets øvrige nivåer, avrundede tallutsagn, omtalehierarki og post-/fullmaktsrelasjoner er ennå ikke generelt strukturert gjennom produktet. De 35 eksakte tabelltreffene beviser ikke at alle begrunnelser er strukturert, og ikke at hvert nevnt historisk nivå har en komplett kjede. Den uberiktigede Innst. 95 S og rettelsesmeldingen mangler. Det finnes ingen utført JSON-/Excel-gjenlesing for dette nye helsnittet. Årsdekning, flerårig kontokontinuitet og generell komitésøkefunksjon ligger utenfor denne undersøkelsen.

Det gjenstår derimot ikke et skjult vedtaksbevisgap for tabellens 36 poster: hver av dem har konkrete API-, nett- og plenumsbevis. Faglig godkjenning av historisk saldo og alle sammenhenger er fortsatt en annen status.

## Forslag til små komplette delutvalg og helinventarport

Et samlet byggeticket kan spesifiseres for **kun den hashfestede Prop. 16 S-versjonen, de to navngitte innstillingene og åtte formelle vedtak**, med all råtekst tilgjengelig og synlig delvis strukturering. Det må da eksplisitt skille «hele dokumentinventaret» fra «all omtale strukturert». Et slikt ticket skal ikke samtidig love generell årsvisning eller generelle adaptere for alle proposisjoner.

Hvis det er for stort for én kontekst, anbefales disse komplette snittene i rekkefølge:

1. **Autentisk forgrening med synlig helinventar:** Begge saks-/dokumentgrener, alle råoriginaler, 37/38-postinventaret og fullmaktsinventaret vises. Strukturér et avgrenset utvalg 1429/1+/22+/60 og 1420/32, med begge innganger og faktisk JSON-/Excel-gjenlesing. Øvrige poster/tekst merkes synlig «bevart, ikke strukturert». Dokumentet må fortsatt hete delvis strukturert dokumentvisning.
2. **Hele endringstabellen i begge grener:** Utvid samme leveranse til alle 37 forslag og 38 vedtatte postendringer, med 35 felles tilrådingsposter pluss32, kildebundet før/delta/etter, egne merknadsroller og fraværende Prop.-rad32. Bevar de seks fullmaktsvedtakene som tekst/inventar selv før all fullmaktstolkning er støttet.
3. **Fullmakter og eksplisitt helinventarport:** Strukturér II–VI og V→81II-forbindelsen uten bevilgningsdelta, og avstem alle kapitler, tabeller og tekstseksjoner i full Prop.-PDF, 81 og beriktiget95 mot hva begge visninger og eksportene faktisk viser. Ikke lukk porten før ustrukturert/uavklart innhold er uttrykkelig inventert og synlig; «fullt strukturert» krever at dette innholdet faktisk er strukturert, ikke bare at tabellparseren har null feil.

Hvert delutvalg skal være en egen komplett brukerleveranse med sluttkontroll av faktisk gjenleste filer, ikke et rent database-/parserlag. Nøyaktig ticketoppdeling og byggemandat må fastsettes i #37. Kildeundersøkelsen autoriserer ingen implementering, publisering eller sammenslåing.
