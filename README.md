## KundeApp

KundeApp er en .NET Core-basert applikasjon designet for å håndtere kundeinformasjon.
Denne applikasjonen gir mulighet til å administrere kundeprofiler, gjennomføre CRUD-operasjoner (Create, Read, Update, Delete),og utføre enkel dataanalyse på kundedataene.
Applikasjonen er utviklet med en lagdelt arkitektur som separerer logikk, dataadgang og brukergrensesnitt.
Med denne applikasjonen kan du lagre all viktig informasjon om kundene dine på ett sted.
Du kan raskt finne frem til en kunde, oppdatere informasjonen deres, legge til nye kunder, eller slette kunder som ikke lenger er aktuelle.
I tillegg så kan kunden lage sin egen profil med brukernavn og passord, for å logge inn og ut.

## Funksjonalitet
Kundeadministrasjon: Opprette, lese, oppdatere og slette kundedata.
Databaselagring: Bruker en SQLite-database (Kunde.db) for å lagre kundeinformasjon.
Logger: Opprettholder logger for systemaktiviteter i Logs-mappen.
Testdekning: Inneholder enhetstester (KundeAppTest.cs) for å sikre kvalitet og pålitelighet i koden.
Konfigurasjon: Applikasjonen støtter ulike miljøer ved hjelp av appsettings.json-filer.

## Prosjektstruktur
Controllers: Inneholder kontrollere som håndterer HTTP-forespørsler og styrer flyten i applikasjonen.
DAL (Data Access Layer): Håndterer interaksjon med databasen, inkludert CRUD-operasjoner.
Model: Definerer de ulike dataobjektene som brukes i applikasjonen, inkludert kundeentiteter.
Views: Inneholder visningsfiler for brukergrensesnittet (ligger under wwwroot).
KundeApp2.csproj: Prosjektfilen for applikasjonen.
Startup.cs: Konfigurerer applikasjonen ved oppstart, inkludert avhengighetsinjeksjon og middleware.
Program.cs: Inngangspunktet for applikasjonen.
appsettings.json: Konfigurasjonsfiler for forskjellige miljøer (produksjon, utvikling, etc.).

## Testing
Prosjektet inneholder enhetstester som kan kjøres ved hjelp av XUnit.
