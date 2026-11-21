# Machinery

Machinery (tidligere Maskindagbok) er en enkel maskindagbok for mobil. Ingen innlogging – alt lagres på telefonen og virker uten nett.

**Åpne appen:** https://krissalt.github.io/Maskindagbok/

Legg den på hjemskjermen: åpne lenken på mobilen → meny → «Installer app» / «Legg til på startsiden».

## Funksjoner
- Dagbok som forside, med dato og klokkeslett, gruppert per dag
- Hurtigknapper: fylt olje, hendelse, vedlikehold, service – lagres med ett trykk, fyll inn senere
- «Neste dag» fører maskinrunde kl. 07:00, følger turnusen (dag 1 av 14 osv.)
- Maskiner med timeteller og jobber etter kjøretimer (Scania-generatorene og John Deere fra CCOM)
- Varselbjelle for jobber som er forfalt eller forfaller snart (10 % av intervallet ≥ 500 t, ellers 20 %)
- «✓ Utført» på jobb – husker det du skrev som knapper til neste gang
- Sikkerhetskopi (JSON) og eksport til CSV/Excel

## Ny versjon
1. Legg til en ny oppføring øverst i `changelog.js` (versjonsnummer, dato, hva som er endret). Appen viser det øverste nummeret.
2. Sett samme nummer i `VERSION` øverst i `sw.js`, så telefonen henter den nye versjonen. `sw.js` må aldri være tom – da virker ikke appen uten nett.
