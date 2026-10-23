# Forslag: to visninger gjennom et avgrenset kildegrunnlag

Status: konkretiseringsforslag under [#37](https://github.com/depmartin/budsjetthistorikk/issues/37), 23. oktober 2026. Forslaget legges frem før publisering av byggetickets og implementering. [Målbildet og V1–V10](to-visninger.md) er bekreftede krav; avgrensningen og oppdelingen her er foreslått. O2b er levert i [PR #39](https://github.com/depmartin/budsjetthistorikk/pull/39), main `5423160`. Den leveransen er en omtaleprøve, ikke de to generelle visningene.

## Problemet som første snitt løser

Brukeren skal kunne åpne et helt dokument og gå videre til en berørt konto, eller velge konto og år og gå videre til dokumentene. Begge veier skal vise de samme kildeopplysningene og bevare hele dokumentets inventar. Dagens postomtale kan ikke brukes som om den allerede importerte alle forslagstall eller hele dokumentet.

Første foreslåtte leveranse er en lokal, eksplisitt valgt JSON-/Excel-pilot. Den følger den etablerte arbeidsflaten og krever ingen ny søketjeneste, nettapplikasjon eller skyressurs. Et senere interaktivt grensesnitt kan bruke samme grunnlag. Piloten skal kunne demonstreres fra bevarte originaler gjennom begge innganger til faktisk gjenleste filer.

## Første dokument og konto-/årsutvalg

Det første komplette dokumentet foreslås å være **hele Innst. 81 S (2024–2025)**, med forbindelsen til vedtak 210 og 211 og den relevante delen av Prop. 16 S. Budsjettåret er **2024**. Post 1 og 22 har bevilgningsendringer; post 60 har fullmakts-/tekstinnhold. Alle tre postene skal være med i dokumentinventaret. Post 60 skal kunne velges som konto uten å bli en tredje bevilgningshendelse.

Prop. 16 S bevares som hel original med et uttrykkelig helinventar, men dens strukturerte 1429-utvalg merkes som delvis dokumentdekning. Første leveranse skal gi hele Innst. 81 S, ikke fremstille 1429-utvalget som en full strukturering av Prop. 16 S. Forgreningen til Innst. 95 S vises med dokumentert omfang og synlig status for ennå ikke strukturert innhold.

Kildegrunnlaget, dekningsgrensene og senere kandidater er samlet i [kildeundersøkelsen](research/to-visninger-37/README.md). [Testmatrisen](research/to-visninger-37/testmatrise.md) angir forventede resultater og hvilke som bare gjelder senere snitt. [Ticketutkastene](research/to-visninger-37/tickets/README.md) skiller startbart forslag fra leveranser med en gjenstående kildeport.

## Slik brukes de to inngangene

### Dokumentvisning

Velg en eksakt dokumentversjon. Vis dokumenttype, nummer, sesjon, dokumentdato, kildeversjon og dekning før konto-/beløpsoversikten. Oversikten viser alle inventerte kapitler/poster, med kildeobserverte beløp og egen beløpsbetydning, tekst/fullmakt, relevant omtale, avsender, relasjon og kontrollstatus. Ustrukturert innhold har kildepeker og tydelig status.

Fra en post åpnes konto-/årsforløpet på samme kildegrunnlag. Fra dokumentet åpnes også dokumenterte forgjengere og etterfølgere. En forgrening viser hvilken del av kapitlene/postene hver forbindelse gjelder. Å åpne en tilknyttet proposisjon gir hele dens inventar og dekningsstatus; navigasjonen skjuler ikke de øvrige postene bak det opprinnelige kontofilteret.

### Konto-/årsvisning

Velg hele kapitler og/eller uttrykkelige kapittel/post-par, sammen med ett eller flere budsjettår. Vis unionen av valgte kontoer innen valgte år. Valg av to konkrete par skal ikke utvides til et utilsiktet kryssprodukt av kapittel- og postlistene. Dette er semantikk i den nye inngangen; gamle B6-filtre beholder sin betydning.

Hver kildebelagt behandlingsrad viser konto, budsjettår, runde, dokument, rolle, dokument-/vedtaksdato og rekkefølge, nivå/før/endring/etter som egne opplysninger, omtale og kontrollstatus. Flere beløpsfelt i samme ledd grupperes visuelt; observasjonenes egne identiteter beholdes i kontrollgrunnlaget. Kjent dokument uten verifisert posttilknytning blir et synlig dekningshull, ikke et konstruert treff eller en skjult kilde.

Fra et ledd åpnes den samme dokumentversjonen som beløpet og teksten kom fra. Tilbake til konto-/årsvisningen beholdes kontoer, år, kildegrunnlag og statuser. JSON bevarer de samme identitetsreferansene som brukes av Excel-lenker og filtrerbare ark. Filene skal kunne gjenleses uten nett eller opprinnelig database.

## Sammenligning og behandlingsrekkefølge

Regjeringens forslag, komiteens gjengivelse, tilråding, alternativer og Stortingets vedtak er forskjellige roller. Sammenligning krever eksakte inngangsobservasjoner og kildebevis for samme konto, budsjettår, beløpsbetydning, enhet, detaljeringsnivå og omfang. Talltype og forslagsrolle fremgår for hvert inngangsbeløp. Forskjellen beregnes bare når grunnlaget er sammenlignbart.

En stadieforskjell binder begge dokument-/observasjonsidentitetene, regelen, det kontrollerte omfanget og resultatets status. Den er en separat avledet opplysning. Den blir verken et vedtatt delta eller et nytt ledd i en bevilgningskjede. Sammenligning av to kildeobserverte endringsforslag er noe annet enn sammenligning av nivåer. Mindretallsforslag vises parallelt med tilrådingen.

Manglende ledd gir et navngitt hull med kilde-/inventargrunnlag. Samme beløp er ikke bevis for at forslaget ble vedtatt. Dato og eksplisitt behandlingsbevis bestemmer rekkefølgen; budsjettår, sesjon, dokumentdato, vedtaksdato og hentetid beholdes adskilt. RNB og nysaldering er nye runder, ikke stadier som automatisk kan trekkes fra et tidligere forslag.

De eldre 210-observasjonenes `round='uavklart'` skal bestå. Nysalderingskontekst må eventuelt bindes separat med kildebelegg, egen versjon og synlig status i det nye sammenligningsgrunnlaget. Den er ikke en stilltiende rettelse av gammel tolkning eller en ny B5-avgjørelse. Uavklart sammenligningsgrunnlag gir ingen beregnet differanse.

## Dekning og flere år

Tre nivåer vises hver for seg: bevarte originaler/helinventar, faktisk strukturert innhold og faglig avklart bruk. Et komplett inventar over en avgrenset innstilling beviser ikke komplett årsdekning. Periodens kildeinventar må også vise dokumenter som ennå ikke er postkoblet. Konto-/årsfilteret avgrenser visningen, ikke globale avvik eller dokumentenes dekningsregnskap.

Flerårsutvalg kan vise flere separate konto-/årsforløp. Positiv kontokontinuitet krever kildebelegg, gyldighet og omfang; likt nummer eller navn gir ingen automatisk sammenslåing. Ukjent kontinuitet vises som et brudd. En dokumentert flytting kan bare koble det belagte oppgave-/postomfanget. Hver års-/kontokjede har egen status for inngående nivå, senere ledd, rekkefølge og konflikter. Godkjent årssaldo er ingen leveranse i det første snittet.

## Foreslått kompatibilitetsgrense

Nye forslags- og innstillingsobservasjoner får separate adaptere og identiteter etter [observasjonsformatet](observasjonsformat.md). De legges ikke inn som vedtaksobservasjoner i B1/B2. Vedtatte observasjoner/hendelser gjenbrukes fra det uttrykkelig valgte grunnlaget. Repriser, kilderettelser, alternative forslag, representasjonslenker og navigasjon oppretter ikke nye vedtatte hendelser.

Det foreslås en **ny opt-in eksportkonvolutt**, foreløpig kalt `visningspilot-1`, for dokumentinventar, nye kildeobservasjoner, forbindelser, sammenligninger, utvalg og dekning. Dette er et formatforslag, ikke et implementert eller besluttet skjema. Før kode i første ticket skal felt-/identitetskontrakten fastsettes og dokumenteres innen godkjent snitt. Gamle B6/B8- og `omtale-pilot-1`-filer bevares med egne lesere og uendrede data; nye felt presses ikke inn i gamle lukkede konvolutter.

Hovedschema 5, gamle kildebyte, ID-er, parser-/tolkningsbetydning, B5-avgjørelser, B7-standardvalg, frozen-v1/v2 og tidligere JSON-/Excel-resultater bevares. Den nye piloten skriver nye filnavn og egne ark. B9s gamle 13-kolonners Historikk beholder sin betydning. Ingen lagringsmigrering eller ny generell plattform er nødvendig for å prøve første snitt.

Innlesning eier kildebevaring og sporbar strukturering; analyse eier utvalg, sammenligning og visning. En manglende/feilet/korrupt/motstridende ny adapter, omtale eller historisk fil skal kunne gi globale visningsavvik uten å hindre oppdagelse, bevaring, lagring eller ordinær eksport av et nytt offisielt vedtak. #10 forblir åpen for faktisk driftsaksept.

## Aksept og neste beslutning

Samme samlede grense gjelder hver byggeticket: **bevart autentisk original → kildebundet beløp/omtale → dokumentert relasjon → begge innganger → skrevet og faktisk gjenlest JSON og Excel**. Intern objektkontroll og fil-eksistens er utilstrekkelig. Begge inngangene avstemmes mot samme globale inventar og nøyaktig samme utvalgte observasjoner/hendelser. Syntetiske feilprøver merkes og holdes atskilt fra autentisk fasit.

De konkrete forventningene står i [testmatrisen](research/to-visninger-37/testmatrise.md). Hvert ticketutkast peker til sine matriserader og kilder, leverer et komplett kontrollerbart snitt og har bare faktiske blokkeringer. Ny kildeundersøkelse er en egen kunnskapsleveranse der nødvendig bevis mangler; en slik port skal ikke blokkere første snitt som allerede har tilstrekkelig kildegrunnlag.

Forslaget legges samlet frem for eieren. Publisering av byggetickets og funksjonsbygging følger et senere mandat. Denne konkretiseringen endrer dokumentasjon og kildebevis; den implementerer ingen ny visning eller eksportleser.
