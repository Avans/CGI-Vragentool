# Criteriumgericht Interview Tool - Gebruikershandleiding

## Doel van de tool
Deze tool is ontworpen om het proces van criteriumgerichte interviews te ondersteunen. Het stelt interviewers in staat om op een gestructureerde manier vragen te stellen, antwoorden te scoren en een samenvatting van de resultaten te genereren. De tool is gebaseerd op een Excel-bestand dat de vragen en antwoordmogelijkheden bevat.

De tool is specifiek te gebruiken om holistische rubrics in Brightspace efficiënt te vullen. Per regel in de rubric heb je een categorie in je excel. Hier zitten subcategorieën in, maar dat zijn eigenlijk bullets in die brightspace rubric regel. Hierdoor weet je dat je de volledige dekking van de rubric regel hebt.

## Hoe te gebruiken

### 1. Excel-bestand voorbereiden
Voordat je de tool kunt gebruiken, moet je een Excel-bestand voorbereiden met de vragen voor het interview. De structuur van dit bestand is cruciaal voor de goede werking van de tool. Zie de sectie [Structuur van het Excel-bestand](#structuur-van-het-excel-bestand) voor gedetailleerde instructies.

Elk werkblad in het Excel-bestand wordt een apart tabblad in de tool. Dit is handig om bijvoorbeeld interviews voor verschillende functies of competentiesets te scheiden.

### 2. Interview starten
1.  Open het `CGI-tool.html` bestand in je webbrowser.
2.  Klik op de knop "Selecteer een interviewbestand (Excel)" en kies het voorbereide Excel-bestand.
3.  De tool verwerkt het bestand en toont de interviewvragen, gegroepeerd per categorie en subcategorie.

### 3. Interview afnemen
-   **Navigeren:** De vragen zijn georganiseerd in tabbladen (overeenkomend met de werkbladen in je Excel-bestand). Binnen een tabblad zijn de vragen gegroepeerd per categorie en subcategorie. Je kunt de subcategorieën openen en sluiten door erop te klikken.
-   **Vragen wisselen:** Binnen een subcategorie wordt willekeurig een vraag getoond. Gebruik de knoppen "Vorige vraag" en "Volgende vraag" om door de vragen van die subcategorie te bladeren.
-   **Antwoord selecteren:** Klik op een van de oordeelknoppen ('Uitmuntend', 'Goed', 'Voldoende', 'Onvoldoende', 'Slecht') om het antwoord van de kandidaat te scoren. Een geselecteerd antwoord krijgt een duidelijke markering. Je kunt je keuze wijzigen door op een ander oordeel te klikken, of de selectie ongedaan maken door nogmaals op het geselecteerde oordeel te klikken.
-   **Toelichting toevoegen:** Onder elke vraag is een tekstveld beschikbaar om een toelichting of specifieke voorbeelden (volgens de STARR-methode, bijvoorbeeld) te noteren. Deze toelichting wordt meegenomen in de resultaten.

### 4. Resultaten
-   Onderaan de pagina vind je de sectie "Resultaten". Voor elke hoofdcategorie wordt een samenvatting gegenereerd.
-   **Gemiddeld Advies:** Per categorie wordt een gemiddeld advies berekend op basis van de gegeven scores. Dit geeft een snelle indicatie van de prestatie van de kandidaat binnen die categorie.
-   **Tekstvak met resultaten:** Alle geselecteerde antwoorden en de bijbehorende toelichtingen worden per categorie verzameld in een tekstvak.
-   **Kopiëren:** Je kunt de resultaten van een categorie eenvoudig naar het klembord kopiëren met de kopieerknop naast de categorietitel.

Je kan op basis van dit advies de juiste kolom in Brightspace aanvinken. Plak dan de tekst uit de output in Brightspace zodat studenten hun feedback kwalitatief ontvangen.

### 5. Resultaten afdrukken
Je kunt de resultaten afdrukken via de printfunctionaliteit van je browser (Ctrl+P of Cmd+P). De tool heeft een speciale print-layout die alleen de relevante informatie toont:
-   Alleen vragen waar een antwoord is geselecteerd, worden getoond.
-   Niet-geselecteerde antwoordopties worden verborgen.
-   Navigatie-elementen en knoppen zijn verborgen.
-   De genoteerde toelichtingen worden volledig weergegeven.

Hiermee kan je, voor je eigen administratie, de resultaten bewaren.

### 6. Interview resetten
Met de knop "Interview Resetten" (bovenaan en onderaan de pagina) kun je de volledige status van het huidige interview wissen. Alle geselecteerde antwoorden en toelichtingen worden verwijderd, en de tool toont weer willekeurige startvragen. Dit is handig wanneer je een interview met een nieuwe kandidaat start.

## Structuur van het Excel-bestand
De tool verwacht een specifieke opmaak van het Excel-bestand. Elk werkblad (sheet) in je Excel-bestand wordt als een apart tabblad in de tool weergegeven.

### Kolommen
Je Excel-werkblad moet de volgende kolommen bevatten:

1.  **Categorie:** De hoofdcategorie van de vraag (bv. "Technische Vaardigheden", "Communicatie").
2.  **Subcategorie:** Een onderverdeling binnen de hoofdcategorie (bv. "Programmeren in Python", "Presentatievaardigheden").
3.  **Vraag:** De concrete interviewvraag die gesteld moet worden.
4.  **Uitmuntend:** De beschrijving van een uitmuntend antwoord.
5.  **Goed:** De beschrijving van een goed antwoord.
6.  **Voldoende:** De beschrijving van een voldoende antwoord.
7.  **Onvoldoende:** De beschrijving van een onvoldoende antwoord.
8.  **Slecht:** De beschrijving van een slecht antwoord.

**Belangrijk:**
- De kolomnamen moeten exact overeenkomen met de bovenstaande lijst.
- Als een vraag niet voor alle oordeelsniveaus een beschrijving heeft, kun je de cel voor dat niveau leeg laten. De knop voor dat oordeel wordt dan niet getoond voor die specifieke vraag.
- Rijen waar de kolom 'Vraag' leeg is, worden genegeerd.
- De tool groepeert vragen automatisch op basis van de waarden in de kolommen 'Categorie' en 'Subcategorie'. Zorg ervoor dat je deze consistent spelt.