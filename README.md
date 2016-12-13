# eksempelkart

## Oppgaver

### Oppgave 1 - komme i gang

* Klon eller fork+klon dette prosjektet slik at du får en kopi på egen harddisk.
* Åpne `index.html` (fra lokal disk) i Firefox eller Chrome og `style.json` i en teksteditor.
* Se på kartet og skumles filene.

### Oppgave 2 - stops

Bruk [Mapbox Style Specification](https://www.mapbox.com/mapbox-gl-style-spec/) og endre slik at dybdekurver (`DEPCNT`) slik at den blir litt tykkere når man zoomer inn. Hint: prøv med `stops`. Kan en diskret forskjell være bedre enn samme tykkelse hele veien?

### Oppgave 3 - roterte symboler med data-driven styling

Se på `S52_SYMBOL_135`. Den takler kun symboler rotert til 135 grader, men med [data-driven styling](https://www.mapbox.com/help/gl-dds-ref/) kan den endres til `S52_SYMBOL_ROTATE` og så heller bruke egenskapen `ROTATE`. Prøv det og se om det virker med `RCTLPT` rest vest for Mortavika-Arsvågen.

Roteringen stemmer ikke helt pga projeksjon. Det bør kanskje løses ved å introdusere en `ROTATE_CRS` som gjør om rotasjonsverdien fra storsirkel til skjerm for det aktuelle stedet og den aktuelle projeksjonen.

NB: [data-driven styling](https://www.mapbox.com/help/gl-dds-ref/) virker dessverre foreløpig kun på JS, ikke Native (iOS + Android).
