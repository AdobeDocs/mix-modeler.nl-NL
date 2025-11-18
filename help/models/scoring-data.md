---
title: Schermindelingsgegevens gebruiken
description: Leer hoe de score van een model in Mix Modeler wordt voortgezet.
feature: Models
exl-id: 2f2c3d20-7b14-41cc-a11a-03e8ad9e5d7a
source-git-commit: 1a9df9f9819d9e0031e58443ec6a9e755a151ba0
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Schermindelingsgegevens gebruiken

Als deel van het scoren van een model, wordt het scoren van gegevens voortgeduurd binnen een dataset in Experience Platform. Als u aanraakkenmerk hebt ingeschakeld tijdens het maken van een model, blijven aanvullende gegevens over de gebeurtenisscore behouden in een gegevensset in Experience Platform.

Elk van deze datasets is met een schema in overeenstemming. Dit artikel documenteert deze schema&#39;s.


## Samengevoegd gegevensschema voor scoring

Het schema voor het noteren van gegevens krijgt de naam `AMM AI Schema - <name of model> <id>` . Bijvoorbeeld: `AMM AI Schema - Model for Online Conversion 10120` .

De dataset, die de het scoren gegevens voor een model voortduurt, wordt genoemd als `AMM AI Aggregrate Scores - <id>`, bijvoorbeeld `AMM AI Aggregrate Scores - 10120`.

Het schema bevat een veldgroep met een object dat details bevat over de scores. Het object bestaat uit de volgende velden.

| Veldnaam | Type | Definitie |
|---|---|---|
| `campaignGroup` | String | Naam van de campagnegroep. |
| `campaignName` | String | Naam van de campagne. |
| `contribution` | Dubbel | Bijdrage voor deze conversie voor het opgegeven aanraakpunt. |
| `conversionEndDate` | Datum | Einddatum van het conversievenster. |
| `conversionName` | String | Naam van de omzetting die tijdens de de opstellingsstap van de omzettingsdefinitie werd gecreeerd. |
| `conversionStartDate` | Datum | Begindatum van het conversievenster. |
| `geo` | String | De geografische locatie waar de conversie heeft plaatsgevonden. |
| `mediaChannel` | String | Naam van het kanaal dat tijdens de stap van de aanraakpuntopstelling werd gebruikt. |
| `mediaSubChannel` | String | Naam van het subkanaal. |
| `revenue` | Dubbel | Ontvangsten die voor het opgegeven aanraakpunt aan deze omrekening zijn toegerekend. |
| `scoreCreatedTime` | DateTime | Tijdstempel wanneer deze score wordt gemaakt. |
| `touchpointEndDate` | Datum | Einddatum van het aanraakpuntvenster. |
| `touchpointName` | String | Naam van het aanraakpunt dat tijdens de de opstellingsstap van de aanraakpuntdefinitie werd gecreeerd. Momenteel wordt het aanraakpunt gedefinieerd op het mediakanaal. |
| `touchpointStartDate` | Datum | Begindatum van het aanraakpuntvenster. |


## Gegevensschema voor scores voor gebeurtenissen

Het schema voor het noteren van gegevens krijgt de naam `Attribution AI Scores - <name of model> <id> - Schema` . Bijvoorbeeld: `Attribution AI Scores - Model for Online Conversion 10120 - Schema` .

De dataset, die de het scoren gegevens voor een model voortduurt, wordt genoemd als `Attribution AI Scores - <name of model> <id>`, bijvoorbeeld `Attribution AI Scores - Model for Online Conversion 10120 `.

Het schema bevat een veldgroep met een object dat details over de kernen bevat. Het object krijgt de naam `attibution_AI_scores__<name of model> id` .

De veldgroep bevat de volgende velden.

| Veldnaam | Type | Beschrijving |
|---|---|---|
| `conversion` | Object | Kolommen met omzettingsmetagegevens. |
|     `passThrough` | Object |  |
|         `eventType` | String | |
|         `channel_typeAtSource` | String | |
|      `dataSource` | String | Globaal unieke identificatie van een gegevensbron. <br> **Voorbeeld:** `Adobe Analytics` |
|      `eventSource` | String | De bron op het moment dat de werkelijke gebeurtenis plaatsvond. <br> **Voorbeeld:** `Adobe.com` |
|      `eventType` | String | Het primaire gebeurtenistype voor deze tijd-reeksverslag. <br> **Voorbeeld:** `Order` |
|      `geo` | String | De geografische locatie waar de conversie is uitgevoerd `placeContext.geo.countryCode` . <br> **Voorbeeld:** `US` |
|      `path` | String | |
|      `priceTotal` | Dubbel | Door de conversie verkregen inkomsten <br> **Voorbeeld:** `99.9` |
|      `product` | String | De XDM-id van het product zelf. <br> **Voorbeeld:** `RX 1080 ti` |
|      `productType` | String | De weergavenaam van het product zoals deze aan de gebruiker wordt getoond voor deze productweergave. <br> **Voorbeeld:** `Gpus` |
|      `quantity` | Geheel | Tijdens de conversie aangekochte hoeveelheid. <br> **Voorbeeld:** `1` |
|      `receivedTimeStamp` | DateTime | Tijdstempel van de conversie ontvangen. <br> **Voorbeeld:** `2020-06-09T00:01:51.000Z` |
|      `skuId` | String | Stock keeping unit (SKU), de unieke identificator voor een product dat door de verkoper wordt gedefinieerd. <br> **Voorbeeld:** `MJ-03-XS-Black` |
|      `timestamp` | DateTime | Tijdstempel van de conversie. <br> **Voorbeeld:** `2020-06-09T00:01:51.000Z` |
|      `totalDaysToConversion` | Geheel |  |
|      `totalTouchpointCount` | Geheel | |
| `customerProfile` | Object | Identiteitsgegevens van de gebruiker die wordt gebruikt om het model te bouwen. |
|      `identity` | Object | |
|           `id` | String | |
|           `namespace` | String | Bevat de details van de gebruiker die wordt gebruikt om het model te bouwen zoals `id` en `namespace`. |
| `touchpointsDetail` | Object [] | De lijst met aanraakpuntdetails die leiden tot de conversie, geordend op een aanraakpunt of tijdstempel. |
|      `scores` | Object | Aanraakpuntbijdrage voor deze conversie als score. |
|           `algorithmicInfluenced` | Dubbel | De beïnvloede score is de fractie van de omzetting die elk marketing aanraakpunt voor verantwoordelijk is. |
|           `algorithmicSourced` | Dubbel | De incrementele score is de hoeveelheid marginale impact die rechtstreeks wordt veroorzaakt door een marketingaanraakpunt. |
|           `decayUnits` | Dubbel | Op regels gebaseerde attributiescore waarbij aanraakpunten die dichter bij de conversie liggen, meer krediet krijgen dan aanraakpunten die verder van de conversie verwijderd zijn. |
|           `firstTouch` | Dubbel | Op regel gebaseerde attributiescore die alle credits toewijst aan het eerste aanraakpunt op een conversiepad. |
|           `lastTouch` | Dubbel | Op regel gebaseerde attributiescore die alle punten toewijst aan het aanraakpunt dat het dichtst bij de conversie ligt. |
|           `linear` | Dubbel | Op regel gebaseerde attributiescore die gelijk krediet aan elk aanraakpunt op een conversiepad toewijst. |
|           `uShape` | Dubbel | Op regels gebaseerde attributiescore die 40% van het krediet toewijst aan het eerste aanraakpunt en 40% van het krediet aan het laatste aanraakpunt. De andere aanraakpunten splitsen de resterende 20% gelijkmatig. |
|      `touchPoint` | Object | Metagegevens van aanraakpunten. |
|           `passThrough` | Object | |
|                `eventType` | String | |
|           `campaignGroup` | String |  |
|           `campaignName` | String | |
|           `campaignTag` | String | |
|           `eventId` | String | |
|           `geo` | String | |
|           `mediaAction` | String | |
|           `mediaChannel` | String | |
|           `receivedTimeStamp` | DateTime | |
|           `timestamp` | DateTime | |
|      `isFirstInThePosition` | Geheel | |
|      `lag` | Geheel | |
|      `position` | String | |
|      `touchpointCountToConversion` | Geheel | |
|      `touchpointName` | String | Naam van touchpoint dat tijdens opstelling werd gevormd. <br> **Voorbeeld:** `PAID_SEARCH_CLICK` |
| `conversionName` | String | Naam van de omzetting die tijdens opstelling werd gevormd. <br> **Voorbeeld:** `Order`, `Lead`, `Visit` |
| `scoreCreatedTime` | DateTime | |
| `segmentation` | String | Conversiesegment zoals geo segmentation, waar het model tegen wordt gebouwd. Wanneer segmenten ontbreken, is `segmentation` gelijk aan `conversionName` . <br> **Voorbeeld:** `ORDER_US` |





Zie [ Schema&#39;s ](../ingest-data/schemas.md) voor meer informatie.
