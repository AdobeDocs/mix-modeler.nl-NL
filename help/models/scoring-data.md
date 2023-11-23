---
title: Scoregegevens
description: Leer hoe de scoring-gegevens van een model in de Mix Modeler aanhouden.
feature: Models
source-git-commit: 3596b83937b3f61ac453940f3a666d8aaf713679
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 3%

---


# Scoregegevens

Als deel van het scoren van een model, wordt het scoren van gegevens voortgeduurd binnen een dataset in Experience Platform. Deze dataset is in overeenstemming met een schema dat voor elk model in uw instantie van de Mix Modeler wordt gecreeerd.

Het schema voor het zoeken naar gegevens heeft een soortgelijke naam `AMM AI Schema - <name of model> <id>`. Bijvoorbeeld: `AMM AI Schema - Model for Online Conversion 10120`.

De dataset, die de het scoren gegevens voor een model voortduurt, wordt genoemd als `AMM AI Aggregrate Scores - <id>`bijvoorbeeld `AMM AI Aggregrate Scores - 10120`.


## Schema

Het schema bevat een veldgroep met een object dat details bevat over de scores. Het object bestaat uit de volgende velden.

| Veldnaam | Type | Definitie |
|---|---|---|
| **campagneGroup** | String | Naam van de campagnegroep. |
| **campagneName** | String | Naam van de campagne. |
| **bijdrage** | Dubbel | Bijdrage voor deze conversie voor het opgegeven aanraakpunt. |
| **conversionEndDate** | Datum | Einddatum van het conversievenster. |
| **conversionName** | String | Naam van de omzetting die tijdens de de opstellingsstap van de omzettingsdefinitie werd gecreeerd. |
| **conversionStartDate** | Datum | Begindatum van het conversievenster. |
| **geo** | String | De geografische locatie waar de conversie heeft plaatsgevonden. |
| **mediaChannel** | String | Naam van het kanaal dat tijdens de stap van de aanraakpuntopstelling werd gebruikt. |
| **mediaSubChannel** | String | Naam van het subkanaal. |
| **omzet** | Dubbel | Ontvangsten die voor het opgegeven aanraakpunt aan deze omrekening zijn toegerekend. |
| **scoreCreatedTime** | DateTime | Tijdstip waarop deze score wordt gemaakt. |
| **touchpointEndDate** | Datum | Einddatum van het aanraakpuntvenster. |
| **touchpointName** | String | Naam van het aanraakpunt dat tijdens de de opstellingsstap van de aanraakpuntdefinitie werd gecreeerd. Momenteel wordt het aanraakpunt gedefinieerd op het mediakanaal. |
| **touchpointStartDate** | Datum | Begindatum van het aanraakpuntvenster. |

