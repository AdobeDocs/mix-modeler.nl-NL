---
title: Overzicht van samenvattingsgegevens
description: Leer hoe u gegevens in Mix Modeler kunt opnemen.
feature: Datasets, Event Datasets, Summary Datasets, Aggregate Datasets
exl-id: dc16a601-bbd9-467b-8a7e-c32654d4069a
source-git-commit: 857641f6c1db749f79056ce2a2ea35fc4d3e3a3c
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 5%

---

# Overzicht van samenvattingsgegevens

Mix Modeler werkt met gegevens op het niveau van de gebeurtenis, geaggregeerde of samenvattende marketinggegevens van verschillende tuinen, en geaggregeerde of samenvattende gegevens van een andere bron, zoals offlinereclame, interne factoren of externe factoren.

De klanten kunnen om het even welk soort gegevens gebruiken die in Experience Platform als datasets worden opgenomen en die op schema&#39;s gebruikend XDM ExperienceEvent of XDM Summiere Metrics als basisklasse gebaseerd is.

Bijvoorbeeld:

* gegevens die zijn verzameld via de Adobe Analytics-bronaansluiting en zijn omgezet in gegevenssets die overeenkomen met de standaardversie of een aangepaste versie van het Adobe Analytics-schema, of anders
* gegevens die zijn verzameld met de Experience Platform Web SDK, Mobile SDK of Edge Network Server-API voor het verzamelen van klantinteracties op internet, mobiel of een ander type apparaat;
* geaggregeerde of samenvattende gegevens van gedraaide tuinen (zoals Facebook, YouTube), verkeersbronnen of gegevens over offlinereclame;
* niet-marketingaggregaat of samenvattende gegevens die interne of externe factoren bevatten die nuttig zijn voor het samenstellen van modellen.

U kunt om het even welk soort mechanisme gebruiken, gesteund door Experience Platform, om uw ervaring gebeurtenis-niveau, samengevoegde marketing inspanningsgegevens, en gegevens uit andere bronnen op te nemen. Zoals de SDK&#39;s van Experience Platform, API&#39;s, bronconnectors, streaming en batch-opname.


## Richtsnoeren

Volg de onderstaande richtlijnen om gegevens in te voeren in Experience Platform voor gebruik met Mix Modeler:

* De incrementele gegevens die aan de gegevenssets worden toegevoegd, mogen elkaar niet overlappen.
* Alle gegevens van één bron moeten dezelfde korreligheid hebben.
* Datum en granulariteit zijn verplichte velden in het onderliggende schema voor alle geaggregeerde gegevens die als datasets zijn opgenomen
* Kanaal is een verplicht veld in het onderliggende schema voor alle marketinginspanningen/bestedingsgegevens die als datasets worden ingevoerd.


## Voorbeelden

Hieronder vindt u enkele voorbeelden van gegevens die gewoonlijk in Mix Modeler worden gebruikt, die verder gaan dan de meer standaard ervaringsgebeurtenisgegevens.

+++ Geaggregeerde gegevens over de marketinginspanning

| Geo | Datum | Datumtype | Kanaal | Campaign | Klikken | Verkocht | Betrokkenheid | Impressie | Openen | Eigendom | Verzonden | Draaien |
|---|:--|---|:---:|---|--:|---|--:|---|---|---|--:|--:|
| AMER | 2021-10-31 | dag | EMAIL | | 12752 | | | | | | 1132945 | |
| AMER | 2021-10-31 | dag | FB | | 148844 | | | | | | | 42111 |
| AMER | 2021-10-31 | dag | YT | | | | 2314452 | | | | | 10540 |
| JPN | 21-10-2021 | dag | EMAIL | | 21089 | | | | | | 3283626 | |
| JPN | 21-10-2021 | dag | SOCIAAL | | | | 621 | | | | | 74512 |

{style="table-layout:auto"}

+++

+++ Geaggregeerde conversiegegevens

| Geo | Datum | Datumtype | Product | Verkochte eenheden | Ontvangsten |
|---|:---|:---:|---|--:|--:|
| EMEA | 2021-09-13 | dag | Maker Economie | 603 | 36537,68 |
| EMEA | 2021-09-13 | dag | Metavers | 55 | 21704,37 |
| JPN | 2022-05-30 | dag | Pro Imaging | 487 | 64469,60 |
| JPN | 2022-05-30 | dag | Document Cloud | 642 | 100509,07 |

{style="table-layout:auto"}

+++

+++ Gegevens van externe factoren

| Gegevens | Datumtype | Factor | Waarde |
|---|:---:|:---:|:---|
| 2020-08-02 | week | SPX | 3325,866 |
| 2020-08-09 | week | SPX | 3364,158 |
| 2020-08-16 | week | SPX | 3385,858 |
| 23-08-2020 | week | SPX | 3497,965 |

{style="table-layout:auto"}

+++

Om met gegevens in Mix Modeler te werken, hebt u gegevens nodig die in datasets worden verzameld en na schema&#39;s in Experience Platform worden gemodelleerd. De interface van Mix Modeler biedt eenvoudige toegang tot zowel de Experience Platform-schema&#39;s als de Datasets-interface.


## Valideren

Als u wilt controleren of uw gegevens correct beschikbaar zijn in Mix Modeler, kunt u het volgende doen:

* De visualisaties van het gebruik in [ Overzicht ](/help/overview.md).
* De download en inspecteert gegevens van [ Geharmoniseerde gegevens ](/help/harmonize-data/overview.md) in Geharmoniseerde datasets.

Om te bevestigen of uw gegevens behoorlijk in Experience Platform worden opgenomen, kunt u [ SQL vragen schrijven en uitvoeren gebruikend de Dienst van de Vraag van Experience Platform ](https://experienceleague.adobe.com/en/docs/experience-platform/query/home).


>[!MORELIKETHIS]
>
>Zie voor meer details over hoe te om schema&#39;s en datasets te beheren:
>
>* [ Schemas ](schemas.md)
>* [ Datasets ](datasets.md)
