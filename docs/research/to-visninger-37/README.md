# #37 – Kildegrunnlag og forslag til de to visningene

**23. oktober 2026. Forslag før implementering.** Undersøkelsen bygger på main `542316088cbca39e35d7b8f26cdd0aee0e96161c`, etter levert O2b/PR #39. [Produktkrav V1–V10](../../to-visninger.md) gjelder fortsatt. [Den konkrete planen](../../visningspilot-plan.md), [testmatrisen](testmatrise.md) og [ni ticketutkast med avhengigheter](tickets/README.md) legges frem samlet. Ingen ny visning, eksportleser eller byggeticket er implementert/publisert av denne leveransen. #10 forblir åpen.

## Anbefalt første leveranse

**T1: hele Innst. 81 S, vedtak 210/211 og kontoene 1429/1, /22 og /60 i budsjettåret 2024**, med relevant Prop. 16 S-innhold og hele proposisjonens inventar. Brukeren kan starte i dokumentet eller konto-/årsutvalget og gjenfinne samme kilder, tekst, beløp, roller og relasjoner i faktisk gjenlest JSON og Excel. Prop. 16 S er først delvis strukturert; hele Innst. 81 S skal være inventert og tilgjengelig. Fullmakten på /60 er ingen tredje bevilgningshendelse.

Dette er et nytt opt-in-snitt. O2bs seks vedtaksfelt og to posthendelser gjenbrukes; regjeringens og komiteens to tilsvarende triosett gir tolv separate kildefelt. Dermed er fasiten **18 eksakte tabellfelt med tre roller, fortsatt bare seks vedtaksfelt og to vedtatte hendelser**. Avrundet omtale er ikke nye eksakte tabellfelt. Gamle `round='uavklart'`, ID-er og filformater beholdes; eventuell nysalderingskontekst får separat kildebundet versjon.

## Hva undersøkelsen faktisk underbygger

| Kildesnitt | Kontrollert funn og praktisk konsekvens | Bevis |
| --- | --- | --- |
| Prop. 16 S → Innst. 81 S → 210/211 | To identiske før/endring/etter-trioer for 1429/1 og /22, samt tekst-/stikkordsfullmakt på /60. Komiteen er samlet. Omtalens lønnstall er avrundet; 2 796 000 er ikke et kildeobservert eksakt lønnsbeløp. | [Eksisterende grunnlag, inventar og ekte O2-filer](eksisterende-grunnlag.md). |
| Hele Prop. 16 S | 37 endringstabellgrupper, 111 eksakte felt, 15 kapitler. 45 ulike uttrykkelige kontoangivelser omfatter også stikkord/fullmakt/kontekst og er ikke 45 bevilgningsendringer. Fullmakter og historiske/fremtidige omtaletall har egne roller. | [Fullt manuelt tabell-/kontoinventar](eksisterende-grunnlag.md#hele-prop-16-s-synlig-inventar-utover-1429). |
| Den andre proposisjonsgrenen | Beriktiget Innst. 95 S har de øvrige 35 endringsgruppene fra proposisjonen **og ny 1420/32: +270 mill.** Totalt 36 grupper. Alle samsvarer eksakt med 359; fullmaktene går til 360–364. Ingen Prop.-rad 32 betyr manglende forslagsfelt, ikke null. | [Forgrening, råoriginaler, lokatorer og plenumsbevis](forgrening.md). |
| Roller i Innst. 95 S | Ap/Sp/SV begrunner post 32; samlet komité tilrår; Stortinget vedtar I–VI enstemmig. Begrunnelsen kan ikke automatisk tilskrives alle disse aktørene. «Beriktiget» er bevart, men urettet versjon/rettelsesmelding mangler. | [Forgreningsrapporten](forgrening.md). To ulike HTML-responshasher har identisk kontrollert hovedtekst. |
| Autentisk komitéendring | 315/78, Prop. 25 S → Innst. 85 S → vedtak 208: regjeringen foreslår +119 mill., Ap/Sp/SV +129 mill.; vedtatt +129 mill. Avledet stadieforskjell +10 mill. Motstemmer 63–35 gir ikke i seg selv et eget tallfestet mindretallsalternativ. | [Komitéendring, presise beløp, aktørunntak og votering](komiteendring.md). |
| Flere runder og år | 341 (2024-nivå, vedtatt 2023), 857 (RNB 2024), 210 (nysaldering 2024), 201 (2025-nivå, vedtatt samme dato som 210). For to valgte kontoer: fem 2024-posthendelser/elleve vedtaksfelt; med de to separate 2025-nivåene sju/tretten. | [Konto-/årsfunn med tabellokatorer og hull](konto-aar.md). Tallene gjelder bare dette uttrykkelige utvalget. |

For hele den undersøkte Prop. 16 S-forgreningen er det **38 monetære postendringer og seks separate fullmaktsvedtak**. Åtte formelle vedtak betyr ikke åtte eller 44 beløpshendelser. Dette er manuelt kildekontrollert fasit for senere bygging, ikke en allerede utført ny produktimport.

## Proveniens og faktisk utført kontroll

Rapportene skiller bevart original, avledet forskningsuttrekk, nettverifisert kandidat, tolkning og uavklart forhold. Originale HTTP-responser beholder egne hasher, URL-er, hentetider, feiljournaler og representasjon. Detaljerte lokatorer finnes i rapportene og deres JSON-ledgere; de skal ikke erstattes av bare dokumentlenker.

| Grunnlag | Manifest og lokatorer | Bevaringsgrense |
| --- | --- | --- |
| O1/O2, hele 81 og Prop. 16 S | [O1-manifest](../omtale-o1/source-manifest.json), [støttemanifest](../omtale-o1/supporting-manifest.json), [B8-fixturer](../../../tests/fixtures/b8/README.md) | Tidligere originaler er gjenbrukt uendret. Ekte A/B JSON-/Excel-par er lest readonly; XLSX-tekstgrunnlaget er sammenholdt byteeksakt med JSON. Ingen nye visningsfiler er produsert. |
| Komitéendring 315/78 | [Manifest](originals/komite/manifest.json), [passasjer](originals/komite/passages.json), [rapport](komiteendring.md) | Nye offisielle originaler og faktisk HTTP-feilinnhold er bevart, sammen med gjenbrukt O1-plenum. Aktør-/voteringssted er kontrollert særskilt. |
| Konto/år og avledede vedtaksobjekter | [Manifest](originals/aar/manifest.json), [konto-/tabellbevis](originals/aar/account-evidence.json) | To tidligere fullsesjonssvar er bevart tapsfritt som gzip med transportmetadata. 341/201 er komplette uendrede objekter innpakket med originale konvoluttdeler og ett dokumentert LF, ikke nye HTTP-svar. Dekompresjon og rekonstruksjon er kontrollert. |
| Innst. 95 S og vedtak 359–364 | [Manifest](originals/forgrening/manifest.json), [inventar](originals/forgrening/inventory.json), [passasjer](originals/forgrening/passages.json), [kontrollresultat](originals/forgrening/verification.json) | Hele nye HTML/PDF-/saks-/plenumssvar. Seks API-objekter er avledet med egne byteoppskrifter fra den samme bevarte fullsesjonsoriginalen, uten innsatte byte. Alle 36 trioer er avstemt mellom innstilling, API, vedtaksside og plenum. |

PDF-tekstuttrekk, tabell-/passasjeledgere og kontrollbilder er avledede hjelpemidler, ikke erstatning for originalene. DNS-feil har ingen råinnholdshash. HTTP 403 eller 500 kan ha en hash for den faktisk bevarte feilkroppen; den er ikke hash for ønsket dokument. Ingen dokumentkorreksjon utledes bare fra endret responsbytehash.

Den nye testmatrisen er **foreslått fremtidig produktaksept**. Dagens kildekontroller og lesing av ekte O2-filer lukker ikke den. Ingen bred produkttestsuite er nødvendig eller hevdet kjørt for denne rene dokument-/kildeleveransen.

[Samlet kontrolljournal](verification.json) registrerer 38 direkte hash-/bytekontroller, dekompresjon av to foreldre og byteeksakt rekonstruksjon av åtte vedtaksutdrag. 22 forsknings-JSON-filer ble parset og 320 lokale Markdown-lenkemål kontrollert uten manglende mål. Uavhengig dokument-/spesifikasjonsgjennomgang fant ingen materielle feil; en meldt ankerfeil er rettet. Dette er dokument- og kildekontroll, ikke ferdig V1–V10-produktaksept.

## Åpne porter og beslutning

- **K1:** autentisk tallfestet parallelt alternativ med opphav og behandlingsutfall. Faktisk komitéendring er funnet; positiv alternativaksept gjenstår.
- **K2:** positiv kontokontinuitet over år, med bevart original, gyldighet og riktig oppgave-/postomfang. Vega-kandidaten og sammeårs-omnummereringen gir ikke dette alene.
- **K3:** uttømmende 2024-kildeinventar for valgte kontoer, med begrunnede ekskluderinger og uavklarte kandidater. Tre kjente vedtak og korrekt lokal regning er ikke full årsdekning.

Disse kunnskapsportene blokkerer ikke det foreslåtte første snittet. [Ticketoversikten](tickets/README.md) viser seks små byggeleveranser og tre kunnskapsleveranser med faktiske avhengigheter. Anbefalingen er å godkjenne **T1 først** og holde resten som forslag. Publisering/bygging krever senere mandat. Ingen automatisk faglig godkjenning, omskriving av gamle formater eller stenging av #10 følger av forslaget.
