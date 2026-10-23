# Dokumentvisning og konto-/årsvisning

Status: eierbekreftet produktkrav 23. oktober 2026. Dette er det autoritative målbildet og akseptgrunnlaget for de to inngangene nedenfor, under [#1](https://github.com/depmartin/budsjetthistorikk/issues/1) og [#32](https://github.com/depmartin/budsjetthistorikk/issues/32), med konkretisering i [#37](https://github.com/depmartin/budsjetthistorikk/issues/37). Kravene er ikke implementert av denne dokumentleveransen eller av O2a/O2b. #37 er en konkretiserings-/kravissue; funksjonsbygging krever et avgrenset kildegrunnlag, en konkret spesifikasjon og eget byggemandat.

[Observasjonsformatet](observasjonsformat.md) og [begrepslisten](../GLOSSARY.md) fastsetter de faglige skillene. [Omtaleplanen](omtale-plan.md) beskriver tekstbelegg og senere temasøk. [Ansvarsdelingen](ansvarsdeling.md) gjelder fortsatt: innlesning bevarer og strukturerer kilder, analyse velger, sammenligner og fremstiller.

## To innganger til samme grunnlag

**Dokumentvisning:** Brukeren velger en bestemt proposisjon, innstilling eller et vedtak, med dokumentversjon. Visningen skal gi alle kapitler/poster og alle endringer og beløpsopplysninger som finnes i dokumentet, med relevant omtale, kildehierarki og presise kildepekere. Den skal vise den uttrykkelige forbindelsen proposisjon → innstilling → vedtak og gjøre det enkelt å sammenligne hva som ble endret mellom behandlingsleddene. Når behandlingen forgrener seg, vises de dokumenterte grenene og deres konto-/årsavgrensning.

**Konto-/årsvisning (kapittel-/postvisning):** Brukeren velger ett eller flere kapitler/poster og ett eller flere budsjettår. Visningen skal finne alle dokumenter og behandlingsledd som berører utvalget: opprinnelig regjeringsforslag, eventuelle tilleggsforslag, innstilling, endelig vedtak, RNB, nysaldering og øvrige endringer, også vedtak uten proposisjon. Hvert beløp skal ha sin talltype, behandlingsrunde, beløpsbetydning, dato/rekkefølge, kilde og tilknyttede omtale med avsender og status. Manglende grunnlag vises der det hører hjemme i forløpet.

Begge inngangene bruker de samme kildeidentitetene, observasjonene, relasjonene og hendelsene. Fra et dokument skal brukeren kunne åpne en berørt konto og dens årsforløp; fra kontoen skal brukeren kunne åpne hele det aktuelle dokumentet og dets behandlingsforbindelser. Bytte av inngang er et nytt utvalg i samme grunnlag, ikke ny registrering av beløp eller hendelser.

## Dokumentkjede med dokumentert omfang

Dokumentkjeden er en mange-til-mange-graf. Én proposisjon kan gi flere saker, innstillinger og vedtak; en innstilling eller et vedtak kan ha flere dokumenterte forslagsgrunnlag. Hver forbindelse må vise hvilke kapitler/poster og budsjettår den gjelder, rolle, behandlingstid og dokumentert rekkefølge, kildebevis og avklaringsstatus. Ukjent omfang eller rekkefølge beholdes som ukjent. Dokumentdato, vedtaksdato, budsjettår, sesjon og hentetid har forskjellige betydninger.

Dette er et faktisk behov: [B8s bevarte saksprøver](research/b8/README.md#observert-dokumentkjede) viser Prop. 16 S (2024–2025) i både sak 100927, kap. 1429/Innst. 81 S, og sak 100889, unntatt kap. 1429/Innst. 95 S. Felles proposisjon gir ikke felles postomfang. [O1-kildegrunnlaget](https://github.com/depmartin/budsjetthistorikk/blob/417e4fdeb22c8c510a56d038686cbf5ffa740cd2/docs/research/omtale-o1/README.md) dokumenterer den avgrensede forbindelsen fra konkrete forslag og omtale via Innst. 81 S og plenumsbeviset til 210. Det beviser ingen komitéendring eller årsdekning.

En saks-/dokumentrelasjon og en postvis forslag-/vedtaksrelasjon må kunne kontrolleres hver for seg. Konto-, forslag-, støtte- og vedtakelsesbevis kan ha forskjellig omfang. Felles dokument, samme dokumentnummer, likt kontonummer eller likt beløp er ikke tilstrekkelig grunnlag for en postkobling. Henvisningene må bevare dokumenttype, nummer, sesjon og eksakt versjon; ett nummer alene identifiserer ikke dokumentet.

Regjeringens forslag, komiteens gjengivelse, tilråding, flertalls-/mindretallsforslag, støtte og Stortingets vedtakelse vises med sine egne roller og tekstbelegg. Parallelle alternativer bevares separat. En begrunnelse fra et mindretall tilskrives ikke vedtatt flertall uten dokumentert forbindelse. Fravær av innstilling, forslag eller vedtak er et hull, ukjent grunnlag eller et kildebelagt ikke relevant ledd, aldri et nullbeløp eller automatisk uendret forslag.

## Beløp og sammenligning

En kildeobservert nivåverdi, et uttrykkelig endringsbeløp, et før-/etterbeløp og en beregnet forskjell er forskjellige opplysninger. Visningen skal bevare råbeløp, enhet, kilde, lokator og kontrollstatus og merke beregninger med inngangsobservasjoner, sammenligningsgrunnlag og regel. Dokumenttypen alene avgjør ikke hva et beløp betyr.

Forskjellen mellom regjeringens forslag og komiteens tilråding innen samme behandlingsrunde er en **stadiesammenligning**. En senere RNB- eller nysalderingshendelse hører til en ny behandlingsrunde. Ingen av delene blir et vedtatt endringsbeløp bare ved subtraksjon. Sammenlignbare beløp må ha dokumentert samme konto, budsjettår, enhet, detaljeringsnivå og beløpsomfang. Sammenligningen angir talltype, forslagsrolle og behandlingsledd for hvert inngangsbeløp. Motstrid eller ukjent sammenligningsgrunnlag skal synes.

### Syntetisk illustrasjon – ingen autentisk kildefasit

Eierens illustrasjon gjelder kapittel 100 post 1 i ett **syntetisk budsjettår**. Alle dokumentstadier og beløp nedenfor er oppdiktede eksempler; «Prop. 1 S» angir ingen kontrollert virkelig proposisjon eller sesjon. At de fire beløpene uttrykker nivå for samme konto, år og omfang, er her en **syntetisk forutsetning**, ikke en kildeavklaring.

| Syntetisk behandlingsledd | Illustrert nivå, kroner | Beregnet forskjell fra raden over | Hva eksemplet viser |
| --- | ---: | ---: | --- |
| Opprinnelig forslag, «Prop. 1 S» | 1 000 000 000 | Ikke relevant | Regjeringsforslag til nivå. |
| Innstilling, tilråding | 1 100 000 000 | +100 000 000 | Stadiesammenligning med forslaget; ingen vedtatt endring. |
| Opprinnelig endelig vedtak | 1 050 000 000 | −50 000 000 | Stadiesammenligning med tilrådingen; vedtatt nivå holdes separat. |
| Senere RNB-proposisjon | 1 200 000 000 | +150 000 000 | Nivåforskjell mellom behandlingsrunder under eksemplets forutsetning; fortsatt et forslag. |

**Alle tabellverdiene er syntetiske.** I en virkelig RNB-kilde må det undersøkes om 1,2 mrd. kroner er nivå, endring, aggregat eller noe uavklart. Beløpet kan ikke uten kildebevis bli et delta på 1,2 mrd., et vedtatt delta på 150 mill. eller en godkjent saldo på 1,2 mrd. En manglende RNB-innstilling eller et manglende RNB-vedtak skal vises som hull. Illustrasjonen gir ingen kildeprøve for implementering eller faglig godkjenning.

Før-, endrings- og etterobservasjoner i ett dokumentert postledd grupperes som samme hendelse. Forslag, alternative forslag, omtale, kilderettelser, dokumentlenker og beregnede forskjeller øker ikke antallet vedtatte hendelser. En beregnet bevilgning krever et uttrykkelig valgt inngående nivå og kildebelagte vedtatte deltaer i dokumentert rekkefølge. Manglende start, ledd eller kjedekonflikt sperrer godkjent kjedesum; et separat observert beløp kan fortsatt vises med sin egen proveniens.

## Fullstendighet og flere år

«Alle» er et dekningskrav, også når noe ennå ikke er strukturert eller faglig avklart. Dokumentvisningen skal avstemmes mot et uttrykkelig inventar for hele dokumentversjonen, ikke bare mot postene adapteren allerede støtter. Den må skille mellom:

- **Fulltekstkildeinventar:** hvilke originaler, representasjoner, kapitler, poster, tabeller og tekstseksjoner som er bevart, og hvilket omfang som mangler. En delvis HTML-representasjon merkes som delvis selv når full PDF er bevart.
- **Strukturert innhold:** hvilke beløpsfelt, tekstseksjoner og relasjoner som faktisk er gjenfunnet og kildebundet, med synlig ustrukturert, uavklart eller feilet innhold.
- **Faglig avklart innhold:** hvilke verdier og relasjoner som er vurdert for angitt bruk. Teknisk gjenfinning, full kildebevaring og avstemt enkeltbeløp er ikke uttømmende faglig dekning.

Fullmakter, stikkord og tekst uten sikker beløps-/postkobling bevares i dokumentets inventar med riktig rolle; de gjøres ikke til bevilgningsendringer. Filtrering av konto eller år avgrenser den viste delmengden. Den skal ikke skjule globalt kildeinventar, kildefeil, ukjent omfang eller dekningshull. Konto-/årsvisningen må dessuten avstemmes mot et eksplisitt kildeinventar for den valgte perioden, slik at dokumenter som ennå ikke er koblet til en post ikke forsvinner fra dekningskontrollen.

Ved flere budsjettår skal kontokontinuitet ha kilde, gyldighetsperiode og omfang. Omnummerering, oppgaveflytting, deling og sammenslåing skal fremgå når de er dokumentert. Uavklart kontinuitet vises som et brudd eller separate konto-/årsforløp. Like kapittel-/postnumre over år er ikke kontinuitetsbevis, og sesjon kan ikke erstatte budsjettår. Ingen dokumentert enkeltkjede gir automatisk helårs- eller flerårsdekning.

## Akseptkrav for senere implementering

Aksepten skal demonstreres fra bevarte autentiske originaler gjennom kildebundet strukturering og begge inngangene til **skrevet og faktisk gjenlest JSON og Excel**. Syntetiske feilsituasjoner merkes særskilt. Dette er krav til senere leveranser; denne dokumentendringen utfører ingen funksjonstest.

| ID | Observerbart akseptkrav |
| --- | --- |
| V1 | Valg av en dokumentversjon viser hele konto-/beløpsinventaret, relevant omtale og dokumenterte behandlingsforbindelser. Manglende strukturering eller faglig avklaring er synlig for de delene det gjelder. Et smalt pilotutvalg kan ikke merkes som full dokumentvisning. |
| V2 | Valg av flere kapitler/poster og flere budsjettår viser alle berørende dokumenter i det kontrollerte kildeinventaret, med originalt forslag, innstilling, vedtak og senere runder. Utvalgets kilde-/årsdekning og hull fremgår. |
| V3 | Brukeren kan gå dokument → konto/år → samme dokument og konto/år → dokument → samme konto/år. Identiteter, versjoner og kontrollstatus er de samme ved tilbakekomst. |
| V4 | En autentisk forgrening, som de to sakene til Prop. 16 S, bevarer forskjellig kapittelomfang og alle dokumentreferanser. Ingen post arver beløp eller begrunnelse bare fra en felles proposisjon eller sak. |
| V5 | Sammenligning viser kildeobserverte nivåer, uttrykkelige deltaer og beregnede forskjeller separat, med kontrollert omfang og rekkefølge. Et manglende stadium gir hull; det gir verken null eller konstruert vedtak. |
| V6 | En kildebelagt komitéendring og parallelle alternativer har korrekt avsender, rolle og forbindelse til vedtatt resultat. 210-prøven alene oppfyller ikke dette, siden den ikke dokumenterer en slik endring. |
| V7 | Flere år har etterprøvbart gyldighets-/kontinuitetsgrunnlag. En merket syntetisk prøve med like kontonumre og ukjent kontinuitet forblir uavklart. |
| V8 | Faktiske JSON-/Excel-filer gjenleses med samme kilder, originaltekst, lokatorer, beløpsverdier, beløpsbetydning, relasjoner, rolle, beregningsgrunnlag og statuser. Begge inngangene kan rekonstrueres og avstemmes mot samme inventar og beløpsgrunnlag. Lange tekster og kildepekere bevares. |
| V9 | Bytte av inngang, filtre, flere omtaleseksjoner og gjentatt eksport endrer ikke grunnlagets hendelsesantall eller skaper ekstra beløpsobservasjoner. Den autentiske 210-prøvens seks vedtaksbeløpsobservasjoner beskriver fortsatt to posthendelser. Antall i utvalget skilles fra antall i hele grunnlaget. |
| V10 | Manglende, korrupt eller motstridende omtale/historisk Excel hindrer ikke at en autentisk ny offisiell vedtaksprøve oppdages, bevares, lagres og ordinært eksporteres. Tomme kontoresultater beholder globale avvik. Gamle ID-er, kontrollavgjørelser, standardvalg og JSON-/Excel-resultater gjenleses uendret. |

## Modellkonsekvenser og leveransegrense

Modellen må kunne representere dokumenter og representasjoner, saker og behandlingsledd, beløpsobservasjoner, hendelser, omtaleseksjoner, relasjoner og avledede beregninger med separate identiteter, kildebevis og statuser. Begge inngangene må kunne bygges fra dette grunnlaget. Dette er krav til uttrykksevne og etterprøvbarhet, ikke et nytt besluttet lagringsskjema, nye feltnavn eller en migreringsplan. [Observasjonsformatets kompatibilitetsregler](observasjonsformat.md#kompatibilitet-og-videre-bygging) består. Eventuelle kontraktutvidelser krever dokumentert kildebehov, eksplisitt versjon og regresjonsbevis før bygging.

[O2a/#34](https://github.com/depmartin/budsjetthistorikk/issues/34) er levert for det godkjente 210/1429/1-snittet. Leveransen i [PR #36](https://github.com/depmartin/budsjetthistorikk/pull/36), flettet som `6f7145d` 23. oktober, er ikke en generell dokument- eller årsvisning. [O2b/#35](https://github.com/depmartin/budsjetthistorikk/issues/35) er levert i [PR #39](https://github.com/depmartin/budsjetthistorikk/pull/39), main `5423160`, med [kontrollgrunnlag](research/omtale-o2b/README.md). Den er fortsatt en pilot for to posthendelser i 2024 og skal ikke utvides til de to generelle inngangene ved å lese dette målbildet inn i pilotens aksept. O3–O5 er fortsatt foreslåtte senere spor med egne kilde-/omfangsavklaringer.

Oppfølgingen under [#37 – Konkretiser dokumentvisning og kapittel-/postvisning med sammenligning av behandlingsledd](https://github.com/depmartin/budsjetthistorikk/issues/37) har nå et [konkret forslag](visningspilot-plan.md), [bevart kildegrunnlag](research/to-visninger-37/README.md), [testmatrise](research/to-visninger-37/testmatrise.md) og [ticketutkast](research/to-visninger-37/tickets/README.md). Første anbefaling er hele Innst. 81 S gjennom begge innganger. En faktisk komitéendring, den andre proposisjonsgrenen og avgrensede konto-/årsutvalg er kildekontrollert; positivt tallfestet alternativ, kontokontinuitet og full årsdekning har åpne kildeporter. Forslaget legges frem før publisering av byggetickets og implementering. #1, #32, #10 og #13 er kravkontekst og separate rester; de skal ikke lukkes for å gjennomføre et senere godkjent snitt. #34/#35 er levert, men leveransen er ikke ny faglig godkjenning eller generell visningsaksept.

Nye offisielle vedtak skal alltid kunne registreres fra egen kilde uavhengig av de to visningene, omtale og historisk Excel. #10 forblir åpen for faktisk driftsaksept. Denne presiseringen endrer ikke driftsmandat eller faglig godkjenning av historiske tall.
