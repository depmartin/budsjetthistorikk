# Komitéendring: 315/78 i nysalderingen 2024

Undersøkt 23. oktober 2026 under [#37](https://github.com/depmartin/budsjetthistorikk/issues/37), fra `542316088cbca39e35d7b8f26cdd0aee0e96161c`. Dette er én avgrenset primærkildeundersøkelse, ikke implementering eller faglig godkjenning. AGENTS.md, arbeidsflyten, issue tracker, begrepsreglene, GLOSSARY.md, ansvarsdelingen, kildefunnene, hele issue-/kommentarsnapshotet og `docs/to-visninger.md` er lest. Matt Pococks research-skill er fulgt i den delegerte forskerrollen; PDF-skillen er brukt til kildeinspeksjon. Ingen produktkode, Git- eller GitHub-tilstand er endret. #10 står åpen.

## Konklusjon og valg

**Kapittel 315 post 78 Frivillighetstiltak, budsjettåret 2024**, gir en liten positiv prøve: regjeringen foreslo **+119 000 000 kroner**, komiteens flertall tilrådde **+129 000 000 kroner**, og Stortinget vedtok det siste. Førbeløpet er **29 050 000**, foreslått etterbeløp **148 050 000**, tilrådd og vedtatt etterbeløp **158 050 000 kroner**. Kildene angir endring og før/etter uttrykkelig; dette er ikke oppdiktede nivåer.

Kandidaten var allerede identifisert i [P2s stadierester](../historisk-excel/p13-p2/stage-residuals.json), konto `315/78`. Denne undersøkelsen følger det ene sporet videre til avsender, særskilt votering og endelig vedtak. Det er ikke foretatt bredt årssøk eller ny årsimport. [O1-konklusjonen](../omtale-o1/README.md) består: 210/1429 har samlet komité og ingen komitéendring. Den valgte casen tilhører en annen proposisjon og **sak nr. 24**, selv om referatet og fellesdebatten også dekker 210 i sak nr. 25.

**Bevisstatus:** Forslag → flertallstilråding → særskilt vedtakelse → vedtak 208/40034045, sak 100887, er verifisert for denne posten. Casen gir ekte komitéendring og dokumentert motstand. Den gir **ikke en særskilt tallfestet mindretallstilråding eller flere parallelle parlamentariske beløpsforslag**. Dette begrenser V6; den må ikke presenteres som full oppfyllelse av hele V6 alene.

## Originaler, transport og kontroll

[Manifestet](originals/komite/manifest.json) bevarer forespurt og faktisk mottatt URL, start-/sluttid i UTC, HTTP-status, responsheadere, byteantall og SHA-256. `Set-Cookie` er utelatt fra metadata; responskroppene er uendret. Syv nye vellykkede responskropper er bevart. Første forsøk fra sandkassen ga fire DNS-feil uten responsbyte; ingen hash er oppfunnet for dem. Deretter lyktes henting med eksplisitt nettverkstilgang. Et forsøk med bare `did=40034045` ga HTTP 500 og faktisk feilside: [vedtak40034045.html](originals/komite/vedtak40034045.html), SHA-256 `5c7743ddfe2cc62db9db7a993d95d3abb31f55b884dbb7ca2cb1a08c774654ec`. Feilsiden brukes ikke som vedtaksbevis. Den fullstendige lenken med `p=100887` ga 200 og riktig vedtak.

| Bevart original | Byte | SHA-256 |
| --- | ---: | --- |
| `prop25s-ch2.html`, del-HTML med postomtale | 92 231 | `87205b4e91472cdef72f73abe482d01b1981a8cd4c0f4863951bb8a2d4d20c7b` |
| `prop25s-ch4.html`, del-HTML med forslag | 104 457 | `17922400028d80971540293ace9d6904d3be86b8d97d880a5b6a18bdd2bb5ecf` |
| `prop25s.pdf`, full PDF, 8 sider | 777 380 | `aeb725790fa208766fc15d24082346ce8c5295c26208a04f7b266b2bce37dd1a` |
| `inns85s.html`, full HTML | 346 750 | `0adeb21331ef20b44186ae6fae539bd304d4e9fe2a22aa64698469c90804c657` |
| `inns85s.pdf`, full PDF, 8 sider | 560 552 | `961591a7f80608e9b15002de1b06f8e51162879b0f0137d0ef38eb3254404288` |
| `vedtak40034045-sak100887.html`, vedtak 208 | 182 316 | `232e06bc5ed62185a856016fea4ed609429d8c654dc3070d8698b3085102c1ab` |
| `sak100887.xml`, full saksrespons | 17 096 | `cfaf7b451df64c4a4cad5f437f04a06da0f1e2377159a6cde6cee6ee2f76fb2e` |

Nye vellykkede HTML-kilder ble mottatt 23. oktober kl. 10.40.39–10.40.40 UTC; PDF-er og presis vedtaks-/saksreferanse kl. 10.41.14–10.41.17 UTC. Hentetidene er ikke dokumentdatoer. Fullstendige tidsgrenser står i manifestet.

Plenumsbeviset gjenbruker [O1s uendrede original](../omtale-o1/originals/votering-161224.html), 2 094 710 byte, SHA-256 `22170a60f769e89642b2e52525899903020de25938aa2b566ea28d11f85fb2e5`, hentet 22. oktober kl. 12.33.42–12.33.47 UTC. Hashen er kontrollert på nytt; det er ingen ny innhenting. Den opprinnelige forespurte URL-en og faktisk mottatte fullreferat-URL-en er kopiert som metadata i manifestets `reused_sources`.

[passages.json](originals/komite/passages.json) bevarer syv komplette relevante HTML-kontekstblokker med kildehash, XPath, HTML-ID og avledet tekst. Mellomrom er komprimert i tekstfeltet; markup/originalbyte er bevart. PDF-tekstene er avledet med pypdf 6.10.0. Fire relevante PDF-sider er rendret med pypdfium2 og visuelt lest i [lokatorsjekken](originals/komite/lokatorsjekk.png). De er kildekontroll, ingen nyprodusert budsjettfigur.

## Presise bevis og roller

Alle tabellrader og PDF-sidetall nedenfor er 1-baserte. Trykte PDF-sidetall samsvarer her med PDF-sidene. Absolutte XPaths finnes i passages.json; radlokatorene gjelder den hashfestede representasjonen ovenfor.

| Belegg | Offisiell primærkilde og presis lokal lokator | Hva beviset viser |
| --- | --- | --- |
| P, regjeringens forslag | [Prop. 25 S (2024–2025), forslag](https://www.regjeringen.no/no/dokumenter/prop.-25-s-20242025/id3075636/?ch=4). `prop25s-ch4.html`, første tabell, `tbody/tr[6]` kapittel, `[13–14]` post/endring/før/etter. PDF side 6. | Forslagets I gjelder statsbudsjettet **2024**, i **kroner**, posttotal 315/78. +119 000 000 fra 29 050 000 til 148 050 000. |
| P-omtale, regjeringen | [Prop. 25 S, kapittel 2](https://www.regjeringen.no/no/dokumenter/prop.-25-s-20242025/id3075636/?ch=2). `prop25s-ch2.html`, `/html/body/main/div/div[3]/div[3]/div[9]`, avsnitt `#kap2-p11`–`#kap2-p14`; PDF side 2, venstre spalte. | Regjeringens forklaring til post 78 beholdes samlet, inklusive sammenhengen med Riksteatret på en annen post. Den er ikke Stortingets egen ordlyd. |
| K0, komitékontekst | [Innst. 85 S (2024–2025), full HTML](https://www.stortinget.no/no/Saker-og-publikasjoner/Publikasjoner/Innstillinger/Stortinget/2024-2025/inns-202425-085s/?all=true). `#m2_1 > div > p[1–2]`; PDF side 4, høyre spalte. | Navngitt samlet komité støtter regjeringens proposisjon. Høyre og Venstre har en generell merknad om nysaldering og aktivitet i 2025. Merknaden er ingen postvis alternativ beløpstabell og endrer ikke budsjettåret 2024. |
| K1, faktisk endring | Samme innstilling, `#m2_2_1`, full blokk med flertallsangivelse, forklaring og forslagstabell; `table/tbody/tr[1]` kapittel, `[2–3]` endring/før/etter. PDF side 4, høyre spalte og tabellen nederst over hele sidebredden. | **Flertallet fra Ap, Sp og SV** øker støtten til LNUs Frifond med 10 mill. utover regjeringens forslag og fremmer +129 000 000 fra 29 050 000 til 158 050 000. |
| K2, tilrådingsrolle | Samme innstilling, `#m3 > div.krnl_chapter > p`, og romertall I, første tabells `tbody/tr[7]` kapittel, `[14–15]` post/endring/før/etter. PDF side 5. | Tilrådingen fremmes samlet **unntatt 315/78**, som fremmes av Ap, Sp og SV. Det er denne flertallstilrådingen som inneholder +129 mill.; setningen om samlet komité kan ikke arves til denne posten. |
| V, postvis vedtakelse | [Referat 16. desember 2024, voteringer](https://www.stortinget.no/no/Saker-og-publikasjoner/Publikasjoner/Referater/Stortinget/2024-2025/refs-202425-12-16/voteringer#2024-12-16-24). Bevart O1-original, `#2024-12-16-24`, I-tabellens `tbody/tr[7]` kapittel og `[14–15]` post. Hele blokken og sluttavsnittene inngår i passages.json. | Innst. 85 S/Prop. 25 S identifiseres, tabellen gjengis, og **I kap. 315 post 78 voteres særskilt**. H, FrP og V varsler motstand. Tilrådingen vedtas **63 mot 35**, voteringsutskrift kl. **19.49.48**. Resten av I samt II vedtas enstemmig i en annen votering. |
| S, endelig vedtak | [Vedtak 208/40034045, sak 100887](https://www.stortinget.no/no/Saker-og-publikasjoner/Vedtak/Vedtak/Sak/?did=40034045&p=100887). `vedtak40034045-sak100887.html`, `//h2[contains(.,'Vedtak 208')]/..`; I-tabellens `tbody/tr[7]` kapittel, `[14–15]` post/endring/før/etter. | Endelig vedtak gjentar +129 000 000 fra 29 050 000 til 158 050 000 for 2024. Identiteten følger URL og «Vedtak 208», støttet av den eksplisitte voteringskjeden; ikke bare samme beløp. |
| Relasjon og dato | [Saks-API 100887](https://data.stortinget.no/eksport/sak?sakid=100887). Navnerom `http://data.stortinget.no`; `/detaljert_sak/publikasjon_referanse_liste/publikasjon_referanse[1,3,4,5]`; saksgangens hendelser `FREMMET`, `AVGITT`, `VOT`. | Binder proposisjon, innstilling og referat til samme sak. Fremmet **22.11.2024**, innstilling avgitt **09.12.2024**, votering **16.12.2024**. API-ens gamle anker `#161224-24` bevares rått; faktisk bevart DOM-ID er `2024-12-16-24`. Dette metadata-beviset erstatter ikke de postvise tabell-/voteringsbevisene. |

Dokumentene er i sesjon **2024–2025**; de aktuelle beløpene gjelder budsjettåret **2024**, runden **nysaldering**. Dette er posttotal i kroner. LNUs Frifond-begrunnelse gjelder det ekstra flertallstillegget. Den gjør ikke hele postøkningen på 129 mill. til LNU-bevilgning, og det avrundede omtaleutsagnet blir ikke en ekstra vedtatt delhendelse.

## Sammenligningsfasit

| Observasjonsrolle, samme 315/78 og år 2024 | Kildeobservert før | Uttrykkelig foreslått/tilrådd/vedtatt endring | Kildeobservert etter | Status og avsender |
| --- | ---: | ---: | ---: | --- |
| Regjeringsforslag, Prop. 25 S I | 29 050 000 | +119 000 000 | 148 050 000 | Forslag fra regjeringen, ikke vedtatt som dette beløpet. |
| Komiteens tilråding, Innst. 85 S I | 29 050 000 | +129 000 000 | 158 050 000 | Flertall Ap/Sp/SV på posten; ingen samlet komité. |
| Endelig vedtak 208, I | 29 050 000 | +129 000 000 | 158 050 000 | Stortinget, særskilt vedtakelse 63–35 den 16.12.2024. |

Tre regnekontroller: 29 050 000 + 119 000 000 = 148 050 000; 29 050 000 + 129 000 000 = 158 050 000; 129 000 000 − 119 000 000 = 158 050 000 − 148 050 000 = **10 000 000**. Siste regnestykke er en **avledet stadieforskjell**, knyttet til de konkrete innobservasjonene. Komiteens tekst sier også uttrykkelig «10 mill. kroner ut over regjeringens forslag»; tekstutsagnet og regnestykket har egne kilde-/beregningsroller. Forskjellen tilråding → vedtak er beregnet **0** med begge stadium til stede; dette må skilles fra manglende stadium.

Det finnes **én vedtatt posthendelse** i dette utvalget, med tre før-/endrings-/etterobservasjoner i vedtaket. Flere forslagstall, komitéomtale, gjengivelse ved votering, regnestykker og kildeversjoner gir ingen ekstra vedtatte hendelser. Verken 119 og 129 mill. eller etterbeløpene skal summeres til bevilgningsendring. Førbeløpet er kildeobservert for dette leddet, ikke en undersøkt startsaldo for hele 2024.

**Mindretall og alternative forslag:** H/V-merknaden og H/FrP/Vs varslede motstand bevares som forskjellige støtte-/motstandsbelegg med eget omfang. De 35 motstemmene gjør ikke en tenkt +119 mill.-mindretallstilråding til et observert alternativ eller vedtak. Ingen separat slik tabell er etablert. En senere adapter må kunne beholde et alternativ med ukjent konto/beløp/utfall uten å sperre det separat dokumenterte vedtaket på 129 mill. En syntetisk negativ kontroll av dette er mulig, men skal merkes syntetisk. Et autentisk parallellforslag krever egen kildeport før full V6-aksept.

## Hva de to inngangene kan vise

**Dokumentinngang:** Velg den bevarte Prop. 25 S- eller Innst. 85 S-versjonen og vis et tydelig **315/78-pilotutvalg**, med originalens fulle PDF/HTML-inventar og synlig ustrukturert øvrig innhold. Vis postens forslag, flertallsunntak og vedtaksforbindelse. Hele dokumentet har flere konti og en separat fullmakt i II; dette notatet strukturerer ikke alt og gir ikke V1-fullstendighet. Den flerårige Narvik-fullmakten er ikke et annet budsjettår for 315/78.

**Konto-/årsinngang:** Velg 315/78, 2024, og vis denne dokumenterte nysalderingsrunden med tre roller og to stadiesammenligninger. De to inngangene skal peke på samme beløp og kildeidentiteter. Saldert budsjett, RNB, andre 2024-endringer og årene 2023/2025 er ikke undersøkt; vis hullet/dekningsgrensen uten å gi førbeløpet status som saldert eller helårsgodkjent. Casen alene gir ingen kontokontinuitet, V2-årsdekning eller V4-forgrening.

## Eksakte senere V5-/V6-prøver

Dette er **foreslåtte produktakseptprøver**, ikke tester kjørt av undersøkelsen.

| Prøve | Autentisk forventning | Dekning |
| --- | --- | --- |
| V5-a: beløpsbetydning | Bevar 29 050 000 før, +119/+129 mill. endring og 148 050 000/158 050 000 etter som egne betydninger; kroner, 2024 og posttotal følger alle stadium. | Positivt kildegrunnlag komplett for ett postledd. |
| V5-b: stadiesammenligning | Forslag → tilråding gir beregnet +10 000 000 for både endring og etterbeløp; tilråding → vedtak gir beregnet 0. Beregningene peker til de faktiske observasjonene og gir fortsatt én vedtatt hendelse. | Positivt kildegrunnlag komplett. |
| V5-c: manglende stadium | Fjern tilrådingskilden i en merket syntetisk variant. Resultat er hull/ukjent sammenligning, aldri null tilråding eller konstruert uendret forslag. | Kildene gir god positiv baseline; fraværsvarianten er syntetisk. |
| V6-a: avsender og unntak | +129 mill. og LNU-tillegget tilskrives Ap/Sp/SV. K0s generelle støtte eller K2s «samlet komité» uten unntaksleddet får ikke overskrive dette. | Autentisk komitéendring og flertall bevist. |
| V6-b: støtte og vedtakelse | Knyt 63–35-voteringen bare til I 315/78 og vedtak 208. Enstemmigheten i resten av I/II eller sak 25 gir ingen enstemmighet på 315/78. H/V-merknaden blir ingen flertallsbegrunnelse. | Autentisk postvis vedtakelses-/motstandsbevis. |
| V6-c: parallelle alternativer | Ingen separat tallfestet mindretallstabell fylles inn fra motstemmer. Et syntetisk tillegg med uavklart alternativ beholder egen status og endrer ikke vedtaksresultatet. | Negativ rolleprøve mulig; **autentisk positiv parallellforslagsprøve mangler**. Hele V6 kan ikke godkjennes fra denne casen alene. |

V3/V8/V9 kan senere prøves for dette smale utvalget gjennom faktiske JSON-/Excel-filer og gjenlesing; denne undersøkelsen leverer ikke slik produktaksept. V7 krever separat kontinuitetsbevis. Uavhengig ny vedtaksinnlesning og gamle ID-er/formater/valg må bestå; fravær eller feil i denne nye forslag-/komitéberikelsen må aldri hindre den.

## Lite komplett byggeticketforslag og gjenstående kildeport

**Foreslått, ikke publisert eller byggemandat:** «Vis dokumentert komitéendring for 315/78 i nysalderingen 2024 gjennom begge utvalg og gjenlest JSON/Excel». Del av #37. Kildegrunnlaget ovenfor holder for dette **postavgrensede** snittet. Ticketen skal uttrykkelig unnta full V1/V2/V6-/årsaksept, og få egen godkjent spesifikasjon før bygging.

Brukerutfall: For valgt Prop. 25 S/Innst. 85 S/vedtak 208 og for valgt 315/78/2024 får brukeren samme tre stadium, beløpsbetydning, flertallsrolle, vedtaksbevis, kildeversjoner og +10 mill.-sammenligning, med tydelig pilot-/dekningsmerke. Leveransen går fra de bevarte originalene gjennom smal separat forslag-/innstillingsstrukturering og eksisterende uavhengig vedtaksgrunnlag til to utvalg, faktisk skrevne/gjenleste JSON og Excel. Ingen generell dokumentparser eller årsimport inngår.

Aksepten er V5-a/b, V6-a/b, merket syntetisk V5-c og V6-c, samt identitets-/hendelseskontroll ved bytte av inngang og JSON-/Excel-gjenlesing. Kilder, komplette relevante tekster, roller, lokatorer og beregningsinnganger skal bestå. Ustrukturerte øvrige konti og II-fullmakten skal forbli synlige i inventaret. Eventuelle nye felt/uttrekk krever eksplisitt versjonert kontrakt og regresjonsbevis i ticketen; gamle B1/B2/B3/B5-/omtale-ID-er og frosne formater omtolkes ikke. Avhengighet til #34/#35 skal begrunnes bare dersom deres konkrete pilotfunksjoner faktisk gjenbrukes; kildene her gjør ikke #35 til automatisk blokkering.

**Separat gjenstående undersøkelsesticket:** «Finn én autentisk parallell beløpsforslagsgren til V6 og bind konto/år/avsender og faktisk voteringsutfall». Kildeport: bevart full forslag-/innstillingskontekst, den alternative tabellen, eksplisitt konto-/års-/beløpsomfang, avsender og voteringsbevis som skiller forkastet/uavklart fra vedtatt. Ukjent alternativ kan beholdes uavklart uten å endre det selvstendig dokumenterte vedtaket. Denne porten må passeres før full positiv V6-aksept; den er ikke et nødvendig datakrav for å registrere vedtak 208 eller nye offisielle vedtak.

## Utført kontroll og begrensning

Originalhashene og gjenbrukt referathash er kontrollert. De relevante HTML-radene, avsenderavsnittene, særskilt votering og vedtakstabellen er lest i de bevarte bytene. Begge PDF-er er fullstendig tekstuttrukket; de fire relevante sidene er visuelt kontrollert for tabell-, side- og spalteplassering. Regnestykkene ovenfor er eksakte heltallsberegninger. Ingen produktprøve, full årsreplay, generell parser, videre kildeår, alternativ beløpstabell eller faglig godkjenning er påstått. Rapporten bevarer eksisterende filer og støtter en avgrenset senere byggbeslutning; #37 og #10 har fortsatt sine separate rester.
