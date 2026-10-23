# Plan og spesifikasjon for kildeforankret budsjettomtale

Status 23. oktober 2026: Behovet og den samlede testgrensen er bekreftet. O1-kildegrunnlaget og O2-oppdelingen er godkjent; O2a/#34 er flettet i PR #36 (main `6f7145d`), og O2b/#35 i PR #39 (main `5423160`). [O2a-kontrakten](omtale-pilot.md), [godkjent oppdeling](research/omtale-o1/o2-forslag.md) og [O2b-kontrollene](research/omtale-o2b/README.md) beskriver leveransen. [Konkretiseringen under #37](visningspilot-plan.md) legges frem med kildebevis, testmatrise og ticketutkast før publisering/implementering. O3–O5 er fortsatt foreslåtte spor. Gjeldende leveringsstatus og kommentarer skal leses i GitHub før videre arbeid.

[Dokumentvisning og konto-/årsvisning](to-visninger.md) er det autoritative målbildet for eierens presisering 23. oktober, med konkretisering i [#37](https://github.com/depmartin/budsjetthistorikk/issues/37). Det samler de to inngangenes krav og aksept og avgrenser dem mot O2a/O2b. Denne omtaleplanen eier fortsatt tekstbelegg og temasøk; planens pilot er ingen implementering av de generelle visningene.

Del av målbildet i [#1](https://github.com/depmartin/budsjetthistorikk/issues/1). Se også [kravgrunnlaget](krav.md), [leveranseplanen](leveranseplan.md), [observasjonsformatet](observasjonsformat.md) og [ansvarsdelingen](ansvarsdeling.md).

Gjeldende overordnet omtalespesifikasjon: [#32](https://github.com/depmartin/budsjetthistorikk/issues/32), del av #1. Les også kommentarene der før videre arbeid.

**O1-oppfølging 22. oktober 2026:** [Kildeundersøkelsen](research/omtale-o1/README.md) har bevart og kontrollert originalene, postomtalen og kjeden til vedtak 210. [O2-piloten og de to komplette byggeticketene](research/omtale-o1/o2-forslag.md) er siden godkjent og publisert som #34/#35. O1-kildebevisene beholdes uendret; O2a-kandidatens faktiske kontroller står i [kandidatrapporten](research/omtale-o2a/README.md).

## Problem

Brukeren vil velge et kapittel eller en post, se hvor bevilgningen ble endret i et budsjettår og hente frem den konkrete kapittel- og postomtalen i proposisjon og innstilling som forklarer forslaget og behandlingen. Dokumentnummer alene gir ikke denne forklaringen. Brukeren vil også kunne undersøke endringer på tvers av år med et spørsmål som «hvilke bevilgningsendringer skyldtes tema X?», med etterprøvbare tekstbelegg og synlige grenser for hva materialet faktisk beviser.

[B8/#28](b8-saksdokumenter.md) er levert med saksdokumentmetadata, kildehenvisninger og separat stikkordvisning. [B9/#30](b9-historikk.md) er levert i [PR #31](https://github.com/depmartin/budsjetthistorikk/pull/31), og Historikk er aktiv hovedvisning med 13 kolonner. Det er et utgangspunkt for å finne saken, men beviser ikke postvis tilknytning til et forslag eller en begrunnelse. Ingen av leveransene leser proposisjonens og innstillingens fulltekst som strukturert omtale.

De [bevarte B8-prøvene](research/b8/README.md) dokumenterer vedtaksbeløp og saksrelasjonen til Prop. 16 S og Innst. 81 S (2024–2025). B8 beviste ikke hvilke avsnitt som forklarer 1429/1 og 1429/22. Det godkjente [O1-kildegrunnlaget](https://github.com/depmartin/budsjetthistorikk/blob/417e4fdeb22c8c510a56d038686cbf5ffa740cd2/docs/research/omtale-o1/README.md) har siden dokumentert den avgrensede post-/behandlingskjeden. Det dokumenterer verken komitéendring, full dokumentstrukturering eller årsdekning.

## Løsning

Bevar offisielle originaldokumenter og deres versjoner, strukturer omtalen med presise kildepekere, og knytt passasjene til dokumenterte behandlingsledd og kapittel/post uten å endre tidligere beløpsobservasjoner. Brukeren skal fra en valgt post kunne finne vedtaksendringen, lese relevant originaltekst i dens sammenheng og skille regjeringens forklaring, komiteens vurdering og det endelige stortingsvedtaket.

Omtale og beløp skal kunne eksporteres strukturert til JSON og Excel med identiteter, versjoner, relasjoner, belegg og kontrollstatus. Full tekst og originalstruktur skal bestå selv om en visning bare bruker et utdrag. Dette gir et kildeforankret grunnlag for senere søk, KI-baserte sammendrag og temaoversikter. Et søketreff er ikke i seg selv bevis for at temaet forårsaket beløpsendringen.

## Brukerhistorier

1. Som budsjettanalytiker vil jeg velge budsjettår, kapittel og post, slik at jeg finner de dokumenterte endringene som gjelder utvalget.
2. Som budsjettanalytiker vil jeg se dato, behandlingsrunde, talltype og beløpsbetydning ved hvert ledd, slik at et regjeringsforslag ikke forveksles med et endelig stortingsvedtak.
3. Som budsjettanalytiker vil jeg åpne den konkrete postomtalen fra en bevilgningsendring, slik at jeg kan undersøke forklaringen uten å lete gjennom hele dokumentet.
4. Som budsjettanalytiker vil jeg lese både proposisjonens og innstillingens relevante passasjer, slik at jeg kan se hva regjeringen foreslo og hva komiteen endret eller begrunnet.
5. Som budsjettanalytiker vil jeg se hvem som står bak en merknad eller et forslag, slik at en mindretallsmerknad ikke fremstilles som begrunnelse for et vedtatt flertallsforslag.
6. Som kildekontrollør vil jeg kunne gå fra en eksportert tekst til dokumentversjon, side eller anker og bevart original, slik at jeg kan kontrollere innhold og sammenheng.
7. Som kildekontrollør vil jeg se overskrifter, tilgrensende tekst og kildehierarki, slik at et avsnitt om flere poster ikke feilaktig fremstår som en forklaring på bare én post.
8. Som budsjettanalytiker vil jeg kunne knytte flere passasjer til samme hendelse og én passasje til flere poster, slik at kildebildet bevares uten kopierte beløpshendelser.
9. Som kildekontrollør vil jeg beholde relevant omtale selv om ingen sikker post- eller hendelseskobling er funnet, slik at uavklarte passasjer kan undersøkes senere.
10. Som budsjettanalytiker vil jeg se kildeutsagn, faglig tolkning, hypotese og ukjent grunnlag hver for seg, slik at en foreslått sammenheng ikke blir et kildefaktum.
11. Som budsjettanalytiker vil jeg se manglende, feilet eller foreldet omtalegrunnlag, slik at en tom visning ikke tolkes som fravær av begrunnelse eller endring.
12. Som ansvarlig for innlesningen vil jeg fortsatt registrere nye offisielle vedtak når omtale- eller historikkilder mangler, slik at ny vedtaksinnlesning er uavhengig av senere analyseberikelse.
13. Som bruker av tidligere uttrekk vil jeg kunne gjenlese gamle ID-er, observasjoner, vurderinger og frosset JSON med opprinnelig betydning, slik at en ny omtaleleveranse ikke omskriver tidligere resultater.
14. Som budsjettanalytiker vil jeg få en avgrenset årslinje med uttrykkelig kilde- og behandlingsdekning, slik at opprinnelig budsjett, RNB, nysaldering og øvrige vedtak ikke skjules bak en antatt komplett saldo.
15. Som budsjettanalytiker vil jeg se dokumenterte kontoflyttinger og gyldighet på tvers av år, slik at like kapittel- og postnumre ikke automatisk behandles som samme konto.
16. Som budsjettanalytiker vil jeg søke etter temaer på tvers av år og få henvisning til hvert relevant tekstbelegg, slik at jeg kan kontrollere hvilke endringer et svar bygger på.
17. Som budsjettanalytiker vil jeg få skilt tematisk omtale fra dokumentert begrunnelse for en endring, slik at et svar på «skyldtes tema X» kan vise usikkerhet og manglende bevis.
18. Som faglig kontrollør vil jeg se modell, modellversjon, promptversjon, kilde-ID-er, belegg og vurderingsstatus for KI-tagger og sammendrag, slik at genererte fortolkninger kan vurderes og erstattes.
19. Som budsjettanalytiker vil jeg se når samme hendelse inngår i flere temaer, slik at overlappende treff eller flere forklarende avsnitt ikke øker antallet endringer eller summen av beløp.
20. Som bruker av datagrunnlaget vil jeg kunne gjenlese den faktiske JSON- og Excel-eksporten med samme kilder, relasjoner og status, slik at analysen kan etterprøves uten den opprinnelige visningen eller en bestemt søketjeneste.

## Implementeringsbeslutninger

Dette er beslutninger om mål og rammer. O2a/O2b følger sin godkjente avgrensede oppdeling i #34/#35. Konkrete adaptere, kontraktutvidelser og tickets utover piloten krever eget kildegrunnlag og mandat.

- Offisielle originalkilder er primærgrunnlaget: regjeringens proposisjon, komiteens innstilling og det endelige vedtaket har separate dokumentidentiteter og versjoner. Samme dokument som finnes i flere formater skal ha sporbare representasjonsrelasjoner, ikke antas byteidentisk.
- Faktisk mottatte originalbyte bevares med kilde-URL, innhentingsmetadata og hash. Manglende respons gir ingen oppfunnet hash. HTML-struktur eller PDF og sidetall må kunne gjenfinnes; en normalisert tekst er avledet materiale, ikke erstatning for originalen.
- En omtaleseksjon får egen identitet bundet til eksakt dokumentversjon, nøyaktig lokator, originaltekst og struktur. Overskriftshierarki, side-/ankerhenvisning og nødvendig omkringliggende kontekst bevares. Tekstuttrekkets versjon skal skilles fra kilderevisjonen.
- Relasjoner til budsjettår, kapittel, post, beløpsobservasjon og dokumentert hendelse er uttrykkelige og mange-til-mange. Hver relasjon har eget kildebevis, rolle og avklaringsstatus. En felles sak, dokumenthenvisning, lik konto eller et likt beløp er ikke tilstrekkelig hendelsesbevis.
- Omtale kan finnes uten beløpsobservasjon eller sikker postkobling. Et felles avsnitt om flere poster bevarer sitt omfang; systemet skal ikke fordele en felles begrunnelse eller et felles beløp vilkårlig.
- Regjering, komité, komitéflertall, navngitte partier/mindretall og vedtatt flertall må holdes adskilt der kilden gir grunnlag. Koblingen fra forslag eller merknad til vedtatt resultat må dokumenteres separat. Fravær av innsigelse beviser ikke at alle begrunnelser er vedtatt.
- Kildeutsagn, faglig tolkning og hypotese har separate belegg og statuser. Ukjent rolle, manglende tekst, uavklart kobling, kildefeil og faktisk kontrollert fravær skal ikke slås sammen. En faglig kontrollavgjørelse er fortsatt separat fra teknisk strukturering.
- Forslagsbeløp, før-/etterbeløp og omtale er ikke ekstra vedtatte endringer. Relasjoner, tekstutdrag og temaer må ikke multiplisere eller dobbeltelle en beløpshendelse. Behandlingens faktiske rekkefølge og talltype skal dokumenteres før en årsrekke eller sammenligning godkjennes.
- Søk på tvers av år krever kontokoblinger med gyldighet, kilde og kjent omfang. Endret oppgavefordeling, omnummerering, deling og sammenslåing skal kunne vises. En join på bare kapittel/post over år er utilstrekkelig; ukjent kontinuitet skal forbli ukjent.
- KI-tagger og sammendrag lagres som separate avledede vurderinger med modellidentitet/-versjon, promptversjon, benyttede kilde-/seksjons-ID-er, evidens og vurderingsstatus. En generert tekst erstatter ikke originalen og blir ikke automatisk faglig godkjent. Ny kilde eller ny modell skal ikke omskrive tidligere resultater.
- Et tema som nevnes i metadata eller omtale gir et relevanstreff. Påstanden om at temaet forklarer en konkret endring krever tekstbelegg og en dokumentert kobling til behandlingsleddet. Temasummer må vise overlapp, hvilke hendelser som inngår og grunnlaget for beløpsutvalget.
- Strukturert bevaring og maskinlesbar eksport prioriteres først. En senere søkeindeks kan bygges på dette og erstattes. Ingen bestemt vektordatabase, skytjeneste, embeddingmodell eller språkmodell er valgt eller nødvendig for å begynne.
- Innlesning eier kildehenting, originalbevaring, versjoner og sporbar strukturering; analyse eier eksplisitte utvalg, søk, sammenstilling og fremstilling. Nye adaptere skal være adskilt fra eksisterende vedtaksinnlesning.
- Feilet eller fraværende omtale må aldri blokkere oppdagelse, lagring eller eksport av nye offisielle vedtak. Historisk Excel, historisk register og historisk startsaldo er heller ingen inngangsavhengighet.
- En senere implementering skal være additiv og eksplisitt versjonert. Tidligere ID-er, råbyte, parser-/tolkningsbetydning, faglige kontrollavgjørelser, lagrede resultater, frosset JSON og eksisterende standardvalg bevares. Konkret kompatibilitets- og versjonsforslag skal inngå i byggeticketen før endring.

## Testbeslutninger

Prosjekteieren bekreftet 22. oktober 2026 én samlet, høy testgrense: **bevart original → omtaleseksjon med kildepeker → dokumentert relasjon til vedtak/hendelse og kapittel/post → faktisk gjenlest strukturert eksport**. Dette er ikke bare en test av interne seksjonsobjekter eller av at en fil finnes. Testgrensen brukes nå i #34/O2a; den opprinnelige planendringen innførte ingen funksjonstester.

- Bruk den eksisterende vertikale kilde–lagring–eksport-grensen som forbilde, med autentiske lagrede kildeprøver i deterministisk CI og separat live kildekontroll. B8/B9 har allerede prøvd frosset JSON og faktisk gjenlest Excel; nye kontroller skal utvide observerbar atferd på samme nivå.
- Prøv både kildebevaring/strukturering i innlesningen og relasjon/utvalg/eksport i analysen gjennom den samlede grensen. Kontroller hele veien at eksportert tekst peker til rett original, dokumentversjon og lokator, med samme rolle og status etter gjenlesing.
- O1s bevarte autentiske passasjer og kildebevis for vedtak 210 (2024–2025), kap. 1429 post 1 og 22, er pilotens kontrollgrunnlag. Nye prøvesaker krever tilsvarende kildekontroll før de blir testfasit. En forklaring som ikke finnes, gir dokumentert manglende eller uavklart grunnlag.
- O2 skal demonstrere hele testgrensen for den avgrensede 210-piloten, inkludert originaler, overskriftshierarki, relasjonsbevis, faktisk JSON- og Excel-gjenlesing og uendret antall beløpshendelser.
- Senere autentiske prøver skal dekke en kildebelagt komitéendring med flertalls-/mindretallsroller, omtale om flere poster og en passasje uten sikker hendelseskobling. Kildene velges etter faktisk kildeundersøkelse.
- Merk syntetiske prøver tydelig. De skal blant annet dekke feil dokumentversjon/lokator, endret tekst, gjentatt lesing, kilderettelse, manglende/feilet kilde, ukjent rolle, feilaktig postkobling, mange-til-mange-relasjoner og kontoflytting med ukjent kontinuitet.
- Kontroller at ny offisiell vedtaksinnlesning fortsatt fungerer med fraværende, korrupt eller motstridende omtale og historisk grunnlag. Globale avvik skal være synlige også når et filter gir null beløpsrader.
- Regresjonskontroller skal gjenlese gamle JSON-/Excel-resultater og stabile identiteter uten omskriving. Ny omtale eller indeks skal ikke gi nye beløpshendelser, endre tidligere faglig kontroll eller automatisk aktivere en historisk tolkning.
- Årslinjen skal prøves mot et uttrykkelig kildeinventar og et avgrenset avstemmingsomfang. En lokal før + endring = etter-kontroll beviser ikke årsdekning. Opprinnelig budsjett, RNB, nysaldering og øvrige endringer må enten være dokumentert dekket eller ha synlige hull.
- Temasøk skal kontrolleres mot kildebelagte relevante og irrelevante passasjer. Et godt resultat bevarer tekstbelegg, avsender, relasjon og usikkerhet, skiller relevans fra årsaksforklaring og viser at overlapp ikke blåser opp antall hendelser eller beløp.

## Avgrensning

- Den opprinnelige planleveransen endret dokumentasjon og spesifikasjon. Senere #34/O2a har eget godkjent mandat og en avgrenset kilde-/eksportadapter; øvrige funksjoner følger fortsatt egne porter.
- Behov og testgrense er bekreftet. O1 er godkjent; #34/O2a er levert for sitt post 1-snitt, og #35/O2b har eget mandat for begge postene. O3–O5 og de to generelle visningene har ikke samlet byggemandat. Et `ready-for-agent`-merke gjelder bare spesifikasjonens beskrevne mandat.
- Videre arbeid følger den konkrete ticketen og dens faktiske kildegrunnlag. Oppfølgingen for de to generelle inngangene er en [egen konkretisering](to-visninger.md#modellkonsekvenser-og-leveransegrense), ikke en utvidelse av pilotens aksept eller forhåndsbestilling av byggetickets.
- Ingen automatisk faglig godkjenning, komplett årsdekning eller automatisk årsaksbestemmelse loves. Historiske kolonneregler, presisjonsregler og kjedekonflikter løses ikke av en tekstkobling.
- Ingen full import av alle tidligere år, retting av hele den historiske kjeden eller produksjonsdrift følger med. #13s historikkrest og #10s faktiske driftsaksept er egne spor; ingen av dem må lukkes for å undersøke omtale eller registrere nye offisielle vedtak.
- Omtale om fullmakter kan bevares, men blir ikke dermed en bevilgningsendring. Den separate fullmakten i vedtak 211 er fortsatt ikke en ekstra beløpshendelse.

## Videre merknader

### Anbefalt rekkefølge og porter

Hver senere byggeticket skal levere et lite, komplett og kontrollerbart snitt. Faser skal deles videre dersom et slikt snitt ikke passer i én fersk agentkontekst. Oppdeling i bare lager, parser og visning oppfyller ikke dette. Foreslåtte tickets og reelle blokkeringer skal vises samlet før publisering, etter [arbeidsflyten](arbeidsflyt.md).

| Fase | Resultat og akseptport | Status | Mandat og videre avhengighet |
| --- | --- | --- | --- |
| O1 – Kildeundersøkelse og avgrenset spesifikasjon | Bevarte Prop. 16 S-/Innst. 81 S-passasjer og plenumsbevis dokumenterer 210/1429/1 og 22, med originaler, lokatorer, roller og grenser. | Utført og godkjent som kildegrunnlag 22. oktober; følger O2a-kandidaten. | [O1s opprinnelige O2-forslag](https://github.com/depmartin/budsjetthistorikk/blob/417e4fdeb22c8c510a56d038686cbf5ffa740cd2/docs/research/omtale-o1/o2-forslag.md) er siden godkjent og publisert som #34/#35. |
| O2a / #34 – post 1 | Komplett opt-in-snitt for 210/1429/1 fra originalomtale og dokumentert relasjon til faktisk gjenlest JSON og Excel. | Levert i [PR #36](https://github.com/depmartin/budsjetthistorikk/pull/36), main `6f7145d`, 23. oktober. | Det leverte A-resultatet bevares uendret. Pilotgrensen står i [målbildet](to-visninger.md#modellkonsekvenser-og-leveransegrense). |
| O2b / #35 – begge poster | Piloten omfatter post 22 og felles omdisponeringsomtale, fortsatt to posthendelser og seks vedtaksbeløpsobservasjoner. | Levert i [PR #39](https://github.com/depmartin/budsjetthistorikk/pull/39), main `5423160`. | Ingen generell dokument-/årsvisning. Gamle A- og nye B-resultater bevares. |
| O3 – Komitéendring og mer sammensatt kildebilde | Demonstrer korrekt avsender/flertall/mindretall, kobling til vedtatt resultat og mange-til-mange-omtale uten dobbelttelling. | [315/78 er kildekontrollert](research/to-visninger-37/komiteendring.md); T2 under #37 foreslår et snitt. Positivt tallfestet alternativ står åpent som K1. | Byggemandat gjenstår. Ingen motstemme omtolkes til et alternativt beløp. |
| O4 – Avgrenset årslinje for konto | Vis opprinnelig budsjett, RNB, nysaldering og øvrige relevante vedtak, riktig talltype/behandlingsrekkefølge, omtale og synlig kilde-/beregningsdekning. Manglende ledd er hull, ikke null. | [1429/1 og /22 i avgrensede 2024/2025-utvalg er kildekontrollert](research/to-visninger-37/konto-aar.md); T3/T4 foreslår separate snitt. Full årsdekning og positiv kontinuitet er åpne K3/K2. | Eget mandat. Den konkrete T3-avhengigheten er T1, ikke hele O3; #13s fulle historikk er ikke forutsetning. |
| O5 – Temasøk på tvers av år | Søk i et eksplisitt kilde-/årsutvalg. Returner konkrete passasjer med avsender, kontokontinuitet, evidens, status og skille mellom tematisk relevans og begrunnelse for endringen. Eventuelle antall/summer dokumenterer hendelsesutvalg og overlapp. | Foreslått; ingen modell, indeks eller årsdekning er valgt. | Bygger på kildeforankret struktur og dokumenterte kontokoblinger fra tidligere faser. Konkret søkesnitt, teknologivalg og byggemandat gjenstår. |

O3–O5 skal ikke arve en antatt faglig godkjenning fra piloten. 210 gir den avgrensede O2-kjeden, men ingen faktisk komitéendring. Den videre [kildeundersøkelsen under #37](research/to-visninger-37/README.md) har nå konkrete kilder for T2–T6, med synlige grenser og åpne K1–K3. [Ticketutkastene](research/to-visninger-37/tickets/README.md) viser faktiske avhengigheter; de er ikke et nytt byggemandat. Kravene står fortsatt samlet i [målbildet](to-visninger.md).

### Start i en ny økt

Les hele den aktuelle ticketen og kommentarene, [AGENTS.md](../AGENTS.md) og dokumentene ticketen peker til. Kontroller gjeldende status for #32/#34/#35/#37 og PR #36/#39. Bruk O1 som bevart kildegrunnlag; den opprinnelige O1-startprompten er erstattet av godkjent oppdeling. Arbeid med dokumentvisning, stadiesammenligning eller konto-/årsvisning skal starte i [det autoritative målbildet](to-visninger.md) og [#37-forslaget](visningspilot-plan.md), med konkretiseringens kilde- og mandatgrense.

### O2b er levert; neste forslag er #37

O2b er flettet i PR #39. B velges eksplisitt med `o2b-html-pdf-1`; gamle A-filer beholder betydningen. [#37-forslaget](visningspilot-plan.md) anbefaler T1 først og legger alle utkast frem før publisering/bygging. Et senere gjennomføringsmandat skal angi ticket; ticket-orchestrator håndterer da samlet review, separat sikkerhetsaudit, PR, CI og autorisert merge. #10 står fortsatt åpen.
