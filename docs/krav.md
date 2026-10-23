# Krav og åpne beslutninger

## Formål og brukere

Finansavdelingen i Finansdepartementet skal kunne analysere og hente ut historiske budsjettforslag og budsjettvedtak. Hvert beløp skal kunne spores til kilde, dokument og behandlingsledd.

## To innganger til samme kildegrunnlag

Prosjekteieren bekreftet 23. oktober 2026 både dokumentvisning og konto-/årsvisning som produktkrav. [Det autoritative målbildet](to-visninger.md) samler omfang, stadiesammenligning, dokumentgraf, beløpsbetydning, dekning, eksportaksept og pilotgrense; [#37](https://github.com/depmartin/budsjetthistorikk/issues/37) gjelder konkretiseringen. Dette presiserer ønsket resultat; de generelle visningene er ikke implementert av O2a/O2b og har ikke samlet byggemandat.

## Første leveranse

- Les inn og bevar endelige stortingsvedtak fra Stortingets kilder. Bevilgningsvedtak gir strukturerte opplysninger om budsjettår, kapittel, post, beløp og kilde.
- Start med sesjonen 2026–2027. Ta med endringer for inneværende budsjettår og vedtak for neste budsjettår. Viderefør innlesningen til nye sesjoner.
- Ta med alle bevilgningsendringer: opprinnelig budsjett, RNB, nysaldering og øvrige vedtak, også uten regjeringsproposisjon.
- Rene lovforslag kan utelates. Bevilgningsendringer i sammensatte lov- og budsjettsaker skal med.
- Oppdag nye og endrede vedtak daglig. Planlagt tidspunkt er kl. 06.00 i Europe/Oslo, med riktig håndtering av sommer- og vintertid.
- Gi en kjørerapport som skiller ingen nye vedtak, innlesningsfeil og uttrekk som krever kontroll.
- Lagre data og lever et kontrollerbart Excel-uttrekk. Interaktivt analysegrensesnitt kommer senere.
- Bevar fullmakter, stikkord og øvrige tekstvedtak med original struktur og kilde. Full detaljstrukturering av fullmaktsrammer er valgfri og skal ikke forsinke bevilgningsinnlesningen.
- Bevar underposter og kildehierarki der de forekommer. Posttotal og underliggende spesifikasjon skal ikke dobbeltelles.

## Historikk og beløp

Prosjekteieren bestilte 20. oktober 2026 presisering av det felles formatet før #6. [Observasjonsformat versjon 1](observasjonsformat.md) og [ADR 0003](adr/0003-felles-belopsobservasjoner.md) fastsetter separate beløpsobservasjoner, dokumentrelasjoner og beregnede verdier, med kompatible kildeadaptere for Excel og Stortinget. Dette er et modellgrunnlag for de eksisterende leveransene; historisk import, forslag, regnskap og omtale er fortsatt egne leveranser. Ingen historisk enhet eller kolonnetolkning er godkjent generelt.

Hvert opprinnelige vedtak og hver senere vedtatte endring skal kunne følges separat på kapittel og post. Bevar endringsbeløp og eventuelle fra-/til-beløp som kilden gir, og skill disse fra beregnet gjeldende bevilgning.

Forslag, vedtak og regnskap er forskjellige talltyper. RNB og nysaldering er behandlingsrunder som kan omfatte flere dokumenter og vedtak. Oppsummeringer av tidligere vedtak skal ikke leses som nye bevilgningsendringer.

Rettelser i en kilde er versjoner av kildeopplysningen. De skal kunne skilles fra et nytt stortingsvedtak om å endre bevilgningen.

Manglende inngående bevilgning skal gi ufullstendig beregningsgrunnlag, ikke et oppdiktet nullbeløp.

## Kontoplan og departementer

Både utgifter og inntekter inngår. Klassifikasjon følger kapittelnummer, ikke beløpets fortegn. Innenfor budsjettkapitlene er 1–2999 utgifter og 3000–5999 inntekter, jf. vedlagt R-101/2024 side 3. Kapitalregnskapets konti 6000–9999 skal holdes utenfor kapittelklassifikasjonen for bevilgningsvedtak.

Departementsnummer, navn, forkortelse og kapitteltilknytning skal kunne vedlikeholdes manuelt. Opplysninger skal ha gyldighetsperiode og kilde. Brukerens departementsoppsett og 2027-filen er utgangspunkt; eldre veiledere skal ikke overstyre nyere opplysninger.

Departementsnummer 10 og 12 er ledige i brukerens oppsett. Særkapitler og inntektskapitler krever eksplisitte oppslag. Hundretallsserier og +3000 er hjelperegler, ikke uttømmende departementskoblinger. Detaljer finnes i [departementsregisteret](departementsregister.md).

## Datakvalitet

Tvetydige uttrekk skal bevares med originalkilden og sendes til manuell kontroll. De skal holdes utenfor godkjente analysetall til de er avklart. Kjøring og uttrekk skal vise uavklarte opplysninger og manglende dekning.

Negative bevilgningsbeløp kan være gyldige, blant annet ved netto driftsresultat. Post 90–99 og særserier skal inngå i dekningskontrollen.

En ny post eller et nytt kapittel skal bevares selv om det mangler i 2027-katalogen. Uavklart departementstilknytning skal synliggjøres og ikke medføre at vedtaket forsvinner.

## Senere kilder og analyse

På sikt skal en post kunne følges gjennom regjeringens opprinnelige forslag, eventuelle tilleggsforslag, stortingsforhandlinger og innstilling, opprinnelig vedtak, alle senere endringer, RNB, nysaldering og regnskap.

Regjeringsforslag, komitéforslag, kapittel- og postomtale og regnskap inngår som egne kildeintegrasjoner. Regnskapstall skal ikke summeres inn som bevilgningsendringer. Overførte midler, fullmaktsrammer og eventuelle overskridelsessamtykker skal også kunne skilles fra årets vedtatte bevilgning.

Kontoutvalg skal støtte departement, kapittel, post og kombinasjoner av disse. Dokument- og konto-/årsvisningens felles sammenlignings- og dekningskrav står i [målbildet](to-visninger.md).

Vedlagt Gul bok-fil gir en strukturert kilde til regjeringsforslaget og kapittel-/postmetadata. Katalogbruk kan forberedes uten uthenting fra regjeringen.no. Forslagsbeløp skal ha egen kildetype og skal aldri registreres som vedtak. Automatisk uthenting av regjeringsforslag skal ikke blokkere første leveranse. Brukeren har også eldre historiske data for senere import.

## Fullstendighet og kontroll

Målet er uttømmende dekning av bevilgningsendringer. Kontrollen må skille mellom funnet kildeinnhold, strukturerte opplysninger og godkjente analysetall. Uavklarte linjer er avvik som skal være synlige; de gir ikke grunnlag for å påstå fullstendig strukturering.

Kildeinventar og uavhengige kontrollsummer skal brukes sammen. Blå bok kan være et kontrollgrunnlag for opprinnelige vedtak; senere oppsummeringer og statsregnskapets bevilgningskolonner er mulige kontrollkilder som må prøves i kildeundersøkelsen. Regnskapets utfallsbeløp er ikke fasit for vedtatt bevilgning.

## Drift og mottakersystem

Python, SQLite og openpyxl er godkjent for lokal innlesning og Excel-uttrekk, og byggemandat er gitt for B1 (#4) 20. oktober 2026. Valget er dokumentert i [ADR 0001](adr/0001-lokal-innlesning.md). Eieren valgte 21. oktober 2026 en varig Windows-vert med lokal lagring for B7. Vert, driftskonto, datamappe og eksisterende bakgrunnstilgang er utsatt etter eierens beskjed «Dette vet jeg ikke, så det må vi komme tilbake til». Kodeleveransen omfatter runner og reviewbart Windows-oppsett; faktisk installasjon/driftsprøve gjenstår, og #10 forblir åpen. Ingen skyressurser eller credentials er opprettet. Se [driftsveiledningen](b7-drift.md).

## Manuelt vedlikehold og varsling

Første leveranse bruker Excel-/CSV-filer til vedlikehold av departements-/kapittelregisteret og behandling av uavklarte uttrekk. Endringer kobles til stabile identifikatorer og bevarer originalkilde, gyldighetsperiode og begrunnelse. Kilderevisjoner må gjøre utdaterte korreksjoner synlige før de brukes videre.

Ved innlesningsfeil eller uttrekk som krever kontroll opprettes en GitHub-issue. Gjentakelser av samme forhold oppdaterer samme issue. Vellykkede kjøringer uten slike avvik gir bare kjørerapport. GitHubs vanlige abonnementer styrer hvem som mottar varsler; løsningen skal ikke love en bestemt e-postlevering.

## Gjenstående bekreftelser

Samlet spesifikasjon, testgrenser og ticketoppdeling er godkjent av prosjekteieren 20. oktober 2026. Byggetickets er publisert som #4–#10. Kildeundersøkelsen #2 er levert i PR #11. Teknologiforslaget og byggemandatet for det smale B1-snittet er godkjent med «Gjør som du foreslår».

Gjenstående tekniske avklaringer:
- Konkret kilde- og fullstendighetskontroll etter kildeprøvene.
- Konkret Windows-vert, driftskonto, lokal lagrings-/rapportbane, eksisterende bakgrunnstilgang og faktisk driftsaksept. Endelig mottakersystem for felles bruk er fortsatt åpent.

Tekniske fakta undersøkes av agenten. Brukeren avgjør behov, prioriteringer og faglig aksept.

## Presisering 21. oktober 2026: nye kilder og historisk pilot

Oppfølging 22. oktober: P13-P1/#24 er levert med separat [2024-adapter og kontrollpakke](historisk-pilot.md), [fullt prøvd lokalt](research/historisk-excel/pilot2024.md). P13-P2/#26 er levert med [kildebelagt kontrollmatrise](research/historisk-excel/p13-p2/README.md), uten aktivering av normalisering, faglig godkjenning eller årsdekning. Åpne faglige kolonne-/register-/hierarkispørsmål og historiske kjedekonflikter består; #13 gjelder fortsatt resten, og #10s driftsaksept gjenstår. Planbestillingens tidligere mandatgrense nedenfor er historisk kontekst.

Nye offisielle tall skal kunne oppdages, bevares, tolkes, lagres og eksporteres fra sin egen nye offisielle kilde uten historiske Excel-filer, eldre beløp, Excel-startsaldo, historisk register eller en vellykket historisk import. Manglende historisk inngående grunnlag skal gi et synlig analyseavvik når en beregning trenger dette, og skal ikke blokkere innlesning av det nye vedtaket eller gi en oppdiktet nullstart. Dette skal ha en uttrykkelig regresjonsprøve, også ved fraværende, korrupt eller motstridende historisk kilde.

Den historiske modellen skal bevare kilden og betydningen uten å gjøre arbeidsbøkenes kolonner eller dagens API-form styrende for nye kilder. Et bedre felles format kan foreslås og versjoneres ved dokumentert behov, med uttrykkelig kompatibilitetsbeskrivelse. Dagens besluttede observasjonsformat, leverte API-er, ID-er og standardvalg gjelder frem til en slik utvidelse er besluttet. Eksisterende parser-, format- og skjemaidentiteter skal beholde sin betydning. Ingen migrering eller kodebygging følger av bestillingen om en plan.

[Pilotplanen under #13](pilotplan-historisk-excel.md) anbefalte 2024 som én lokal leveranse fra original til historiske observasjoner, lagring, Excel/avviksrapport og uavhengig sammenligning. Årsvalget støttes av den [utførte, avgrensede Excel-/Storting-prøven](research/historisk-excel/pilotkontroll.md). Filadapter og pilotimport er siden levert som P1, og avgrenset kildekontroll som P2. Full årsavstemming og generelt godkjent historisk analysegrunnlag gjenstår. Uavklarte enheter, kolonnefortolkninger og organisasjonskoblinger begrenser faglig bruk av berørte verdier, uten å hindre råbevaring og kontrolluttrekk. Den tidligere åpne byggemandatgrensen for piloten er historisk; nye utvidelser trenger eget mandat. Utsatt driftsaksept i #10 er fortsatt åpen.

## Godkjent saksberikelse og stikkord – 22. oktober 2026

Eieren bestilte #28/B8 med kildekontroll, implementering, samlet review, separat sikkerhetsaudit, CI og merge. Saksdokumentenes metadata skal hentes fra Stortingets saks-API og versjoneres separat fra tidligere vedtaks-/beløpsobservasjoner. Formelt vedtaksnummer med sesjon, teknisk API-ID og klikkbare innstillings-/proposisjonsnumre vises ved beløp i Excel og frosset JSON med eksplisitt ny versjon. Saksrelasjoner er ingen bevist postvis forslagstilknytning. Dokumentfulltekst og forslagsbeløp er utenfor omfanget.

Eieren presiserte samme dag at «Stikkord» skal være en egen synlig kolonne. 1429/22 i vedtak 210 skal vise «kan overføres», med bevart råtekst og kildepeker. Ingen stikkord funnet og uavklart tolkning er ulike utfall. Stikkordsvisningen er separat berikelse, uten endring av gamle observasjoner eller ekstra beløpshendelse. Vedtak 211s fullmakt skal fortsatt ikke bli bevilgningsbeløp.

Tidligere ID-er, råbyte, B5-avgjørelser, v1/v2-tolkninger og B7s standardvalg bevares. Manglende eller feilet saksgrunnlag skal synes uten å stoppe nye vedtak eller beløpseksport. Globale dokumentavvik bevares før filtre. Historisk Excel/register/start er ingen avhengighet. [B8-veiledningen](b8-saksdokumenter.md) beskriver den nye opt-in-grensen; orkestratorens review, sikkerhetsaudit, CI og merge er egne leveringsporter. #10s faktiske driftsaksept er fortsatt utsatt, og #1/#10/#13 holdes åpne for sine rester.

## Godkjent hovedvisning for historikk – 22. oktober 2026

Eieren bestilte #30/B9: Historikk skal være første aktive ark i B8-uttrekket, med nøyaktig 13 synlige kolonner i denne rekkefølgen: Kapittelnummer, Postnummer, Kapittelnavn, Postnavn, Stikkord, Dato, Vedtaksnummer, Innstillingsnummer, Proposisjon, Beløp før vedtak, Vedtatt endring, Beløp etter vedtak og Kontrollstatus. Kildenavn skal brukes, med forsiktig skille mellom postnavn, stikkord og handlingsord. Manglende eller motstridende grunnlag skal synes. Før/etter er kildeobserverte beløp, ingen konstruert null eller kjedesaldo.

Tidligere detaljkolonner og full sporbarhet beholdes i en egen synlig reservefane. Flere dokumenter beholder alle henvisninger og klikkbare lenker uten flere beløpsrader eller hovedkolonner. Kontrollstatus skal også synliggjøre globale avvik før filtre, ferskhet og faglige begrensninger. En tom beløpsvisning skjuler ikke disse. Se [B9-veiledningen](b9-historikk.md) og [kontrollrapporten](research/b9/README.md). Eksisterende frosset JSON, ID-er, kilder, B1–B7 og uavhengig ny offisiell registrering bevares. Nytt konkret 210-uttrekk produseres etter review, CI og merge, med eget navn. #10 holdes åpen.

## Bekreftet behov og testgrense for omtale – 22. oktober 2026

B8/#28 og B9/#30 er levert; B9s 13-kolonners hovedvisning er flettet i [PR #31](https://github.com/depmartin/budsjetthistorikk/pull/31). Saksmetadata og dokumentlenker gir fortsatt ingen bevist postvis forklaring. Proposisjons- og innstillingsfulltekst er egne, fremtidige kildeleveranser.

Brukeren skal kunne velge kapittel/post, følge endringer gjennom et budsjettår og hente frem konkret kapittel- og postomtale fra proposisjon og innstilling som forklarer forslag og behandling. På tvers av år skal brukeren kunne undersøke hvilke bevilgningsendringer som skyldtes et tema, med tekstbelegg og uttrykkelig skille mellom relevanstreff, kildeutsagn, tolkning og dokumentert begrunnelse. Kontinuitet ved omnummerering og omorganisering må ha kilde og gyldighet; likt kapittel/post er ikke automatisk samme konto over år.

Originaldokumenter og dokumentversjoner skal bevares. Omtaleseksjoner skal ha stabil identitet innen kildegrunnlaget, presis HTML-/PDF-lokator, hierarki og kontekst. Flere passasjer kan belyse samme hendelse, og én passasje kan gjelde flere poster; uavklart omtale skal også beholdes. Forslag og omtale skal ikke gi ekstra vedtatte beløpshendelser. Regjeringens, komitéflertallets og mindretallets utsagn må skilles, og et mindretalls argument kan ikke tilskrives vedtatt flertall uten bevis. KI-tagger og sammendrag skal være separate avledede vurderinger med modell-/promptversjon, kilde-ID-er, belegg og vurderingsstatus.

Prosjekteieren har bekreftet den samlede testgrensen: **bevart original → omtaleseksjon med kildepeker → dokumentert vedtaks-/hendelses- og kapittel/post-relasjon → faktisk gjenlest strukturert eksport**. JSON og Excel skal kunne etterprøves med uendrede kilder, relasjoner og statuser. Ny omtale må bygges additivt og versjonert uten å omskrive gamle ID-er, kontrollavgjørelser eller frosset JSON. Feilet/fraværende omtale og historiske filer må aldri blokkere nye offisielle vedtak.

[Omtaleplanen](omtale-plan.md) samler spesifikasjon, akseptporter og gjennomføringsrekkefølge. O1s faktiske kildebevis er kontrollert og godkjent. Prosjekteieren godkjente 22. oktober 2026 O2-oppdelingen som #34/O2a og #35/O2b, separat omtalegrunnlag og eksplisitt `omtale-pilot-1`. #34 er levert i PR #36 (main `6f7145d`), #35 i PR #39 (main `5423160`), med [kontrollgrunnlag](research/omtale-o2b/README.md). [O2a-kontrakten](omtale-pilot.md) fastsetter felter, ID-er, teknisk kontroll og uavhengig ny vedtaksinnlesning før produktkode. O2b omfatter begge 210-postene. [Forslaget under #37](visningspilot-plan.md) konkretiserer de to inngangene med kilder, testmatrise og ticketutkast; det er ikke nytt byggemandat. Senere komitéendring, årslinje og søk krever egne mandat. Ingen ny faglig godkjenning følger av piloten.

[Presiseringen 23. oktober](to-visninger.md#modellkonsekvenser-og-leveransegrense) avgrenser pilotene mot de to generelle visningene og angir neste konkretisering. Ingen vektordatabase, sky, modell eller automatisering er valgt. #10 forblir åpen for driftsaksept; #13s resterende historikkarbeid er uavhengig.
