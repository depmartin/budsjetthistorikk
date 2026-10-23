# Leveranseplan

Oppdatert 23. oktober 2026. Den opprinnelige første leveransen og dens godkjente oppdeling er bevart nedenfor. B8/B9 er levert; O1-kildegrunnlaget og O2-oppdelingen er godkjent under [omtalesporet](omtale-plan.md). [Dokumentvisning og konto-/årsvisning](to-visninger.md) samler eierens nye bekreftede mål og aksept. Godkjente mål, pilotens byggemandat og faktisk levert funksjon skal skilles.

Spesifikasjonen, testgrensene og oppdelingen ble godkjent av prosjekteieren 20. oktober 2026. Byggetickets er publisert som #4–#10. Kildeundersøkelsen #2 er levert i PR #11 med [akseptmatrise og byggegrense](research/issue-2/byggestart.md). De tre historiske kildekonfliktene gir ikke godkjent additiv historikk, men er avgrenset og har eksplisitte kontrollkrav. Python, SQLite og openpyxl og byggemandatet for B1 (#4) er godkjent. B1 har et implementert vertikalt snitt for ett opprinnelig vedtak; videre oppstart følger ticketenes avhengigheter og mandat. Se [arbeidsflyten](arbeidsflyt.md).

## Første leveranse

Endelige stortingsvedtak fra sesjonen 2026–2027 skal hentes, bevares, struktureres og lagres. Bevilgningshistorikk leveres som kontrollerbart Excel-uttrekk med kilder og synlige avvik. Daglig kjøring planlegges kl. 06.00 i Europe/Oslo.

Regjeringsforslag, komitéforslag, regnskap, eldre sesjonsimport, avansert fullmaktsstrukturering og interaktivt grensesnitt er senere utvidelser. Vedlagt Gul bok-fil kan gi katalogmetadata, med tydelig skille fra vedtakstall.

## Publiserte leveranser

| ID | Leveranse | Blokkert av | Kontrollerbart resultat |
| --- | --- | --- | --- |
| U1 / #2 | Kildeprøver og kontrollgrunnlag, eksisterende issue #2 | Ingen; oppstart er bestilt | Reproduserbare vedtaksprøver, beløpsenheter og forslag til avstemming |
| B1 / #4 | Ett endelig bevilgningsvedtak fra kilde til lagring og Excel | U1 | Original kilde, alle åtte postlinjer i den valgte prøven og sporbar eksport fungerer samlet |
| B2 / #5 | Nye vedtak og kilderettelser uten dubletter | B1 | Gjentatt og avbrutt kjøring bevarer ID-er, kilderevisjoner og korrekte kjørerapporter |
| B3 / #6 | Følg postens opprinnelige bevilgning og senere endringer | B1 | Endringsvedtak, fra-/til-beløp og beregnet gjeldende bevilgning kan kontrolleres uten dobbeltelling |
| B4 / #7 | Særkapitler, inntekt, nettoresultat og underliggende spesifikasjon | B1 | Representative særtilfeller går fra kilde til korrekt klassifikasjon og Excel, også med negativt beløp og post 90–99 |
| B5 / #8 | Vedlikehold register og behandle uavklarte uttrekk | B1 | Excel-/CSV-endringer og kontrollstatus kan importeres og brukes på nytt med sporbarhet, uten å endre originalkilden |
| B6 / #9 | Samlet sesjonsuttrekk med departementsutvalg og dekningsrapport | B2, B3, B4, B5 | Alle aktuelle vedtak inventeres; eksport viser historikk, kilder og uavklarte/manglende deler, med avstemming |
| B7 / #10 | Daglig kjøring og videreføring over sesjonsskifte | B6 | Kjøring kl. 06.00, tidssone, sesjonsskifte, gjenopptak og GitHub-varsling uten dupliserte feilissues er demonstrert |

Hver byggeticket skal beskrive en smal, komplett funksjon gjennom nødvendige lag. Tabellen er ikke en oppdeling i bare database, parser og grensesnitt. Endelig størrelse vurderes etter U1. En for stor leveranse deles før oppstart.

B1 omfatter bare et representativt første tilfelle. Det ferdige systemet skal håndtere alle aktuelle kildelinjer eller gjøre manglene eksplisitte. Godkjente summer skal ikke skjule uavklarte beløp.

## Aksept for første leveranse

- Endelige vedtak fra sesjonen 2026–2027 kan leses inn, lagres og spores til originalkilden; nye sesjoner kan følges videre.
- Godkjente bevilgningslinjer viser budsjettår, kapittel, post, beløpsbetydning og vedtaksidentitet. Hver opprinnelige bevilgning og senere endring bevares.
- Gjentatt kjøring og kilderettelser fører ikke til dobbeltelling eller tap av kildehistorikk.
- Utgifter, inntekter, særkapitler, nettoresultater og underliggende spesifikasjon klassifiseres og telles korrekt. Fullmaktsrammer og regnskap summeres ikke inn som bevilgning.
- Excel-uttrekk støtter departements-/kapittel-/postutvalg og viser kilder, endringer og synlige mangler. Manglende grunnlag gir ikke en tilsynelatende komplett sum.
- Excel-/CSV-basert registervedlikehold og manuell kontroll kan gjenbrukes med sporbarhet. Utdaterte korreksjoner oppdages når kilden endres.
- Kjørerapport og GitHub-issue viser feil og uavklarte uttrekk. Gjentakelser oppdaterer samme issue; vellykkede kjøringer uten avvik gir ingen nye issues.
- Kjøring kl. 06.00 i Europe/Oslo er demonstrert i avtalt driftsmiljø. Koden alene regnes ikke som produksjonssatt daglig jobb.
- Kildeinventar og uavhengig avstemming dokumenterer dekningsgraden. Åpne avvik skal være synlige; leveransen kan ikke erklæres uttømmende før relevante mangler er avklart.

## Godkjente testgrenser

- Deterministiske faglige tester på lagrede kildeprøver: beløpsenheter, økes/reduseres, fra/til, nettoresultat, underposter og fullmaktsrammer.
- Klassifikasjonstester ved inntektsgrensen og eksplisitte oppslag for særserier. Konti 6000–9999 holdes utenfor bevilgningskapitlene.
- Integrasjonskontroll fra kilde til lagring, ny kjøring, rettelse, kontrollstatus og eksport.
- Live kildekontroll adskilt fra deterministisk CI, slik at en utilgjengelig nettside ikke skjules som feil i fagreglene.
- Excel-uttrekk avstemmes mot godkjente beløpslinjer og viser uavklarte eller ufullstendige beregninger.
- Sesjonsinventar og uavhengige kontrollkilder prøves før fullstendig dekning erklæres.

Disse testgrensene inngår i den godkjente spesifikasjonen. Konkrete kildeprøver og uavhengige kontrollkilder velges i U1 og dokumenteres før byggetickets gjennomføres. Nye produktvalg skal ikke skjules som tekniske testbeslutninger.

## Avklaringer før bygging

Excel-/CSV-filer er bekreftet arbeidsflate for manuelt vedlikehold og kontroll. GitHub-issues er bekreftet varslingskanal ved feil og uavklarte uttrekk. Gjentakelser oppdaterer samme issue; vanlige vellykkede kjøringer gir bare rapport.

Python, SQLite og openpyxl er valgt etter U1 for lokal innlesning og uttrekk, jf. [ADR 0001](adr/0001-lokal-innlesning.md). Eieren valgte 21. oktober 2026 en varig Windows-vert med lokal lagring for B7. Konkret vert, driftskonto, datamappe og eksisterende bakgrunnstilgang er utsatt av eieren. Kode og reviewbart oppsett leveres med [driftsmanual](b7-drift.md) og [deterministisk kontrollrapport](research/b7/README.md); faktisk oppgaveinstallasjon og driftsprøve gjenstår. #10 forblir åpen til dette er akseptert. Ingen produksjonsressurser eller daglig jobb er opprettet. Materielle endringer i omfang, testaksept eller ticketoppdeling legges frem på nytt før videre bygging. Endelig mottakersystem for felles bruk er fortsatt åpent.

## Leverte utvidelser og neste prioritet

| Leveranse | Status ved presisering 23. oktober 2026 | Betydning for neste arbeid |
| --- | --- | --- |
| B8 / #28 – saksdokumenter og stikkord | Levert; se [B8-veiledningen](b8-saksdokumenter.md) og [kildeprøven](research/b8/README.md). | Saksmetadata, dokumentnumre, lenker og stikkord er tilgjengelige. Det er ingen innlest proposisjons-/innstillingstekst eller bevist postvis forslagstilknytning. |
| B9 / #30 – Historikk som hovedvisning | Levert i [PR #31](https://github.com/depmartin/budsjetthistorikk/pull/31); se [B9-veiledningen](b9-historikk.md). | Historikk er første aktive ark med 13 kolonner, og tidligere felt bevares i Historikkdetaljer. Dette er presentasjon av bevart grunnlag, ikke ny årsaksforklaring. |
| O1 – omtalegrunnlag | Utført og godkjent; [kildegrunnlaget](research/omtale-o1/README.md) følger O2a-kandidaten. | Avgrenset 210-kjede er dokumentert. Ingen faktisk komitéendring, full dokumentstrukturering eller årsdekning er bevist. |
| O2a / #34 – 210/1429/1 | Levert i [PR #36](https://github.com/depmartin/budsjetthistorikk/pull/36), main `6f7145d`, 23. oktober. | Godkjent post 1-snitt og egen `omtale-pilot-1`-eksport er bevart etter [kontrakten](omtale-pilot.md). Leveringsportene vurderes mot #34. |
| O2b / #35 – begge 210-postene | Levert i [PR #39](https://github.com/depmartin/budsjetthistorikk/pull/39), main `5423160`; [kontrollgrunnlag](research/omtale-o2b/README.md). | Forblir en pilot med to posthendelser; generell dokument-/årsvisning inngår ikke. |
| To innganger til samme kildegrunnlag | [Autoritativt mål og aksept](to-visninger.md) er bekreftet. Under [#37](https://github.com/depmartin/budsjetthistorikk/issues/37) foreligger [kildebelagt plan, testmatrise og ticketforslag](visningspilot-plan.md) til gjennomgang før publisering og implementering. | Første foreslåtte snitt er hele Innst. 81 S gjennom begge innganger. Videre tabell-/gren-/årsutvalg har egne utkast; positivt alternativ, kontinuitet og full årsdekning har åpne kildeporter. Ingen nytt byggemandat eller implementert generell visning. |
| O3–O5 – komitéendring, årslinje og temasøk | Foreslåtte senere spor i [omtaleplanen](omtale-plan.md#anbefalt-rekkefølge-og-porter). | Egne kildevalg, avgrensninger og byggemandater gjenstår; nye visningskrav gir ikke automatisk mandat til funksjonsbygging. |

Omtaleplanen har pilotens akseptporter og videre rekkefølge. Målbildet for de to inngangene eier deres samlede krav og konkretiseringsgrense. #10s faktiske driftsaksept og #13s resterende historikkarbeid er separate spor. Fravær av historikk eller omtale skal aldri blokkere innlesning av nye offisielle vedtak.

## Planforslag for historisk Excel under #13

Den [opprinnelige pilotplanen](pilotplan-historisk-excel.md) foreslo én lokal byggeticket for hele 2024-arbeidsboken fra uendret original til historiske observasjoner, lagring, kontrollpakke og uavhengig sammenligning. Den [utførte tallprøven](research/historisk-excel/pilotkontroll.md) begrunnet årvalget med konkrete treff og avvik, uten helårsavstemming eller faglig godkjenning. P13-P1/#24 er siden levert med [2024-adapter og kontrollpakke](historisk-pilot.md), og P13-P2/#26 med [kildebelagt kontrollmatrise](research/historisk-excel/p13-p2/README.md). Tidligere omtale av manglende byggemandat gjelder planbestillingens historiske tidspunkt. Videre årganger, åpne faglige kolonne-/register-/hierarkispørsmål, normalisering og historiske kjedekonflikter hører fortsatt til #13. Ingen generell faglig godkjenning eller årsdekning følger av P1/P2. Nye offisielle tall skal kunne registreres uavhengig av historiske filer; #10s utsatte driftsaksept er fortsatt åpen.

## Relasjoner i GitHub

Publiseringsverktøyet støtter ikke skriving av native sub-issue- og avhengighetsrelasjoner. Ticketene har derfor eksplisitte «Del av #1» og «Blokkert av #N» i teksten. Oversikten i #1 samler ticketene. Dette er tekstlige relasjoner, ikke native GitHub-blokkeringer.
