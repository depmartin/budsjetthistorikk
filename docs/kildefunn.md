# Varige kildefunn for innlesningen

Dette er faglige og tekniske funn som skal brukes på tvers av agentøkter. Dokumentet ligger på main og gjelder også før hele forskningsarbeidet i #2 er ferdig. Funn, kildebevis og konsekvens holdes samlet.

## To visninger: kildekontrollert grunnlag under #37

**Kontrollert 23. oktober 2026 mot main `5423160`:** [#37-undersøkelsen](research/to-visninger-37/README.md) har bevart originaler, hasher, presise tekst-/tabellokatorer, aktør- og vedtakelsesbevis. [Planen](visningspilot-plan.md), [testmatrisen](research/to-visninger-37/testmatrise.md) og [ticketutkastene](research/to-visninger-37/tickets/README.md) er forslag før implementering. O2b er levert i PR #39; det er ingen generell dokument-/årsvisning.

- Hele Innst. 81 S gjelder 1429/1, /22 og tekst-/fullmaktspost /60. Prop./innstilling/210 har to identiske beløpstrioer; 211 gjelder fullmakt uten bevilgningsbeløp. Bevar gamle observasjoners `round='uavklart'`; ny nysalderingskontekst må bindes separat. Foreslått T1 bruker 18 kildefelt med tre roller, men fortsatt bare seks vedtaksfelt/to monetære posthendelser.
- Prop. 16 S har 37 endringstabellgrupper og 45 ulike kontoangivelser inklusive kontekst/fullmakt. Beriktiget Innst. 95 S har de øvrige 35 gruppene og ny 1420/32 (+270 mill.), alle eksakt belagt i 359. Manglende Prop.-rad 32 er ikke regjeringsforslag null. Hele forgreningen gir 38 monetære postendringer og seks separate fullmaktsvedtak. Ap/Sp/SVs begrunnelse, samlet tilråding og enstemmig vedtak skilles. Urettet innstilling/rettelseshistorikk er uavklart; endret HTTP-hash beviser ikke semantisk rettelse. [Grenbevis](research/to-visninger-37/forgrening.md).
- Autentisk komitéendring er funnet på **315/78**: +119 mill. i Prop. 25 S, +129 mill. fra Ap/Sp/SV i Innst. 85 S og vedtatt i 208 med 63–35. Motstemmer beviser ikke et tallfestet mindretallsalternativ. [Aktør-/voteringsbevis](research/to-visninger-37/komiteendring.md).
- Valgte vedtak 341→857→210 gir fem 2024-posthendelser/elleve vedtaksfelt på 1429/1 og /22, ikke komplett årsdekning. Separat 201 gjelder 2025 til tross for samme dato som 210. Like kontokoder beviser ikke kontinuitet. Hele tidligere sesjonsresponser er nå bevart tapsfritt i repoet; avledede objekter har eksakte byteoppskrifter. [Årsbevis og dekningshull](research/to-visninger-37/konto-aar.md).

Praktisk konsekvens: samme versjonerte kildegrunnlag må drive begge innganger og faktisk gjenleste JSON-/Excel-filer. Rådekning, strukturering og faglig avklaring er separate statuser. Positivt tallfestet alternativ, kontinuitet over år og full årsdekning har egne åpne kildeporter. Ingen gamle ID-er, tolkninger eller formater omskrives; nye vedtak skal fortsatt registreres uavhengig. #10 forblir åpen.

## Omtale for vedtak 210: O1-kildebevis

**Kontrollert 22. oktober 2026 under #32:** [O1-rapporten](research/omtale-o1/README.md) bevarer seks offisielle originalrepresentasjoner med HTTP-metadata, SHA-256 og presise HTML-/PDF-lokatorer. Prop. 16 S forklarer 3 mill. kroner fra 1429/22 til egne stillinger på 1429/1, samt et avrundet lønnsanslag på 2,8 mill. Innst. 81 S støtter forslaget fra samlet komité; plenumsreferatet dokumenterer enstemmig vedtakelse. Eksakte vedtaksendringer er +5 796 000 og −3 000 000. Koblingen dokumenteres med postomtale, konkrete forslag/tilråding, votering og 210/40034048, utover felles saksmetadata.

**Konsekvens:** Prøven kan brukes til et komplett omtalesnitt, men gir ingen autentisk komitéendring eller mindretallsrolle. Beregnet rest 2 796 000 er ikke et observert eksakt lønnsbeløp. Post 22s to rånavn og post 60s fullmaktskontekst beholdes; omtale gir ingen nye beløpshendelser eller årsdekning. [To foreslåtte O2-tickets](research/omtale-o1/o2-forslag.md) skal godkjennes før publisering/bygging. Nye vedtak registreres uavhengig av omtale og historisk Excel; #10s driftsaksept står åpen.

## Historiske 2024-kolonner: P2-kontroll og bruksgrenser

**Kontrollert 22. oktober 2026:** [P2-matrisen](research/historisk-excel/p13-p2/README.md) binder alle ni beløpskolonner til avgrenset kontrollbruk og konkrete kildebevis. Hs faktor 1 000 000 er validert for 1 573 felles kontrollaggregater; 726 leksikalske presisjonsspor beholdes. Et separat binær-/ULP-begrenset heltallsforslag gir eksakt samsvar i dette omfanget, uten aktivering. 120 H-nullrester er klassifisert som 64 offisielle flyttinger, ett uttrykkelig nullomfang og 55 uavklarte fraværsårsaker. Fravær blir ingen nullbevilgning eller ikke-eksistens.

Faktisk lønnskilde er [Prop. 36 S kapittel 5](https://www.regjeringen.no/no/dokumenter/prop.-36-s-20242025/id3076783/?ch=5) med vedlegg 4, selv om hele M er 0. Lønn er inkludert i N på kontrollkonto 20/1. Offentlig lønnsfordeling summerer med reserve 2309/1 til 0; slik totalsum må ikke brukes som M-bevis. N-kontrollen dekker alle 737 ikke-null postkandidater mot et samtidig register, med tre direkte originalforslagsankre. Dette er ikke individuell avstemming av alle departementsproposisjoner.

Alle fire ikke-null L-felt har dokumentankre. p34 og p36 er datert samme dag, så en generell datoavgrensning «før nysaldering» er utilstrekkelig. Seks materialstratum-rester mellom K+L+N og dokument-D er [kildeforklart som forslag mot vedtak](research/historisk-excel/p13-p2/stage-residuals.json), med komitétillegg på samlet 600 mill. kroner og tilsvarende økning på 5800/50. De tre formelle kjedekonfliktene består. 228/85 og 2440/31 har konkrete fremtidige adapterforventninger, mens eksisterende v2 og 2 894-observasjonsankeret er uendret. Konsekvens: bruk kontrollmatrisens konkrete omfang; ingen generell normalisering, nullstart, komponentgodkjenning eller årsdekning følger av kildefunnene.

## Bevilgningsendringer finnes også som ANNET

**Observert 20. oktober 2026:** Stortingets API klassifiserer konkrete bevilgningsendringer som `ANNET`. Et uttrekk av bare `stortingsvedtak_type.id = BUDSJETT` mister derfor relevante vedtak.

| Prøve | Sesjon | Vedtaksnummer | Vedtaks-ID | Sak-ID | API-type |
| --- | --- | --- | --- | --- | --- |
| RNB 2024 | 2023–2024 | 857 | 40033719 | 98919 | ANNET |
| Nysaldering 2024 | 2024–2025 | 428 | 40034287 | 100289 | ANNET |

### Kildebevis

- [RNB-vedtak 857](https://www.stortinget.no/no/Saker-og-publikasjoner/Vedtak/Vedtak/Sak/?did=40033719&p=98919), med endringer blant annet på kapittel 21 post 1.
- [Nysalderingsvedtak 428](https://www.stortinget.no/no/Saker-og-publikasjoner/Vedtak/Vedtak/Sak/?did=40034287&p=100289), med konkrete fra-/til-beløp og bevilgningsendringer.
- API-typen er kontrollert i [sesjonsresponsen 2023–2024](https://data.stortinget.no/eksport/stortingsvedtak?sesjonid=2023-2024) og [sesjonsresponsen 2024–2025](https://data.stortinget.no/eksport/stortingsvedtak?sesjonid=2024-2025).
- [Versjonsfestet kontrollrapport med hentetider og SHA-256](https://github.com/depmartin/budsjetthistorikk/blob/5fdff33c73629c29215b4fc68a5bf8928639e7ed/docs/research/issue-2/kontrollkilder.md). Ved registreringen 20. oktober 2026 var den bredere undersøkelsen fortsatt under arbeid i [#2](https://github.com/depmartin/budsjetthistorikk/issues/2) og [utkast-PR #11](https://github.com/depmartin/budsjetthistorikk/pull/11).

### Konsekvens for innlesning og tester

1. Bevar vedtaksoversikten på tvers av API-typer. Bruk innhold og relevante saks-/dokumentkoblinger til å identifisere bevilgningskandidater.
2. Behandle ANNET-eksemplene som kildeprøver i dekningskontrollen. De skal kunne finnes selv om BUDSJETT-filteret ville utelatt dem.
3. API-type skal bevares som kildemetadata og skal ikke alene avgjøre om vedtaket er relevant.
4. At noen ANNET-vedtak inneholder bevilgninger betyr ikke at alle ANNET-vedtak gjør det. Ukjente eller tvetydige kandidater skal gi synlige kontrollavvik.
5. Fullstendighet krever mer enn kontroll av vedtakstype: kildeinventar og uavhengig avstemming skal brukes sammen.

Disse kontrollene er tatt inn i byggeticketene [#7](https://github.com/depmartin/budsjetthistorikk/issues/7) og [#9](https://github.com/depmartin/budsjetthistorikk/issues/9).

## Sakens dokumentgruppe er ikke et inngangskrav

**Kontrollert 20. oktober 2026:** Et initiativ fra Stortingets presidentskap om Akersgata-forprosjektet ble fulgt opp med en endelig økning på **9 700 000 kroner** på kapittel **41 post 45** for 2025, i vedtak **1149**, ID **40035422**, sak **103529**. Sakens direkte dokumentgruppe er melding, mens relevante fellesinnstillinger også viser proposisjoner.

Initiativvedtak **486**, ID **40034385**, ba om at bevilgning skulle fremmes senere. Det er ikke selv en kapittel-/postbevilgning. Endelig fullmaktsvedtak **1156**, ID **40035429**, har ramme **72 mill. kroner** for forpliktelser; dette er ikke en ekstra årsbevilgning.

Konsekvens: Finn kandidater fra alle vedtak og innholdet deres. Bevar sak, dokumentgruppe og initiativ som proveniens. Verken en direkte Prop.-lenke, dokumentgruppen proposisjon, et kronebeløp eller en tom relasjonsliste alene avgjør om en endelig bevilgning finnes. Skill anmodning, sats, fullmaktsramme og faktisk bevilgningslinje.

Kildebevis: [endelig bevilgning](https://www.stortinget.no/no/Saker-og-publikasjoner/Vedtak/Vedtak/Sak/?did=40035422&p=103529), [initiativvedtak](https://www.stortinget.no/no/Saker-og-publikasjoner/Vedtak/Vedtak/Sak/?did=40034385&p=101938), [separat fullmakt](https://www.stortinget.no/no/Saker-og-publikasjoner/Vedtak/Vedtak/Sak/?did=40035429&p=103529) og [versjonsfestet rapport og saksgraph](https://github.com/depmartin/budsjetthistorikk/blob/53a44e819dcbf1d73df57969cb7cb8864a7310b3/docs/research/issue-2/stortingsinitiativ.md).

Den første avgrensede undersøkelsen av nyere sesjoner fant ikke en sikkert selvstendig bevilgning. Et senere målrettet søk fant en autentisk positiv prøve: **vedtak 249, ID 40005719, 6. februar 2003**, bevilger **7 000 000 kroner på kapittel 41 post 21** til Mehamn-kommisjonen. Fulltekstene til representantforslaget, komitéinnstillingen, presidentskapets bevilgningsinnstilling og den parallelle lovinnstillingen viser ingen proposisjon som grunnlag for bevilgningen. Dette er en kontrollert relevant kildekjede, ikke en påstand om hele ulykkens forhistorie. [Endelig vedtak](https://www.stortinget.no/no/Saker-og-publikasjoner/Vedtak/Vedtak/Sak/?did=40005719&p=26250) og [versjonsfestet rapport og fasit](https://github.com/depmartin/budsjetthistorikk/blob/50871d870d1e8d80aba03069bb30ee9d533db77f/docs/research/issue-2/selvstendig-bevilgning.md).

I de historiske saksmetadataene avviker dessuten eksport-ID fra dokumentets forsamling og kanoniske URL (for eksempel inno-200203-114 mot inns-200203-114). Bevar avviket og kontroller publikasjonen mot tittel, URL og innhold; ikke rett råverdien stilltiende. Oppnevning, taushetsplikt og innsynsregler i samme sak er negative bevilgningsprøver. Eldre HTML i denne prøven er et historisk kildebevis og utvider ikke første leveranses startdato.

## Bevilgninger kan vedtas direkte uten komitéinnstilling

**Kontrollert 20. oktober 2026 etter eksempel fra prosjekteieren:** [Vedtak 599 (2025–2026)](https://www.stortinget.no/no/Saker-og-publikasjoner/Vedtak/Vedtak/Sak/?did=40036289&p=107811), ID **40036289**, 26. mars 2026, er type **ANNET**. Det reduserer inntektsbevilgningene på **5538/70–72** med henholdsvis **1 154 167 000**, **2 175 000 000** og **1 250 000 kroner**. Saken ble etter dokumentert prosedyrevedtak behandlet direkte uten komitéinnstilling; grunnlaget er et representantforslag og et erstattende forslag i salen. Ingen proposisjon inngår i den undersøkte behandlingskjeden. Manglende Prop.- eller Innst.-kobling skal derfor ikke føre til eksklusjon.

Samme sak inneholder både satser, faktiske kapittel-/postendringer og anmodninger. Bevar elementene hver for seg. Vedtak 598 har en separat endring på 5543/70 og skal ha sin egen identitet. Vedtak 591–597 og 600 skal ikke gi ekstra bevilgningslinjer.

Kilden har et faktisk tallavvik: vedtakssiden, sesjons-API-et og forslags-API-et viser til-beløpet for 5538/70 som `I 615 833`. Voteringsreferatets HTML og publikasjons-XML viser **1 615 833 000**, i samsvar med før minus reduksjon. Bevar råavviket og referatet som avklaringskilde. Ingen generell regel skal bytte I med 1, legge til nuller eller stille overskrive tall med beregnet verdi. Dette er motstrid mellom representasjoner, ikke en observert rettelse over tid.

[Versjonsfestet rapport, kildefasit, rå API-objekter og kontrollresultater](https://github.com/depmartin/budsjetthistorikk/blob/131ad9d6bcf62c2e1e6156784fd02d21e0a5876d/docs/research/issue-2/vedtak599/README.md). Prøven er eldre enn produksjonsstarten 2026–2027 og endrer ikke startavgrensningen.

## Statsregnskapets bevilgningskolonne har et hentbart originalgrunnlag

**Kontrollert 20. oktober 2026:** Den offentlig tilbudte [PDF-en for Statsrekneskapen 2024](https://www.regjeringen.no/contentassets/1d45fede74ff4ef18ce06bbd6163c723/nn-no/pdfs/stm202420250003000dddpdfs.pdf) ga HTTP 200, selv om en tidligere direkte HTML-forespørsel ga 403. Bruk en uttrykkelig publisert alternativ representasjon når den er tilgjengelig; dette betyr ikke at alle adresser eller årganger er hentbare.

PDF-ens tabell 2.1 og 2.2 har enhet 1 000 kroner. Alle 1 655 uttrukne postrader har Løyving som stemmer eksakt mot 594 kapittelsummer og begge totalsummer. Løyving er årets bevilgning; Samla løyving inkluderer overføring, og Rekneskap er utfall. Sumkontroll mot PDF-en validerer uttrekket, ikke hele vedtakskjeden.

[Versjonsfestet rapport, kildehash og kontrollgrunnlag](https://github.com/depmartin/budsjetthistorikk/blob/100a591ea10209f8cc85b2e190cbb5e1af482bb2/docs/research/issue-2/varig-kildegrunnlag.md). Bevar kildepresisjonen og skill mellom manglende kolonne og nullbeløp.

## Sesjon og kilderettelser krever full sammenligning

**Kontrollert 20. oktober 2026:** Virkelige vedtak om budsjettåret 2024 ligger i to sesjoner. Sakens opprinnelige sesjon kan dessuten være forskjellig fra vedtakets sesjon. En datomarkør alene er ikke tilstrekkelig for å oppdage etterslep eller rettelser.

Kilden viser siste versjon og dokumenterer ikke en rettelseslogg eller en bindende tidsgrense for gamle rettelser. Bevar gode råversjoner og sammenlign vedtaksobjekter per ID. Endret responstid alene er transportmetadata. Endret innhold med samme ID krever ny kildeversjon og ny vurdering av berørte kjeder; en manglende ID i ett svar er et avvik, ikke automatisk sletting.

To faktiske sesjonshentinger viste bare ulike responstidspunkter. Beløpsrettelse, sen innkomst og midlertidig fravær ble prøvd som tydelig merkede syntetiske kontrolltilfeller. De er ikke observasjoner av en reell historisk rettelse. [Versjonsfestede prøver og begrensninger](https://github.com/depmartin/budsjetthistorikk/blob/100a591ea10209f8cc85b2e190cbb5e1af482bb2/docs/research/issue-2/varig-kildegrunnlag.md).

## En katalog er ikke en uttømmende liste over senere poster

**Kontrollert 20. oktober 2026:** Vedtak 526, ID 40034443, 25. mars 2025, bevilger 454 000 000 kroner på ny post 32 under eksisterende kapittel 900. Kombinasjonen 0900/32 finnes ikke i den undersøkte opprinnelige kapittel 900-tabellen for 2025.

Bevar derfor beløpslinje og kilde selv om katalogoppslaget feiler. Opprett synlig kontrollbehov og et sporbarhetsgrunnlag for katalogutvidelse. Manglende førbeløp er ikke i seg selv bevis på nullstart. [Endelig vedtak](https://www.stortinget.no/no/Saker-og-publikasjoner/Vedtak/Vedtak/Sak/?did=40034443&p=102001) og [versjonsfestet kildeprøve](https://github.com/depmartin/budsjetthistorikk/blob/100a591ea10209f8cc85b2e190cbb5e1af482bb2/docs/research/issue-2/ny-katalogpost.json).

## Sluttsaldo og hele hendelseskjeden krever ulike kontroller

**Kontrollert 20. oktober 2026:** Hele 2024-materialet er avstemt. Alle 1 625 felles DFØ-/statsregnskapsposter stemmer eksakt for årets bevilgning. Alle 43 nøkkelforskjeller er forklart: 30 regnskapsrader med null bevilgning og 13 bevilgninger som er reversert til null. Alle 1 574 Blå bok-poster stemmer mot de opprinnelige vedtakene.

Dette gjør ikke hele hendelseskjeden automatisk korrekt. To publiserte vedtak gjentar samme endring for 1860/01 og 4860/01, og 5999/90 har motstrid mellom forrige saldo og senere førbeløp. Supplerende undersøkelser bekrefter at motstridene også finnes i de publiserte tilrådingene, voteringsforslagene og referatene. De kan ikke avskrives som bare en API-/parserfeil. Sluttsaldo er kontrollert; en rettslig entydig additiv kjede er ikke dokumentert. Bevar kildenes observasjoner og synlige konflikter; ikke fjern like beløp eller opprett en endring bare for å få summen til å stemme. [Versjonsfestet årsavstemming med inventar og avviksledgere](https://github.com/depmartin/budsjetthistorikk/blob/a3a9b90e50e170855b51d87d86fd1d4fe89a02ab/docs/research/issue-2/aar/README.md).

Årsprøven viser dessuten to bevilgningstabeller uten standardinnledning om statsbudsjettet. Kun søk på denne innledningen ville mistet 76 posthendelser. Kandidatinnlesning må bevare alle vedtak og kombinere innhold, tabellstruktur og saksreferanser.

DFØs rå inntektsfortegn er motsatt vedtakets fortegn i hele den kontrollerte 2024-årgangen. Dette er en kildeavhengig normalisering, ikke en endring av regelen om inntekt/utgift etter kapittel. Overføring mellom år er egne felt og holdes utenfor årets bevilgningsendringer.

De to Havtil-postene har dokumentasjon på én økonomisk gjennomføring i departementets tildelingsbrev, som henviser til begge stortingsbehandlingene. Det er ikke funnet en formell uttaksrettelse. Bevar derfor begge vedtaksobservasjoner. Ikke-additiv behandling krever sporbar kontrollavgjørelse, ikke en generell regel som fjerner like beløp. [Supplerende kildeundersøkelse](https://github.com/depmartin/budsjetthistorikk/blob/a03a53aea87360169faa8ee4de212daeb413d625/docs/research/issue-2/dobling/README.md). Brevet er en nettobservasjon fra offisiell PDF med utilgjengelige originalbyte; begrensningen er dokumentert.

For **5999/90** er brutto finansieringsbehov dokumentert som postens økonomiske rolle, men det forklarer ikke motstriden mellom RNB-null og nysalderingens førbeløp. Bevar kontrollert sluttbeløp **120 371 709 000 kroner** separat fra den sperrede additive historikken. En differanse på **101 874 353 000 kroner** skal ikke bli en oppdiktet mellomliggende økning. [Supplerende kildeundersøkelse og fasit](https://github.com/depmartin/budsjetthistorikk/blob/a03a53aea87360169faa8ee4de212daeb413d625/docs/research/issue-2/finansiering/README.md).

## Historiske Excel-filer krever skille mellom observasjon, stadium og hendelse

**Kontrollert 20. oktober 2026:** Alle 13 arbeidsbøker for 2013–2025 på historikkbranchen er lest ved revisjon `da720e9dd4ebfff31d88c14488c5f3217d045786`. SHA-256 og byteantall samsvarer med kilderegisteret før og etter lesingen. Originalene er uendret. [Filkontroll og modellvurdering](research/historisk-excel/modellvurdering.md) har festede kildelenker, inventar og konkrete celler.

Rådata og dokumentarket har ulike detaljeringsgrader og flere dokumentrader per post. En kapittel-/postkobling kan doble dokumentbeløp; dokumentreferanser er ikke automatisk selvstendige beløpshendelser. Hele f150-kolonnen i 2015 er numerisk null og krever særskilt kontrollmarkering. En konkret sammenligning mot vedtak 74 for 2013 støtter millioner kroner i rådata og motsier antakelsen om tusen kroner i dette tilfellet; bred enhets- og stadieavstemming gjenstår. Regnskapskolonne og egen vedtaksdato finnes ikke i de undersøkte arkene.

Konsekvens: bruk filene som konkrete prøver ved videre modellering. Bevar kildeverdier, enhet, underpost, budsjettstadium, beløpsbetydning og dokumentkoblinger før eventuell normalisering. Foreslått felles observasjonskontrakt i rapporten er et modellråd, ikke en vedtatt migrering eller godkjenning av historiske summer. B1/B2s Storting-identitet og prøvedatasett skal ikke brukes som erstatning for en historisk kildeadapter.

## B3-prøver: tabellvariasjon, lokatorer og sperrede kjeder

**Kontrollert 20. oktober 2026:** Den autentiske 2541/70-kjeden for 2024 er nå prøvd deterministisk fra avledede originalbyte gjennom B2, separat B3-lagring, gjenåpning og Excel. Foreldrehash, henteproveniens og reproduksjonsoppskrift finnes i [B3-fixturene](../tests/fixtures/b3/README.md). Avledede utdrag er merket som delvise prøver; syntetiske mutasjoner er egne negative kontroller.

| Vedtak | Nøyaktig 1-basert kildelokator | Kildebeløp, kroner |
| --- | --- | ---: |
| 40032850, nr. 271, 18.12.2023, sak 95779 | `table[1]/tr[92]` | nivå 12 818 000 000 |
| 40033719, nr. 857, 21.06.2024, sak 98919 | delta `tr[1070]`, før/etter `tr[1071]` | −608 000 000, fra 12 818 000 000 til 12 210 000 000 |
| 40033805, nr. 14, 05.11.2024, sak 100001 | delta `tr[4]`, før/etter `tr[5]` | +400 000, fra 12 210 000 000 til 12 210 400 000 |
| 40034064, nr. 221, 17.12.2024, sak 100898 | delta `tr[80]`, før/etter `tr[81]` | +680 000 000, fra 12 210 400 000 til 12 890 400 000 |

Forsknings-CSV-ens `row` er nullbasert og må ikke kopieres direkte til HTML-lokatoren. Originaltabellen 40032850 har seks hodeceller (`Kap., Post, Formål, tom, Kroner, Kroner`), RNB fem, 40033805 fire og 40034064 fem (`Kap., Post, Formål, tom, Kroner`). B1s parserbredde utvides ikke under samme versjon; B3 bruker en separat adapter med disse konservative mønstrene. Underpost-/driftsresultatradene i de samme autentiske vedtakene er fortsatt kontrollbehov i dette snittet. De gir ingen generell underposttolkning eller sesjonsgaranti.

40034443 mangler standardinnledning med år i brødteksten, men tittelen sier uttrykkelig statsbudsjettet 2025. +454 000 000 på 900/32 og −227 000 000 på 1760/45 bevares uten før/etter; «(Ny)» konstruerer ingen nullstart. Rundeetiketter krever tittel eller annet uttrykkelig kildegrunnlag. En desemberdato alene gjør ikke et vedtak til nysaldering.

De autentiske Havtil-overgangene i 40034064/40034226 og 5999/90 i 40033025/40033719/40034287 er regresjonsprøver som **skal sperre den additive kjeden**. Begge Havtil-identiteter, RNBs observerte null og nysalderingens observerte sluttbeløp bevares. 40036289s rå `I 615 833` normaliseres ikke. B3 har ingen generell beløpsdeduplisering, I→1-regel, nullpåfylling eller kunstig mellomendring. Disse kontrollene avklarer ikke de historiske konfliktene faglig.

## B4-prøver: post-24-komponenter og observerte nye nivåer

**Kontrollert 20. oktober 2026:** Komplette vedtaksobjekter er hentet ut byteidentisk fra de allerede bevarte, offentlige sesjonsresponsene. Foreldrehash/byteantall ble kontrollert før avledning. Nye prøver og reproduksjon finnes i [B4-fixturene](../tests/fixtures/b4/README.md); eksisterende B3-fixturer er uendret. Alle lokatorer nedenfor er **1-baserte**. Forsknings-CSV-enes `row` er nullbasert.

| Vedtak / kapittel-post | Hode og komponenter i table[1] | Observert totalcelle | Kroner |
| --- | --- | --- | ---: |
| 40032763, 2445/24, original 2024 | tr[75], tr[76–79]/td[4] | tr[79]/td[5] | −334 642 000 |
| 40032791, 2460/24, original 2024 | tr[99], tr[100–101]/td[4] | tr[101]/td[5] | 102 500 000 |
| 40032850, 2470/24, original 2024 | tr[81], tr[82–87]/td[4] | tr[87]/td[5] | −15 000 000 |
| 40032976, 5440/24, original 2024 | tr[57], tr[58–62]/td[4] | tr[62]/td[5] | 295 900 000 000 |
| 40033719, 5440/24, senere oppstilling | tr[1367], tr[1368–1372]/td[4] | tr[1373]/td[4], Sum: | 191 800 000 000 |
| 40034064, 2470/24, senere oppstilling | tr[71], tr[72–77]/td[4] | tr[78]/td[4], tomt formål | −15 000 000 |
| 40034226, 5440/24, senere oppstilling | tr[46], tr[47–51]/td[4] | tr[52]/td[4], tomt formål | 233 300 000 000 |

2470s seks originalkomponenter er −730 000 000, +594 000 000, +90 000 000, +1 000 000, +55 000 000 og −25 000 000 kroner. De summerer eksakt til den **separat observerte** totalcellen. Kildens komponentnummer står i formålsteksten; navnene beholdes, også når SDØEs oppstilling bruker andre navn enn forvaltningsbedriftene. Negative nettoresultater og «Driftsinntekter» på en komponent endrer ikke kapittelets utgiftsside.

De senere oppstillingene er nye **nivåer**, uten kildeobservert delta i disse post-24-blokkene. Forskningsmaterialets −104 100 000 000 og +41 500 000 000 er beregnede differanser, ikke egne kildebeløpsceller. B4 bevarer derfor etterbeløpet og komponentene, med sperret additiv saldo (`mangler_delta`). Dette gjelder også 2445/24-oppstillingen i 40035422 (2025), −369 642 000 med Sum-rad; ingen automatisk −5 mill.-endring konstrueres.

Post-90-prøven 40033025 bevarer blant annet 2410/90 `tr[17]/td[4]` 39 751 273 000 med «overslagsbevilgning», 5310/90 `tr[45]` 13 970 169 000, 5310/93 `tr[46]` 8 287 563 000, 1651/98 `tr[13]` 68 000 000 000 og 5999/90 `tr[62]` 101 874 353 000 kroner. Disse er budsjettkapitler selv om postene gjelder finansielle transaksjoner. 40034287s nye 2800/96 `tr[65]` bevarer 42 800 640 000 uten oppdiktet nullstart. Eksisterende ANNET-, Havtil-, finansierings- og rå-I-prøver består uendret som kontrollgrunnlag.

Fullmaktsprøven 40035429 har 72 mill. kroner i forpliktelsesramme i `/html/body/div/div/p` (første p under første indre div), ikke en årsbevilgning. 40034385s `/html/body/div/p` er initiativ til senere bevilgning. Begge gir null beløpsobservasjoner og kan eksporteres selvstendig med fulltekst og separat tekstklassifikasjon. Årsøkningen 41/45 på 9 700 000 i 40035422 er en egen bevilgningsobservasjon. Ingen generell fullmaktsparser eller manuell kontrollavgjørelse er innført.

### Register og kapitalgrense: bevisets begrensning

B4 bruker de ni tidligere dokumenterte oppslagene i [departementsregisteret](departementsregister.md) som avgrenset datagrunnlag for **bare 2027**, med artefakthash `952757a9964f92a7e2cb1972fcfb6b82b426d4973de641a29fef5ea66d6c1adb`. Originalarbeidsboken ble ikke gjenfunnet og cellene er **ikke kontrollert på nytt i B4**. Kode 23 bevares som Ymse, fdep og gdep holdes separate, og ingen +3000-/intervallkobling er bekreftet ved implementering. 5531 FIN mot 2531 BFD er tidligere dokumentert negativt bevis mot automatisk −3000, ikke en ny cellekontroll. Historiske 2024/2025-prøver får ingen 2027-organisasjon. Regnekontroll er separat fra organisasjonens kontrollstatus.

Kapitalgrensen bygger på dokumentert R-101/2024 (vedleggshash `813b9b0f8dc24f2414387cf32bc1ce4ba16a9e42855ccc4c0ed60d96b0592f92`), tabellen på side 2 og forklaringen på side 3, jf. [faggrunnlaget](faggrunnlag.md). 1–2999 er utgift, 3000–5999 inntekt og 6000–9999 kapitalregnskapskonti. Ingen autentisk 6000+-rad ble funnet i de undersøkte bevilgningskildene. Grensekontrollene er derfor uttrykkelig **syntetiske**, ikke nye kildefunn om bevilgninger på kapitalregnskapskonti.

Prøvene gjelder støttede mønstre og kontrollavvik, uten generell årsdekning, organisasjonsgodkjenning eller løsning av de tre historiske kjedekonfliktene. B3-historikkeksportens rå rad-HTML var ikke hele vedtakets fulltekst; B4 legger hele den valgte B2-fullteksten til begge eksportformene med tegnbevarende videreføring.

### Syntetiske kontrollgrenser etter B4-review

**Kontrollert 20. oktober 2026:** Separate syntetiske mutasjoner viser at et utvidet `rowspan`/`colspan` i tabellhodet og flerleddede komponentkoder som `1.25` må sperre v2s beløpstolkning/avstemming gjennom lagring og Excel. Dette er robusthetsprøver, ingen nye funn om feil i Stortingets historiske kilder. Den frosne v1-parseren endres ikke under samme identitet; ny konservativ tolkning krever uttrykkelig v2. Kildeuavhengige kontraktprøver bevarer dokumenterte underpostkoder `0`, `10` og `25` uten Storting-spesifikke nummereringsavvik. Et [syntetisk arkiv fra den leverte B3-basen](../tests/fixtures/synthetic-history-v1.md) kontrollerer samme v1-identitet og sperrede saldo både ved ny beregning og med et resultat allerede lagret.

Komponenttilknytningen behandler bare indeksene i aktuell blokk. En manuell prøve gjennom offentlig `extract_revision` over 800/1 600/3 200 syntetiske blokker (114 560/228 960/457 760 HTML-tegn) brukte henholdsvis 2,163/7,979/30,994 sekunder før rettingen og 0,396/0,799/1,617 sekunder etter, målt i samme lokale Python-miljø. Målingen gjelder v2-kallet med kilde/B2 allerede lagret, inklusive lagring av nytt uttrekk. Den demonstrerer tilnærmet lineær vekst for denne prøven og er ingen generell tidsgrense for maksimal kildestørrelse. CI har en deterministisk prøve med 160 blokker, begge totalplasseringer, separate komponentforeldre og Excel, uten veggklokkekrav. Autentiske kildefixtures er uendret.

En egen kontroll med ugyldige blokker (komponent 7, observert total 8) avdekket også kvadratisk medlemskontroll av hierarkiavvik ved lagring. Et midlertidig sett bygges nå én gang for oppslag; den opprinnelige avvikstuppelens rekkefølge og gjentakelser bevares. Samme lokale prøve gjennom offentlig v2-kall over 3 200/6 400/12 800 blokker (457 761/915 361/1 830 561 HTML-byte), med B2 allerede lagret, brukte 2,583/7,195/22,624 sekunder før og 1,599/3,204/6,725 sekunder etter. Gyldige blokker beholdt tilnærmet lineær vekst: 1,572/3,223/6,579 sekunder etter. CI kontrollerer funksjonelt 320 ugyldige blokker med alle avvik og kildeceller gjennom gjenåpning og Excel, sperret saldo, bevarte gjentakelser og avvisning av skjult siste avvik. Tidsmåling og instrumentering av likhetssammenligninger ligger utenfor testsuiten; dette er ingen generell tidsgrense for 32 MiB-kildegrensen.

## B5: kontrollbevis og registergrunnlag

**Kontrollert 21. oktober 2026:** Offentlig gjenhenting av [referatets XML](https://data.stortinget.no/eksport/publikasjon?publikasjonid=refs-202526-03-26) kl. 07.14.46 UTC ga HTTP 200, 595 225 byte og SHA-256 `4eed3a96b705a6bc80f9f7776efbde1c3dab07f36b898ed4722617ff59ea5b56`. Hele originalen er byteidentisk med #2s bevarte XML. Den nøyaktige lokatoren `/Forhandlinger/Mote/Hovedseksjon/Saker/VoteringerStart/Voteringer[7]/Sakdel/Presinnlegg[17]/Liste/Pkt[6]/Tbl/table/tgroup/tbody/row[3]/entry[3]/A` treffer én node med fullstendig etterbeløp 1 615 833 000, første tegn siffer `1` (U+0031), med NBSP som gruppeskille. [Vedtaksobjektet](https://www.stortinget.no/no/Saker-og-publikasjoner/Vedtak/Vedtak/Sak/?did=40036289&p=107811) og den bevarte B3-fixturen beholder rå ettertekst `I 615 833`. Dette er et representasjonsavvik, ingen dokumentert rettelse av API-vedtaket.

Et smalt [deterministisk referatutdrag](../tests/fixtures/b5/README.md) bevarer eksakt 7 148 byte fra originalens nullbaserte byteposisjon 578 380. Utdragets egen SHA-256 er `7fa34518b05f948e7ff834995e97513a492262790be8445609bc453c9a09ff51`; foreldrehash og både original-/utdragslokator følger sidevognen. B5-rundturen viser at en uttrykkelig kontrollør kan godkjenne akkurat `etter_belop` for 5538/70 med dette beviset, samtidig som råverdi, ukjent rått kronebeløp og avvik beholdes. Førbeløpet deler fysisk celle, men har annet beløpsfelt og endres ikke. Ingen I→1-regel eller nullpåfylling innføres. CI henter ikke nett. Dette kontrollankeret godkjenner ikke andre felt, kjeder eller år.

Gul bok-originalen er ikke gjenfunnet eller kontrollert på nytt i B5. Startregisteret bruker kun brukerens navneoppsett og de ni 2027-koblingene med tidligere filhash `952757a9964f92a7e2cb1972fcfb6b82b426d4973de641a29fef5ea66d6c1adb`. Postkatalogen starter tom. Prøven 40034443 viser fortsatt +454 000 000 kroner på 900/32 i 2025 ved `table[1]/tr[4]/td[4]`; [opprinnelig katalogundersøkelse](research/issue-2/ny-katalogpost.json) dokumenterer at kapittel 900 fantes, mens post 32 ikke fantes. B5 krever eksplisitt katalogkombinasjon og 2025-organisasjonsgrunnlag ved avklaring. En godkjent katalogpost gir ingen inngående null og ingen løsning på kjedens manglende start. Alle tidligere kildeprøver og sperrede historiske konflikter består.

## B6: fullt inventar og utført beløpskontroll er forskjellige bevis

**Kontrollert 21. oktober 2026:** Begge hashkontrollerte originalinventarene fra 2023–2024 og 2024–2025 er prøvd offline gjennom B2, 50 uttrykkelige v2-uttrekk og samlet B6-Excel. Alle 2 183 ID-er og fem API-typer ble beholdt, også de 2 133 ID-ene uten valgt beløpsuttrekk. Hovedsesjonens 1 260 ID-er og supplementets 923 fikk separate dekningsrader. Kildeinnhold var komplett for disse bevarte inventarene; struktur og faglig dekning var fortsatt ufullstendig. De 5 492 beløpsobservasjonene er ikke samme telleenhet som forskningsrapportens posthendelser. Uavklarte tabell-/kontofelt i det bredere utvalget beholdt sperret historikk. Ingen gammel kontrollprosent eller teknisk saldo ble kopiert som faglig godkjenning. [Kontrolloppskrift, kildehash, begrensninger og konsekvenser](research/b6/README.md).

Den nye reproduksjonen av #2 beregnet 1 625 eksakte felles DFØ-/Løyving-poster fra bevarte råfelt, 43 forklarte omfangsforskjeller med manglende side som `None`, og 1 574 eksakte opprinnelige API-/Blå bok-poster. Dette kontrollerer avledede, hashfestede 2024-artefakter og er ingen ny original-PDF-kontroll eller automatisk avstemming av et annet sesjonsutvalg. Manglende eksportavstemming må fortsatt vises som ikke utført.

Nye komplette, byteidentiske prøver for ANNET 40034048 og 40034229 bevarer alle 76 posthendelser uten standardinnledning. Forelderen er SHA-256 `9cfeaef59510a54ff8b2a695e0be368e67cfbab574f8d3f466c0c2f0c3c92680`; utdragenes SHA-256 er henholdsvis `2a540261f110b761a0213516c8ad72844d0285744ca0f1cdd4cb1afce06f0850` og `66208daf51111356ad73c26985819870ab9c2f97ec7b070024d89e150cd772b9`. Nøyaktige byteposisjoner/proveniens følger [B6-fixturene](../tests/fixtures/b6/README.md). Dette er delvise enkeltvedtaksprøver, ingen fullsesjonsgaranti. Konsekvensen er fortsatt at type/innledningsfrase ikke kan brukes som inngangsfilter, og at uavklarte kilder må synes selv uten beløpsuttrekk.

## Historisk Excel: avgrenset 2024-prøve og adaptergrenser

**Kontrollert 21. oktober 2026:** [Tallprøven](research/historisk-excel/pilotkontroll.md) sammenligner den uendrede 2024-arbeidsboken ved `da720e9` (SHA-256 `870d30d55b4f7f6791fe48ea2a15aa3e98d61946393385d0411e46a0169f60f3`, 257 569 byte) med tolv allerede bevarte, autentiske enkeltvedtak gjennom uendret B2/SQLite og uttrykkelig Storting-v2. Alle 2 894 observasjoner er lest tilbake med identisk innhold; gjentakelse er idempotent. Rapportens manifest identifiserer foreldrebyte, fixtures, adapterhash, kilde-ID-er og lokatorer. Dette er et avgrenset utvalg uten årsdekningspåstand.

Saldertprøvens 375 API-postnivåer gir 271 eksakte hele kronekandidater, 103 rå OOXML-presisjonsspor og manglende Excel-nøkkel 5999/90. Ingen avrunding godkjenner presisjonssporene. Sju senere vedtak gir 854 eksakte postdelta-kontroller og sju rester på unionen av valgte gruppenøkler. Råbeløpet 30 000 000 på 228/85 finnes i 40033719 `table[1]/tr[143]/td[5]`, men v2 klassifiserer det som uavklart. 40034226 `table[1]/tr[37]` har `(NY) 31` og 11 900 000 000 på 2440/31, men v2 lager ingen beløpsobservasjon. Fravær av sikkert delta og fravær av råtall er dermed ulike funn. Seksten avledede komponentdifferanser gir tolv eksakte Excel-treff og fire Excel-fravær ved beregnet 0; de er ingen nye observerte API-deltaer.

**Konsekvens:** [pilotplanen under #13](pilotplan-historisk-excel.md) anbefaler 2024 med disse regresjonsankrene. Råbevaring og kontrolluttrekk kan bygges med uavklarte felt; generell kolonnesemantikk, presisjon og historisk organisasjon krever videre avklaring før faglig bruk. 1860/1, 4860/1 og 5999/90 forblir sperret. Nye offisielle kilder skal kunne leses inn uten historisk Excel eller startsaldo. Prøven implementerer ingen historisk adapter, endrer ingen tidligere parser/ID og lukker verken #13 eller #10.

## Vedlikehold av funn

### B8: saksdokumenter, nil og separat stikkordvisning

**Kontrollert 22. oktober 2026:** [B8-kildeprøven](research/b8/README.md) dokumenterer komplette offentlige saks-API-originaler for 100927 (12 383 byte, SHA-256 `2ee25b327b78772523d56317c752e35f5134eef60db9536f6dea3c94ad8fed27`) og 100889 (15 888 byte, SHA-256 `3a8f0918a3fcce90bf2c93f3ce972c3de7277c76e27e5ef563d6c43384cf2af2`). Hver har fem publikasjonshenvisninger. Proposisjonens eksport-ID er nil selv om etikett/URL finnes. Referatet har samme eksport-ID for to ulike debatt-/voteringslenker; ID alene er ingen unik henvisning. Begge saker gjelder Prop. 16 S, men henholdsvis Innst. 81 S for kap. 1429 og Innst. 95 S for resten. Gjensidig `sammekilde` innebærer ingen arvet post- eller innstillingstilknytning.

Den uendrede B6-prøven 40034048 viser formelt vedtak 210 (2024–2025), 1429/1 +5 796 000 fra 160 243 000 til 166 039 000 og 1429/22 −3 000 000 fra 32 185 000 til 29 185 000. Post 22s formålsfelt har kursivmerket «kan overføres» på `table[1]/tr[5]/td[3]`. Et nytt byteidentisk utdrag av 40034049, formelt 211, bevarer en separat stikkordsfullmakt om 1429/60 uten beløpsrad. Utdragets hash/forelder og gjenlesingsprøven er dokumentert i [B8-rapporten](research/b8/README.md).

**Konsekvens:** Dokumentreferanser og stikkord skal berike vedtaksvisningen separat fra immutable beløpsobservasjoner. Nye kilde-/tolkningsbindinger og feil/ferskhet må være synlige; ingen dokumentjoin skal multiplisere beløp. Råoriginalene inneholder også offentlige parlamentariske biografidata og er ikke anonymisert; normalisert B8 begrenses til saks-/dokumentmetadata. Ingen dokumentfulltekst eller forslagsbeløp er hentet. Kildeprøven dekker to saker, ikke sesjon/år, og lukker ingen drifts- eller historikkrest.

**Syntetiske regresjonskontroller 22. oktober 2026:** [B8-prøvene](../tests/test_b8.py) endrer proposisjonens PRP-kode til et annet nummer, sesjon eller serie uten å endre etiketten; det må gi motstrid. En ukjent lenkekode gir uavklart identitet, mens originalens nil eksport-ID fortsatt er legitim. En tom kursivmarkør må ikke skjule umerket «kan overføres», og ett kjent markert stikkord må ikke skjule et annet umerket, ukjent eller ufullstendig stikkord. Råtekst/HTML og lokator bevares; kjente ord vises sammen med uavklart status i faktisk Excel. Kontrollerte avbrudd og samtidige kall ved SQLite-grensen viser at første responsbyte og metadata låser forsøket; andre byte/metadata avvises, identisk gjenopptak lykkes. HTTP-portprøver viser at lesefeil i feilinnhold avslutter forsøket og lukker responsen, uten oppfunnet råhash. Eksplisitte delbyte får sin faktiske hash og status som delrespons. Dette er feilprøver av den lokale B8-kandidaten, ingen nye kildefunn, HTTP-hentinger eller endringer i tidligere lagrede resultater.

### B9: kildeforankrede navn og avledet hovedvisning

**Kontrollert 22. oktober 2026 på samme bevarte 210-original:** `chapter_name` er Riksantikvaren, mens `purpose` inneholder postnavn sammen med handlingsord og eventuelle stikkord. Kapittelraden er `table[1]/tr[2]/td[3]`; post 1 og 22 står på henholdsvis tr[3] og tr[5]. [B9-kontrollen](research/b9/README.md) dokumenterer utskillingen av Driftsutgifter og Flerårige prosjekter kulturminneforvaltning uten dagens register. Den nye hovedvisningen skal ikke omtolke generelle nivåbeløp til etterbeløp eller velge mellom motstridende kildeverdier. Tidligere detaljfelt og råtekst beholdes. Lange detaljfelters videreføringspekere må følge kolonneinnsetting og omdøping av arket; råinnholdet endres ikke. Dette er et presentasjonsfunn, ingen ny innhenting eller faglig beløpsgodkjenning.

### B7: sesjonsliste, forsøk før HTTP og prøvens grenser

**Kontrollert 21. oktober 2026:** Den offisielle [dokumentasjonen for sesjoner](https://data.stortinget.no/dokumentasjon-og-hjelp/sesjoner/) angir rot `sesjoner_oversikt`, `innevaerende_sesjon`, `sesjoner_liste/sesjon` og feltene `id`, `fra`, `til`. Den sier uttrykkelig at en fremtidig sesjon kan ligge i listen, og beskriver dato/tid som lokaltid. Dokumentasjonseksemplet bruker `https://data.stortinget.no` som navnerom; tidligere bevarte vedtakskilder bruker `http://data.stortinget.no`. B7s sikre sesjonsparser godtar disse to eksakte navnerommene. Dette er kontroll av dokumentasjonen, ingen ny bevart live sesjonsrespons eller påstand om faktisk sesjonsskifte. **Konsekvens:** bruk offisiell liste og startet periode, ikke maksimal ID. Alle startede produksjonssesjoner fra 2026–2027 kontrolleres fullt hver dag; ingen aldersgrense innføres for rettelser.

Den deterministiske B7-prøven setter ni allerede bevarte autentiske vedtaksobjekter i tydelig syntetiske, komplette testkonvolutter for tre sesjoner. Originalfixturene er uendret og hashene følger den syntetiske proveniensen. Hele runnerløpet bevarer ANNET 40033719/40034287, de 76 posthendelsene uten standardfrase i 40034048/40034229, rå `I 615 833` i 40036289 og sperrede 1860/1-, 4860/1- og 5999/90-kjeder i frosset B6-JSON/Excel. Supplerende sesjoner har separate dekningsrader. Konvoluttene er **ikke** hele ekte sesjoner, og teknisk testsuksess er ingen ny årsdekning eller løsning på kildekonfliktene.

Nye syntetiske forsøk demonstrerer at en timeout før B2-staging må bevares uten oppfunnet råhash, slik at gamle faglige verdier blir `ikke vurderbar` i B2/B5/B6. Tapt staging-/Excel-/GitHub-POST-kvittering kan gjenfinnes eller avstemmes uten ny blind kilde-/issueopprettelse. Dette er deterministiske avbruddsprøver; ingen installert Windows-oppgave, live GitHub-varsling eller faktisk 06-kjøring er demonstrert. Eierens valg og gjenstående driftsaksept finnes i [B7-manualen](b7-drift.md).

Den samlede [B7-kontrollrapporten](research/b7/README.md) beskriver den utførte Windows-testsuiten, den symbolske låseprøvens begrensning, de 2 663 bevarte beløpsobservasjonene og varslingsrestansen i den syntetiske prøven. Ingen testvolum eller avledet kontrollprosent er produksjonsaksept.

**Syntetisk regresjonskontroll 21. oktober 2026:** En gyldig, ikke-tom sesjonskatalog kan i en feilprøve utelate en tidligere kontrollert sesjon mens en annen fortsatt finnes. En slik liste må ikke erstatte kjent kontrollomfang: unionen beholdes i HTTP, frosset B6 og Excel, og fraværet gir `sesjon_mangler_i_katalog` i kjørerapport/outbox. [Prøven](../tests/test_b7_sessions.py) bevarer både et forsinket vedtak og en rettelse i den utelatte sesjonen, gjentar avviket samme/neste dato med samme issue og utelater en uttrykkelig fremtidig katalogperiode fra innlesning. Dette er ingen observasjon av faktisk bortfall i Stortingets katalog.

En separat [filfeilprøve](../tests/test_b7_controlled.py) bruker et ellers godkjent nullbeløp og avviser bare JSON-filpublisering ved OS-grensen. `kjorerapport_fil_feilet` må lagres før GitHub-levering, også uten andre avvik. Én publiseringsrunde og én leveringsrunde per start bevarer både feilvarsling og grensen på 100 outbox-rader. JSON-filen viser status før levering; SQLite/returverdi viser kvitteringen etterpå. Samme forhold bruker samme issue over forsøk/datoer; manglende bakgrunnstilgang lar varselet stå i kø uten nye credentials. Dette er syntetiske feilprøver, ingen utført driftsaksept.

Oppdater eksisterende funn når nye prøver presiserer det. Bevar skillet mellom observert kildeinnhold, en designanbefaling og et åpent spørsmål. Vesentlige nye funn skal få en kort inngang fra AGENTS.md eller relevant fag-/arbeidsdokument, slik at neste økt finner dem uten chatloggen.

## Hele den historiske 2024-piloten

**Kontrollert 21. oktober 2026:** [Hele pilotkontrollen](research/historisk-excel/pilot2024.md) har lest original SHA-256 `870d30d55b4f7f6791fe48ea2a15aa3e98d61946393385d0411e46a0169f60f3`, 257 569 byte, fra revisjon `da720e9`. SQLite og faktisk kontrollpakke/Excel er gjenlest. Begge ark gir 44 652 fysiske celler og 2 136 fraværende posisjoner, samlet 46 788 inventarposisjoner og 16 339 beløpsobservasjoner. Originalen er uendret; fullstendige inventarer og kandidater behandles lokalt.

Hele H-unionen mot hashfestet Blå bok-uttrekk har 1 694 nøkler: 847 eksakte hele kronekandidater, 726 desimalspor, 120 Excel-nøkler uten referanse og manglende Excel-konto 5999/90. Alle 120 har rå H=0; de er fortsatt ikke treff. Hele dokumentkontrollen mot det separate forskningsuttrekket har 1 359 unionnøkler: 1 354 eksakte og fem rester. Forskningsrepresentasjonen inkluderer 228/85 og 2440/31; den er ikke en parserutvidelse eller ny full v2-replay.

Den avgrensede v2-prøven er gjentatt separat: 2 894 observasjoner, H 271/103/1, dokumentdelta 854 treff/sju rester, komponenter tolv treff/fire Excel-fravær ved avledet 0. De tre kjedekonfliktene består. G er prøvd mot faktisk Gul bok-forslag og I mot faktisk RNB-forslag. M og N har uttrykkelig uprøvde, åpne sammenligninger. Konkrete URL-er, hasher og lokatorer står samlet i kontrollrapporten.

**Konsekvens:** bruk den separate historiske adapteren og [pakkegrensen](historisk-pilot.md) ved videreføring. Ingen generell enhets-, presisjons-, hierarki- eller organisasjonsgodkjenning følger av treffene. Nye offisielle observasjoner lagres og eksporteres uavhengig av historisk fil/register/start; bare startavhengige analyser sperres. #13 gjelder øvrige år og #10s faktiske driftsaksept gjenstår.

**Rettet og kontrollert 21. oktober 2026:** Ny historisk tolkning v2 bevarer den tidligere v1-databasen og fullpakken. Dokumentarkets J er kapittelnavn, H er postens formål og I er separat rå stikkordstekst. Alle 1 371 navn-/formålspar er kontrollert mot originalen og faktisk ny Excel. En tom OOXML-formel har fortsatt formeltilstedeværelse og sperrer cache som kandidat. Samlet løst innhold og gjentatte råkontekster har egne grenser; små shared-string-prøver gir varig avvisning før uttrekk. Sammenligningsgrunnlag v2 krever bundet matematisk kontrollprofil og referansens faktiske kildeår; likt beløp med uforenlig år/enhet/betydning gir ikke treff. Runneren beskytter alle kilde-/kontrollfiler før første skriving, også originalen kalt `summary.json`. Originalhashen og de dokumenterte H-/D-/v2-resultatene er uendret. Bruk ny uttrekks-ID og ny pakkekatalog ved rettet tolkning; gamle lagrede ID-er skal aldri få nytt innhold.

**Syntetisk områderegresjon 21. oktober 2026:** I OOXML kan bare ankercellen ha `<f t="array" ref="H2:H3">`, mens H3 har numerisk cache uten egen formel. Egen formeltilstedeværelse alene sperrer derfor ikke alle formelresultater. [Offentlige import-/sammenligningsprøver](../tests/test_historical_excel.py) viser nå at v3 bevarer cache, egen XML og områdets anker/ref/type, men sperrer begge cellers kandidater og mulige treff. Shared- og dataTable-områder har samme konservative resultatgrense. Ugyldige/overlappende områder og samlet areal over posisjonsbudsjettet avvises med originalbyte bevart. Reversert XML-rekkefølge og fysisk cache utenfor arkdimensjonen skjuler ingen cache. Områder utvides ikke til nye inventarceller. Dette er en syntetisk robusthetsprøve; den autentiske 2024-originalen har fortsatt ingen formler. Eksisterende v1/v2 må leses uendret, og ny tolkning må ha v3-identitet og egen lokal fullpakke.

### O2a: gjenlesing av samme O1-originaler

**Kontrollert 22. oktober 2026:** [O1-bevisene](research/omtale-o1/README.md) er grunnlaget for den avgrensede #34-adapteren. Kap. 1429-overskriften er DOM-søsken til P1 og må bindes med egen lokator. Hele HTML-P1 samsvarer med PDF-side 3 etter fjerning av PDF-mellomrom/orddeling; dette er passasjesamsvar, ingen full dokumentekvivalens. Regjeringens avrundede lønnsanslag må ikke bli en eksakt restkomponent. Komitéfraværskontrollen leser hele Innst. 81 S; ukjent støtterolle er en annen status enn kontrollert fravær av mindretall. Ingen ny HTTP er gjort i O2a.

**Konsekvens:** [Pilotkontrakten](omtale-pilot.md) bevarer komplette originaler og uendret B8-grunnlag separat fra schema 5. Den autentiske 210-prøven bruker `step_id` som posthendelsesgruppe; det valgfrie `event_id` i observasjonene er null og skal ikke omskrives. De seks observasjonene gir fortsatt to posthendelser. [Kandidatkontrollen](research/omtale-o2a/README.md) skiller teknisk gjenlesing fra faglig godkjenning og faktisk drift. #10 står åpen.

**Retterkontroll 22. oktober 2026:** Omberegnede rapport-ID-er beviser ikke hendelser eller observasjoner. Vedtaksradene må stemme med samme kildebundne uttrekk og originalens lokale tabellgruppe, råfelt og hendelsesregel. KT/V kan nevne 1429 i innledning eller post 60 selv når selve beløpstabellens kapittel er feil. KS-utsagnet «støtter regjeringens forslag» beviser heller ikke en samlet komité uten det navngitte avsenderbelegget. Merkede syntetiske endringer av disse feltene og Excel-padding er dokumentert i [rettingsbevisene](research/omtale-o2a/retting-review-audit.md); de er ikke nye autentiske kildefunn.

**Andre retterkontroll 22. oktober 2026:** XML-original `b6/40034048.xml`, SHA-256 `2a540261f110b761a0213516c8ad72844d0285744ca0f1cdd4cb1afce06f0850`, har `sesjon_id=2024-2025`. Identisk HTML alene kontrollerer ikke dette feltet eller vedtakets øvrige metadata. `chapter_raw` må være tabellens 1429, også når et konsistent snapshot hevder 1428. I OOXML er `hyperlink/@ref` et mulig celleområde selv uten nye eksplisitte celler; den avgrensede eksporten produserer bare enkeltcellelenker. [Andre retterbevis](research/omtale-o2a/retting-etterkontroll2.md) viser avvisning av de eksakte feilfilene og små sentinelprøver før inputinnlasting. **Konsekvens:** bind konvolutt, vedtaksmetadata og hele rå kontokonteksten til originalen, og kontroller alle tillatte område-/indeksfelter før openpyxl får input. B2s UUID beholdes som referanseidentitet; den er ingen kildeobservert XML-verdi eller ny innholdshash. Dette er syntetiske robusthetsprøver med uendrede autentiske originaler, ingen ny HTTP, årsdekning eller faglig godkjenning.

**Siste defensive retterkontroll 22. oktober 2026:** XML-kildens dupliserte metadata må også svare til den bevarte, hashfestede JSON-sidevognen. En syntetisk endret metadata-URL med uendret XML og sidevogn er dokumentert i [sluttrettingen](research/omtale-o2a/retting-finalaudit.md). Hele metadataobjektet avstemmes uten overskriving av rådata; senere B2-konvolutter er fortsatt separate kildeobservasjoner. Støttemanifestet leses én gang med faktisk 1 MiB-bytebegrensning før JSON-dekoding og strukturkontroll. Avvik beholder mottatte sidevogner og synlig status. Ingen ny kilde eller nettverkskontroll inngår.

**O2b-kontroll 23. oktober 2026:** De samme O1-originalene dokumenterer P22/K22s reduksjon på 3 mill. og tilbakepeking til post 1. P1 er fortsatt én seksjon: omdisponeringsutsagnet har separate relasjoner til de to eksisterende posthendelsene; lønnsutsagnet gjelder bare post 1. Omtalens kulturmiljøforvaltning og tabellenes kulturminneforvaltning beholdes som forskjellige rånavn. [O2b-kontrollen](research/omtale-o2b/README.md) viser faktiske gjenleste filer, separate filtre, uavklart syntetisk tilleggsforslag og gamle A-filer uten omskriving. **Konsekvens:** velg ny B-uttrekksversjon uttrykkelig, kontroller post 22s lokale kapittel-/post-/fra-til-gruppe og bevar A-algoritmen. PN/post 60/Vega er fullmaktskontekst uten 210-beløpsrelasjon. Ingen ny HTTP, kildeversjon, beløpsobservasjon, årsdekning eller faglig godkjenning følger av B.
