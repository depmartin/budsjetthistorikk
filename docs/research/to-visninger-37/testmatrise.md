# Foreslått testmatrise for #37

**Fremtidig aksept, ikke utførte produkttester.** 23. oktober 2026, mot [planforslaget](../../visningspilot-plan.md) og [V1–V10](../../to-visninger.md). Det som faktisk er kildekontrollert nå står i [forskningsoversikten](README.md) og de fire kildenotatene. Positive porter som mangler autentisk fasit står uttrykkelig åpne. Syntetiske mutasjoner må merkes og kan aldri erstatte positiv autentisk aksept.

## Felles testgrense

Hver T-ticket skal demonstrere **bevart autentisk original → kildebundet beløp og omtale → dokumentert relasjon → dokumentinngang og konto-/årsinngang → skrevne og faktisk gjenleste JSON-/Excel-filer**. Begge innganger må bruke samme versjonerte grunnlag, ikke to manuelt sammensatte fasiter. Sammenlign synlige Excel-celler/lenker og kontrollgrunnlaget med JSON og originale lokatorer; at filen finnes eller internobjektet stemmer, er ikke nok.

Minimumsutvalg i hvert snitt: dokumentvalg, enkeltkonto, flere kontoer, tekst-/fullmaktskonto der det finnes, tomt utvalg og offline-gjenlesing. Globale inventar-/kildeavvik beholdes også i tomt utvalg. Ved T3/T4 prøves både år og dokumentvalg. Nye prøver får egne filnavn; ekte gamle A/B-filer overskrives ikke.

## Eksakt beløpsfasit og telleenheter

Alle tall her er kroner. Før/endring/etter er **tre kildefelt i én posthendelse**, ikke tre hendelser. Forslag, tilråding og vedtak har separate observasjoner/roller; bare siste er vedtatte felt/hendelser. Beløpsutsagn i forklaringstekst og fullmaktsrammer telles separat.

| Snitt | Regjeringsforslag | Tilråding | Vedtak | Avledet sammenligning |
| --- | --- | --- | --- | --- |
| 1429/1, 2024, Prop.16/81/210 | 160 243 000 / +5 796 000 / 166 039 000 | Samme trio | Samme trio | Forslagsdelta→tilrådingsdelta 0; tilråding→vedtak 0, hvis omfang/rollebevis følger med. |
| 1429/22, samme | 32 185 000 / −3 000 000 / 29 185 000 | Samme trio | Samme trio | Tilsvarende 0. |
| 315/78, 2024, Prop.25/85/208 | 29 050 000 / +119 000 000 / 148 050 000 | 29 050 000 / +129 000 000 / 158 050 000 | Samme som tilråding | +10 mill. mellom de kildeobserverte deltaene; 0 til vedtak. Ingen ekstra vedtatt hendelse. |
| 1420/32, 2024, 95/359 | Ingen rad i den kontrollerte Prop.16-tabellen | 812 765 000 / +270 000 000 / 1 082 765 000 | Samme trio | Prop.→95 uavklart/manglende, **ikke** +270 mill. fra null. |

Kilder/lokatorer: [1429 og full Prop.](eksisterende-grunnlag.md), [315/78](komiteendring.md), [95/359](forgrening.md). I første snitt er forventningen /1 alene **9 felt/3 vedtaksfelt/1 vedtatt hendelse**, /22 likt, begge **18/6/2**, tomt **0/0/0**. Fullmakter og globale inventarlinjer består utenfor denne talltellingen.

| Konto-/årsutvalg, bare valgte vedtaksobjekter | Forventning |
| --- | --- |
| 2024, 341/40032928 | 1429/1 nivå 161 243 000; /22 nivå 32 185 000. To valgte posthendelser/to felt. |
| 2024, 857/40033719 | /1 før 161 243 000, delta −1 000 000, etter 160 243 000. Én hendelse/tre felt. Ingen /22-rad i kontrollert blokk. |
| 2024, 210/40034048 | To hendelser/seks felt som over. Samlet med 341/857: **fem/elleve**. |
| 2025, 201/40034038 | /1 nivå 163 173 000; /22 nivå 33 408 000. To separate hendelser/to felt. Årsunionen for disse to kontoene: **sju/tretten**, uten antatt kontinuitet. |

Kilde: [konto-/årsrapporten](konto-aar.md). Dette er ikke antall for hele dokumenter eller komplette årsforløp. Forslags-/komitéfelt kommer i tillegg med egne roller.

## Matriserader

| ID | Autentisk prøve / nødvendig negativ kontroll | Forventet observerbar atferd etter begge innganger og gjenlesing | Ticket / port |
| --- | --- | --- | --- |
| M01 | Bevarte originaler, manifest, avledede XML og gzip-foreldre; mutert hash/lokator/tekst | Faktisk råhash, versjon og tekststed kontrolleres. Riktig original kan gjenfinnes; feil gir navngitt avvik. Avledet objekt rekonstrueres byteeksakt fra riktig forelder og dokumentert separator; ingen oppfunnet HTTP-proveniens. | T1, alle senere nye kilder. |
| M02 | Hele tosidige Innst.81: sammendrag, merknader, tilråding I–II; 1429/1,/22,/60 | Hele inventaret og relevant kontekst er tilgjengelig i dokumentvalg, også når konto ikke har beløpsrad. Dekning skiller råkilde, struktur og faglig avklaring. | T1 / V1. |
| M03 | To trioer med tre kilder/roller | 9/3/1, 9/3/1, 18/6/2 og 0/0/0 som definert over. Kildehenvisninger og relatert omtale stemmer; forslag/tilråding er ingen ekstra vedtatt hendelse. | T1 / V5,V9. |
| M04 | Prop.V punkt3→81II→211; Vega/RNB-omtale og avrundet lønn | /60 har stikkordsfullmakt, ikke beløpsdelta. Vega 10 mill. fordelt 5 i 2024/5 i 2025 og historisk RNB omtales med riktig rolle. Ingen nye 2025-nivåer eller eksakt lønn 2 796 000 konstrueres. | T1 / V1,V9. |
| M05 | Hele Prop.16 med delvis strukturert 1429-utvalg | Globalt 37-gruppe-/45-referanseinventar og fullmakter er synlig. Ingen merking som fullstendig strukturert proposisjon i T1; søstergrenens aktuelle strukturstatus fremgår. | T1, T5 / V1. |
| M06 | Dokument→konto→dokument og konto→dokument→konto | Samme dokument-/observasjons-/grunnlagsidentiteter. Åpnet dokument viser hele inventaret. Tilbake bevares kontopar, år og statuser; ingen ny kilde eller hendelse oppstår. | Alle T / V3. |
| M07 | Flere eksplisitte kontopar, hele kapittel, union og tomt utvalg; syntetisk kryssproduktfare | Utvalget følger ny kontrakt uten utilsiktede kapittel/post-kombinasjoner; gamle B6-filtre er uendret. Globale avvik/dekning beholdes ved null beløpsrader. | Alle T / V2,V3. |
| M08 | Like trioer; merket manglende stadium, faktisk null på 4400/2 senere | Avledet 0 krever to tilstedeværende sammenlignbare beløp. Manglende er ukjent, faktisk 0 beholdes som observert verdi. Resultat peker til inngangene og regelen. | T1, T5 / V5. |
| M09 | Gamle 210-observasjoners `round='uavklart'` | Ingen gammel ID, tolkning eller B5-status endres. Ny nysalderingskontekst er separat, kildebundet og versjonert; uten sammenligningsgrunnlag ingen differanse. | T1 / V5,V10. |
| M10 | Autentisk 315/78 +119→+129 mill. | Ni valgte kildefelt, tre vedtaksfelt, én vedtatt hendelse; avledet +10 mill. og 0 med eksakte innganger og likeverdig betydning. Øvrig dokumentinnhold har synlig delvis strukturering. | T2 / V5. |
| M11 | 85s postvise Ap/Sp/SV-unntak og plenum sak24 63–35 | Partigruppe, samlet komité der riktig, tilråding og vedtak har egne bevis. Generell støtteformulering overstyrer ikke postunntaket. Votering gjelder riktig sak/tidspunkt. | T2 / V6 roller. |
| M12 | Dagens kilder: opposisjon uten tallfestet alternativ; syntetisk alternativ; senere autentisk alternativ | Motstemmer blir ikke et numerisk forslag. Syntetisk negativ prøve merkes. Positiv parallellvisning krever autentisk alternativ, opphav og behandlingsutfall; denne porten er **åpen**. | T2 negativ; K1 før positiv V6. |
| M13 | Sak100927/81/210–211 mot 100889/95/359–364; like lokale romertall | Felles Prop. gir ikke felles postomfang. 1429 følger 81-grenen; 1420 følger 95. Lokalt II i 81 er ikke II i 95. Flere referatlenker med samme eksport-ID bevares. | T1 grensevern; T5/T6 positiv helgren / V4. |
| M14 | Full Prop.: 37/111/15, 45 ulike kontoangivelser, II–VI og faktisk 4400/2=0 | Alle eksakte tabellfelt samt øvrig tekst-/fullmaktsinventar avstemmes mot originalen. Delt ramme på flere poster multipliseres ikke; historisk/fremtidig kontekst blir ikke nye deltaer. Tolkningshull er synlige. | T5 / V1. |
| M15 | Beriktiget95 og 359–364: 36 trioer, 35 felles med Prop., ny32 | Alle 108 vedtaksfelt avstemmes. Hele forgreningen har 38 monetære posthendelser og seks separate fullmaktsvedtak. Ap/Sp/SV-begrunnelse, samlet tilråding og enstemmig vedtak skilles. Manglende Prop.32 gir ingen nullutfylling. | T6 / V1,V4,V5. |
| M16 | 341 (vedtatt2023, budsjett2024) →857→210 | For de to valgte kontoene fem posthendelser/elleve vedtaksfelt. Kildebundet rekkefølge, separate nivå/delta/før/etter. Lokal regning merkes avgrenset kontroll, uten årsbalansegodkjenning. | T3 / V2. |
| M17 | Hele 857s 1429-blokk til neste kapittel | Ingen /22-rad i denne blokken gir dokumentert fravær her, ikke 0 eller bevis for ingen andre RNB-saker. Dokument-/periodeinventaret viser resterende hull. | T3 / V2,V5. |
| M18 | 201 og 210 begge datert16.12.2024, men budsjett2025/2024 | Årsvalg og årsunion har riktige nivåer og 7/13-utvalg. Ikke filtrer på vedtaksdatoens kalenderår som budsjettår. Flere år summeres ikke til ett nivå. | T4 / V2,V7. |
| M19 | Like kontokoder over år, kjent oppgaveflyttingskandidat og syntetisk ukjent mapping | Separate forløp med ukjent kontinuitet. Ingen automatisk kobling ut fra kode/navn eller en oppdiktet +1000-regel. | T4 / negativ V7. |
| M20 | Vega-kandidat uten råoriginal og sammeårs510→1510; senere positivt årsskiftebevis | Kandidat/avgrenset forslag er ikke full vedtatt kontokontinuitet. Positiv gyldighet, år, oppgaveomfang og status må dokumenteres. **Åpen positiv port.** | K2 før positiv V7. |
| M21 | Tre kjente2024-vedtak, manglende perioderegister; senere eksplisitt helårsinventar | Delvis dekning er synlig, også uavklarte kandidater uten sikker kontokobling. Før+delta=etter og et bokstavelig1429-søk beviser ikke full periode. **Positiv helårsport åpen.** | T3 hull; K3 før full V2. |
| M22 | Flere seksjoner/relasjoner, gjentatt eksport/lesing og skifte av inngang | Samme P1/vedtaks-ID-er gjenbrukes. Mange-til-mange-relasjoner eller aliaser skaper ingen ekstra vedtatte hendelser, kopierte beløp eller dobbeltelling. | Alle T / V9. |
| M23 | Faktisk ny JSON-fil lukket/gjenlest uten nett/database; mutert binding | Original-/versjons-/lokator-/rolle-/status-/bevisbinding og utvalg kan kontrolleres fra filen. Manipulert hash, rolle, relasjon eller skjult avvik avvises/rapporteres etter kontrakten. | Alle T / V8. |
| M24 | Faktisk ny XLSX lukket/gjenåpnet, synlige celler/lenker og fullstendig kontrollgrunnlag | Samme antall, beløp, tekst, roller og statuser som JSON. Dokument-/kontonavigasjon virker innen filen, også offline. Lange tekststykker rekonstrueres tapsfritt i riktig orden; kildetekst blir ikke kjørbare Excel-formler. Ingen nødvendig sporbarhet er skjult bare i database. | Alle T / V8. |
| M25 | Ekte tidligere A/B-par, frossetB6/B8/B9, schema5 og standardvalg | Gamle lesere, bytegrunnlag, observasjons-ID-er, tolkninger og B5-avgjørelser består. Nye filer/ark/formatversjon velges eksplisitt. Ingen ny standard eller obligatorisk migrering. | Alle T / V10. |
| M26 | Ny offisiell vedtaksrespons sammen med fraværende, feilet, korrupt eller motstridende ny adapter/omtale/historikk | Nytt vedtak oppdages, råbevares, registreres og kan ordinært eksporteres. Valgfri berikelsesfeil blir synlig separat og blokkerer ikke kjernen, heller ikke med tomt visningsutvalg. | Alle T / V10. |
| M27 | Syntetiske ulike år/enheter/kontoer/beløpsbetydninger/detaljeringsnivå/omfang/roller; kildebelagt nivå vs delta | Ingen meningsløs stadiedifferanse eller sum av nivåer. Avledet forskjell har regel og eksakte innganger; uavklart grunnlag gir navngitt hull. Ingen automatisk faglig godkjenning. | Alle T / V5. |
| M28 | To rå95HTML-svar, begge «Beriktiget», kontrollert identisk hovedtekst; manglende tidligere versjon | Hvert HTTP-svar beholder hash/proveniens. Råresponsforskjell blir ikke oppfunnet semantisk dokumentrettelse. Tidligere versjon/rettelsesmelding står uavklart. | T5/T6 / V4,V10. |

## Dekning av målkrav og begrensninger

| Målkrav | Relevant matrise | Hva første snitt ikke lukker |
| --- | --- | --- |
| V1 helt dokument | M02,M04,M05,M14,M15 | T1 gir hele81 og delvisProp.; T5/T6 utvider navngitte tabeller/inventar, ikke generell fulltolkning av alle tekster. |
| V2 konto/år | M07,M16–M18,M21 | Full periode er åpen K3, ikke bevist av delutvalg. |
| V3 samme grunnlag/navigasjon | M06–M07 | Må demonstreres i faktisk produktuttrekk. |
| V4 dokumentgraf/versjon | M13,M28 | Urettet95/rettelseshistorikk mangler. |
| V5 sammenligning | M03,M08–M10,M15,M27 | Ukjent betyr fortsatt ukjent. |
| V6 flertall/mindretall | M11–M12 | Positivt tallfestet alternativ krever K1. |
| V7 kontinuitet | M18–M20 | Flerårsfilter kan leveres; positiv kontinuitet krever K2. |
| V8 reelle filer | M23–M24 | Ingen nye visningsfiler er laget i denne undersøkelsen. |
| V9 ingen dobbeltelling | M03–M04,M22 | Fullmakt, tekst, forslag og avledet forskjell blir ikke vedtatte hendelser. |
| V10 kompatibilitet/uavhengig innlesning | M25–M26,M28 | #10s faktiske driftsaksept er separat og forblir åpen. |

Det er ikke tillatt å krysse av alle V1–V10 bare fordi T1 er levert. Hver ticket lukker kun sine kildebelagte tilfeller og dokumenterer øvrige hull. Gjennomføring og testbevis registreres først ved et senere godkjent byggemandat.
