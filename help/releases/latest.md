---
title: De huidige Mix Modeler-releaseopmerkingen weergeven
description: Opmerkingen bij de nieuwste Mix Modeler-release
feature-set: Experience Cloud
feature: Release Notes
exl-id: 38a47672-2af2-437c-b769-4d5febb941f5
source-git-commit: 7581053507bd1a6a07b2f3853f454631ecee8cec
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Opmerkingen bij de release van Mix Modeler

**Laatste update**: 26 februari, 2026.

Deze releaseopmerkingen betreffen de meest recente release van Mix Modeler. Mix Modeler-releases werken op een doorlopend leveringsmodel, dat een gemiddelde maandelijkse release mogelijk maakt. Deze releaseopmerkingen worden daarom regelmatig bijgewerkt.

## februari 2026

| Functie | Beschrijving | [ Begin van de Uitvoer ](#release-strategy) | [ Algemene Beschikbaarheid ](#release-strategy) |
|---|---|---|---|
| **Geharmoniseerde factorenwerkschema** | De factoren worden nu beheerd als deel van a [ geharmoniseerde het factorenwerkschema ](/help/harmonize-data/overview.md#factors). Dit vereenvoudigt hoe te [ factorgegevens ](/help/ingest-data/schemas.md#factor-standard-fields-field-group) bepalen, hoe te [ interne en externe factoren als deel van uw datasetregels ](/help/harmonize-data/dataset-rules.md#factor-datasets) beheren, en hoe te om factorgegevens in [ modellen ](/help/models/build.md#configure) te gebruiken. | 25 februari 2026 | 25 februari 2026 |
| **[!UICONTROL Granular incrementality reporting]** | Bepaal geharmoniseerde gebieden zodat kunt u neer in het melden van uw model boren gebruikend [ korrelige inzichten die gebieden ](/help/models/build.md#granular-insights-reporting-fields) melden, in plaats van het moeten afzonderlijke modellen tot stand brengen. | 18 februari 2026 | 18 februari 2026 |

## januari 2026

| Functie | Beschrijving | [ Begin van de Uitvoer ](#release-strategy) | [ Algemene Beschikbaarheid ](#release-strategy) |
|---|---|---|---|
| **[!UICONTROL Dataset rules]** | [ Bijgewerkte lijst van datasetregels ](/help/harmonize-data/dataset-rules.md). U kunt naar één of meerdere datasetregels zoeken en, een datasetregel direct van de lijst bekijken uitgeven of schrappen. | 13 januari 2026 | 13 januari 2026 |
| **[!UICONTROL Current spend]** | Voeg een huidig doorvoerpunt in de [ marginale visualisatie van de reactiecurve ](/help/models/insights.md#marginal-response-curves) in Modelinzichten toe. | 13 januari 2026 | 13 januari 2026 |
| **[!UICONTROL Sort and resize columns]** | Toegevoegde soort en resize van kolommen in de [ Modellen ](/help/models/overview.md) en [ Punten ](/help/plans/overview.md) lijst. | 13 januari 2026 | 13 januari 2026 |
| **Bevestigingen** | Oplossingen voor de volgende tickets: <ul><li>AMM-3328: Veldinvoer uitgeschakeld voor nieuwe operatoren voor Factoren</li><li>AMM-3359: Datumkiezer en keuzelijst met invoervak vergrendelen.</li><li>AMM-3441: Het dupliceren van een abonnement vult niet automatisch het datumbereik en het budget in.</li></ul> | 13 januari 2026 | 13 januari 2026 |


## Releasestrategie

[!UICONTROL Mix Modeler] gebruikt functiemarkeringen (ook wel &#39;schakelmarkeringen&#39; genoemd) om de zichtbaarheid van nieuwe functies te bepalen, zodat u de functionaliteit op gecontroleerde schaal kunt testen voordat de volledige versie wordt uitgebracht. Deze releasestrategie omvat de volgende fasen:

* **Beperkte het Testen**: Een gefaseerde versie begint met het testen door interne gebruikers van Adobe. Het wordt dan ter beschikking gesteld aan een kleine groep klantenrekeningen om ervoor te zorgen dat de eigenschap aan klantenbehoeften en verwachtingen voldoet.

* **Begin van Uitvoer**: De Uitvoer van een gefaseerde versie begint met de Beperkte het Testen fase. De release wordt vervolgens in de loop van een paar maanden geschaald van 0% naar 100% beschikbaarheid voor klanten. De gefaseerde uitrol gebeurt op het niveau van de Organisatie van Experience Cloud, zodat ontvangen alle gemachtigde gebruikers in een organisatie de zelfde ervaring.

