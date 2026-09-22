# Reinteller – automatisk telling fra flyfoto

Et enkelt, selvstendig undervisningsverktøy som demonstrerer hvordan bildeanalyse kan brukes til å telle rein i fly- og dronebilder.

Verktøyet kjører direkte i nettleseren og krever ingen server, database eller installasjon. Det er laget for **demonstrasjon av metode i undervisning**, ikke som et validert verktøy for bestandsestimering eller forvaltningsbeslutninger.

## Kom i gang

1. Åpne `index.html` direkte i en moderne nettleser, eller publiser mappen med GitHub Pages.
2. Last inn et JPG-, PNG- eller WebP-bilde.
3. Velg analysemetode eller bruk **Automatisk**.
4. Juster tersklene ved behov.
5. Klikk på markeringer for å deaktivere eller aktivere enkeltfunn manuelt.
6. Lagre bildet med markeringer dersom du ønsker dokumentasjon av resultatet.

## Analysemetoder

- **Automatisk:** forsøker først å finne røde markeringer og går ellers over til enkel råfotoanalyse.
- **Røde markeringer / annotert bilde:** teller røde markører i et allerede annotert bilde.
- **Mørke objekter på lys snø:** finner sammenhengende mørke objekter på lys bakgrunn basert på terskler for mørkhet og objektstørrelse.

Råfotoanalysen er klassisk bildebehandling, ikke en ferdigtrent AI-modell. Stein, vegetasjon, skygger og dyr som står tett kan derfor føre til feilklassifiseringer.

## Faglig bakgrunn

Undervisningsdelen i programmet er inspirert av forskning på bruk av UAV-bilder til telling av svalbardrein:

> Paulsen, I. M. G., Pedersen, Å. Ø., Hann, R., Blanchet, M.-A., Eischeid, I., van Hazendonk, C., Ravolainen, V. T., Stien, A., & Le Moullec, M. (2023). *How Many Reindeer? UAV Surveys as an Alternative to Helicopter or Ground Surveys for Estimating Population Abundance in Open Landscapes*. Remote Sensing, 15(1), 9. https://doi.org/10.3390/rs15010009

Artikkelen viser blant annet at deteksjon fra UAV-bilder kan være ufullstendig, at bildeegenskaper og bakgrunn påvirker hvor lett rein oppdages, og at automatisert objektgjenkjenning med maskinlæring er en relevant videre utviklingsretning.

## Publisering med GitHub Pages

1. Opprett et nytt GitHub-repository.
2. Last opp innholdet i denne mappen til roten av repositoryet.
3. Gå til **Settings → Pages**.
4. Velg **Deploy from a branch**.
5. Velg `main` og mappen `/ (root)`.
6. Lagre. GitHub viser deretter adressen til nettsiden når publiseringen er klar.

`index.html` er selvstendig og inneholder både eksempelfoto og logo innebygd som data. Det er derfor ingen eksterne filer som må lastes sammen med nettsiden for at selve demonstrasjonen skal fungere.

## Nettleserstøtte

En oppdatert versjon av Chrome, Edge, Firefox eller Safari anbefales. HEIC-bilder støttes ikke nødvendigvis direkte av nettleseren; konverter i så fall bildet til JPG eller PNG først.

## Lisens og fri bruk

Prosjektet er **åpent for alle** og kildekoden distribueres under **MIT-lisensen**. Det betyr at du kan bruke, kopiere, endre, publisere og bygge videre på programmet, også i andre prosjekter, så lenge copyright- og lisensinformasjonen følger med.

NMBU-logoen er tredjepartsinnhold og omfattes ikke av MIT-lisensen. Se `COPYRIGHT.md` for detaljer om logo, eksempelfoto og forskningsartikkel.

## Kreditering

**Laget av Ronny Steen**  
**Skyggekoding (ghost coding): ChatGPT**

Krediteringen er ment som åpen dokumentasjon av hvordan demonstratoren ble utviklet. Se `LICENSE` for programvarelisensen og `COPYRIGHT.md` for merknader om tredjepartsinnhold.
