# Introduksjon til JSON

JSON står for **JavaScript Object Notation**, og er en måte å lagre objekter som skal brukes i JavaScript. Det at dataen skilles fra koden gjør det enklere å endre og vedlikeholde data som brukes av en applikasjon eller webside. Dette ligner litt på å bruke Firebase eller andre NoSQL-databaser, men forskjellen er at JSON-data kan lagres lokalt, i samme mappe som websiden.

Data i en JSON-fil har en spesifikk syntaks, som du kan lese om på W3schools: [JavaScript JSON (w3schools.com)](https://www.w3schools.com/js/js_json.asp).

I denne innleveringen skal du øve på å bruke JSON og importere JSON-data til en nettside. 

## Oppgave 1: Data om høyeste fjell i hvert fylke
Lag en fil som heter **fjelltopper.json**. Denne skal inneholde en array med objekter. Hvert objekt skal inneholde navnet på et fylke, navn på høyeste fjelltopp i det fylket, og høyden på fjelltoppen. Du finner en liste med de høyeste fjelltoppene i hvert fylke på Peakbook: [Fylkestopper (norge) (peakbook.org)](https://peakbook.org/index.php?module=index.lists.view&pbeItem=1&id=1400).

En mal for filen **fjelltopper.json** finner du vedlagt i dette repositoriet.

## Oppgave 2: List ut fjelltoppene på en webside
Lag en webside som bruker dataen fra JSON-filen for å liste opp de høyeste fjelltoppene i hvert fylke. Du kan skrive ut som en tabell eller som en liste. 

For å importere dataen fra JSON-filen, kan du bruke denne koden:
```javascript
import data from "./fjelltopper.json" assert { type: "json" };
```
Denne koden både importerer JSON-dataen, og gjør den om (parse) til JavaScript-data. Du trenger derfor ikke å bruke metoden `JSON.parse()` som er beskrevet på w3schools. 

Dataen blir importert som en array med objekter, kalt `data`. Du må derfor bruke en for-løkke for når du skal skrive ut dataen på websiden.

En mal for websiden finner du vedlagt i dette repositoriet som **index.html**.

## Oppgave 3: Sortering av data
Sorter listen over fjelltopper etter høyde, fra høyest til lavest. 

For å få hjelp til dette kan du se video og forklaring på denne siden: [How to sort an array of objects by a property value in JavaScript (flaviocopes.com)](https://flaviocopes.com/how-to-sort-array-of-objects-by-property-javascript/).

Du kan lese mer om sortering av arrays på W3schools: [JavaScript Sorting Arrays (w3schools.com)](https://www.w3schools.com/js/js_array_sort.asp).
