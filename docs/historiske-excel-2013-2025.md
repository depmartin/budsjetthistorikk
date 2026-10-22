# Historiske Excel-data 2013–2025 – kildeobservasjoner

Status: innledende inspeksjon 20.10.2026. Observasjoner er ikke en godkjent tolkning av beløp eller komplett datavalidering.

## Filinventar
Kilden er `Samlet_inputdata_2013_2025.zip`, med 13 Excel-arbeidsbøker: `YYYY_samlet_inputdata.xlsx` for alle budsjettår 2013–2025. Hver bok har to ark og ingen ekstra filer i arkivet. Arkene har ca. 1 800–2 000 rader for rådata og ca. 1 000–1 860 rader for dokumenttilknytning (inkludert overskrifter). Bevar arbeidsbøkene byteidentisk og registrer SHA-256 for hver fil ved import.

## Ark og kolonner
- Rådataarket heter `Rådata` i 2013–2024 og `Rådata2025` i 2025. Det har 14 kolonner: `Dep`, `Kap`, `Post`, `Upost`, `Kapnavn`, `Postnavn`, `Gul bok (f90)`, `Saldert (f120)`, `Endring RNB-prop (f148)`, `Budsjettets stilling ink. RNB (f150)`, `Tilleggsbevilgninger første halvår (f176)`, `Tilleggsbevilgninger etter RNB (f177)`, `Lønnsoppgjør (f179)`, `Nysald-prop`.
- Dokumentarket heter `DokumentiltknyntningYYYY` (merk skrivemåten) og har 15 kolonner: `kap_nr`, `post_nr`, `upost_nr`, `belop`, `doknr10`, `doknr20`, `doknr30`, `post_navn`, `stikkord`, `kap_navn`, `gdep_nr`, `fdep_nr`, `omr_nr`, `kat_nr`, `gdep_navn`.

## Tolkning og risikoer
- `Rådata` har flere budsjettstadier. Ikke summer kolonnene ukritisk: noen er nivåer, andre endringer. `Gul bok` er forslag og `Saldert` et annet stadium; ingen av dem er regnskap.
- Beløpsenhet MÅ avklares med uavhengig kilde. Eksempel fra 2013: kapittel 1 post 1 har `10.032` i rådata, mens dokumentarket har beløp som `2000000`. Dette kan indikere ulike enheter (f.eks. tusen kroner vs. kroner), men er ikke verifisert. Ikke multipliser automatisk før kontroll.
- Underpost `Upost` / `upost_nr` er en del av identiteten. Posttotal og underpost må ikke dobbeltelles.
- Dokumentarket har både positive og negative `belop` og dokumentreferanser som `p146/24-25` og `i540/24-25`. Ikke anta at hver rad er et unikt endelig stortingsvedtak; dokumentkoder og eventuelle summeringer må tolkes og kontrolleres.
- Skill `Dep`, `fdep_nr` og `gdep_nr`. Gul bok-gruppering er ikke nødvendigvis administrativ departementstilknytning; historisk tilknytning må være årsspesifikk.
- Dokumentkoder kan vise sesjoner som ikke er identiske med budsjettåret (f.eks. dokumentkode 25-26 i 2025-arket). Bevar kildestrengen ordrett og undersøk årsaken før kronologisk modellering.
- Manglende verdi er ikke null; negative tall kan være gyldige. Bevar radnummer, ark, filhash og originalverdi for sporbarhet.
- Klassifiser inntekts-/utgiftskapitler etter kapittelnummer, ikke beløpets fortegn. Se `docs/krav.md` og `GLOSSARY.md`.

## Forslag til gjennomføring
1. Kontroller publiserbarhet: repositoryet er offentlig. Ikke legg ut originalfilene før dette er avklart.
2. Legg originaler i `data/historisk/original/` og lag kildeinventar med filnavn, budsjettår, hash, ark, kildestatus og dato.
3. Bygg separat historisk Excel-adapter under `innlesning/`, uten å endre eksisterende B1-kontrakt.
4. Importer råobservasjoner med kildeidentitet, beløpsenhet, stadium, underpost og kontrollstatus. Uavklart tolkning skal ikke inngå i godkjente analysetall.
5. Test årdekning, overskrifter, datatyper, duplikater, fortegn, sumkontroller, underposter og avstemming mot uavhengig kilde. Tilby analyseeksport først etter kontroll.

Relatert: issue #13. Dette dokumentet er en varig kildeobservasjon, ikke godkjenning av tallgrunnlaget.
