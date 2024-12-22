[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/pKHO5ZJl)

# README: Proof of Concept Umbraco Website

## Overzicht
Dit project is een Proof of Concept (PoC) voor een website gebouwd met Umbraco CMS. Het doel is om de mogelijkheden en beperkingen van Umbraco te evalueren voor toekomstige implementaties.

## Doelen van het project
1. **Onderzoeken van Umbraco-functionaliteiten:** Evalueren van contentbeheer, templates, en extensiemogelijkheden.
2. **Integratie testen:** Controleren of Umbraco kan worden geïntegreerd met andere systemen en API's.
3. **Prestaties evalueren:** Testen van de snelheid en schaalbaarheid van de Umbraco-omgeving.
4. **Proof of concept presenteren:** Demonstreren van de belangrijkste functies aan belanghebbenden.

---

## Installatie
Volg de onderstaande stappen om het project lokaal op te zetten:

### Vereisten
- **Umbraco versie:** 12+ (of een versie volgens projectbehoefte)
- **.NET versie:** 6 of hoger
- **Database:** SQL Server of SQLite (voor PoC-doeleinden)
- **Node.js:** (optioneel voor frontend-builds)

### Installatie stappen
1. **Clone de repository:**
   ```bash
   git clone https://github.com/pgm-2425-itexploration/meetup-1-PGM-mattcecc.git
   cd umbraco-poc
   ```
2. **Herstel NuGet-pakketten:**
   ```bash
   dotnet restore
   ```
3. **Database configureren:**
   - Wijzig de verbindingstring in `appsettings.json`:
     ```json
     "ConnectionStrings": {
       "umbracoDbDSN": "Server=localhost;Database=UmbracoPoC;User Id=sa;Password=YourPassword;"
     }
     ```
4. **Start de applicatie:**
   ```bash
   dotnet run
   ```
5. **Toegang tot de Umbraco-backend:**
   - Open [http://localhost:44341](http://localhost:44341)
   - Log in met de opgegeven beheerdersgegevens.
---

## Belangrijkste functionaliteiten
- **Contentbeheer:** Dynamische pagina's maken en bewerken via het CMS.
- **Templates:** Aanpasbare ontwerpen met behulp van Razor-sjablonen.
- **Mogelijkheden voor extensie:** Gebruik van Umbraco-pakketten en API-integraties.

---

## Structuur van het project
```
- /Controllers      : Backend-logica
- /Models           : Gegevensmodellen
- /Views            : Razor-templates
- /wwwroot          : Statische bestanden
- appsettings.json  : Configuratiebestand
```

---

## Testen
### Handmatige tests
1. Controleer of nieuwe pagina's kunnen worden gemaakt in de backend.
2. Test API-integraties door dummy-gegevens te importeren.
3. Controleer de snelheid van paginalading in verschillende browsers.

### Automatische tests
Voer de volgende opdracht uit voor unit tests:
```bash
dotnet test
```
---

## Toekomstige verbeteringen
- Integratie met externe systemen zoals een CRM.
- Optimalisatie voor mobiele apparaten.
- Uitbreiden van de CMS-functionaliteit met aangepaste pakketten.

---
