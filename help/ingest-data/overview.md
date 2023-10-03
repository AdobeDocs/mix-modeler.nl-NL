---
title: Samenvattingsgegevens
description: Leer hoe u gegevens in de Mix Modeler kunt opnemen.
feature: Datasets, Event Datasets, Summary Datasets, Aggregate Datasets
exl-id: dc16a601-bbd9-467b-8a7e-c32654d4069a
source-git-commit: 33883626d8e7aca2eecc3571593be53ef41ac458
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 10%

---

# Samenvattingsgegevens

Mix Modeler werkt met gegevens op gebeurtenisniveau, geaggregeerde gegevens over marketinginspanningen van diverse tuinen en aggregaten of samenvattende gegevens van andere bronnen, zoals offlinereclame, interne factoren of externe factoren.

De klanten kunnen om het even welk soort gegevens gebruiken die in Experience Platform als datasets worden opgenomen en die op schema&#39;s gebruikend XDM ExperienceEvent of XDM Summiere Metrics als basisklasse gebaseerd is.

Bijvoorbeeld:

* gegevens die zijn verzameld via de Adobe Analytics-bronaansluiting en zijn omgezet in gegevenssets die overeenkomen met de standaardversie of een aangepaste versie van het Adobe Analytics-schema, of anders
* gegevens die worden verzameld met de SDK van het Web van het Experience Platform, Mobiele SDK, of de Server API van het Netwerk van Edge voor het verzamelen van klanteninteractie op Web, mobiel, of een ander type van apparaat;
* geaggregeerde gegevens van gedraaide tuinen (zoals Facebook, YouTube), verkeersbronnen of gegevens over offlinereclame;
* niet-marketingaggregaat of samenvattende gegevens die interne of externe factoren bevatten die nuttig zijn voor het samenstellen van modellen.

U kunt om het even welk soort mechanisme gebruiken, gesteund door Experience Platform, om uw ervaring gebeurtenis-niveau, samengevoegde marketing inspanningsgegevens, en gegevens uit andere bronnen op te nemen. Bijvoorbeeld de Experience Platform-SDK&#39;s, API&#39;s, bronconnectors, streaming en batch-opname.


## Richtsnoeren

Volg deze richtlijnen om gegevens in Experience Platform in te voeren voor gebruik met Mix Modeler:

* De incrementele gegevens die aan de gegevenssets worden toegevoegd, mogen elkaar niet overlappen.
* Alle gegevens van één bron moeten dezelfde korreligheid hebben.
* Datum en granulariteit zijn verplichte velden in het onderliggende schema voor alle geaggregeerde gegevens die als datasets zijn opgenomen
* Kanaal is een verplicht veld in het onderliggende schema voor alle marketinginspanningen/bestedingsgegevens die als datasets worden ingevoerd.


## Voorbeelden

Hieronder vindt u enkele voorbeelden van gegevens die gewoonlijk in de Mix Modeler worden gebruikt en die verder gaan dan de meer standaard ervaringsgebeurtenisgegevens.

+++ Geaggregeerde gegevens over de marketinginspanning

| Geo | Datum | Datumtype | Kanaal | Campaign | Klikken | Verkocht | Betrokkenheid | Impressie | Open | Eigendom | Verzonden |
|---|:--|---|:---:|---|--:|---|--:|---|---|---|--:|
| AMER | 2021-10-31 | dag | EMAIL | | 12752 | | | | | | 1132945 |
| AMER | 2021-10-31 | dag | FB | | 148844 | | | | | | |
| AMER | 2021-10-31 | dag | YT | | | | 2314452 | | | | |
| JPN | 2021-10-21 | dag | EMAIL | | 21089 | | | | | | 3283626 |
| JPN | 2021-10-21 | dag | SOCIAAL | | | | 621 | | | | |

{style="table-layout:auto"}

+++

+++ Geaggregeerde conversiegegevens

| Geo | Datum | Datumtype | Product | Verkochte eenheden | Ontvangsten |
|---|:---|:---:|---|--:|--:|
| EMEA | 2021-09-13 | dag | Maker Economie | 603 | 36537.68 |
| EMEA | 2021-09-13 | dag | Metavers | 55 | 21704.37 |
| JPN | 2022-05-30 | dag | Pro Imaging | 487 | 64469.60 |
| JPN | 2022-05-30 | dag | Document Cloud | 642 | 100509.07 |

{style="table-layout:auto"}

+++

+++ Gegevens van externe factoren

| Gegevens | Datumtype | Factor | Waarde |
|---|:---:|:---:|:---|
| 2020-08-02 | week | SPX | 3325.866 |
| 2020-08-09 | week | SPX | 3364.158 |
| 2020-08-16 | week | SPX | 3385.858 |
| 2020-08-23 | week | SPX | 3497.965 |

{style="table-layout:auto"}

+++

Om met gegevens in Mix Modeler te werken, hebt u gegevens nodig die in datasets worden verzameld en na schema&#39;s in Experience Platform worden gemodelleerd. De interface van de Mix Modeler verleent gemakkelijke toegang tot zowel de Schema&#39;s als Datasets UI.


>[!MORELIKETHIS]
>
>Zie voor meer details over hoe te om schema&#39;s en datasets te beheren:
>
>* [Schema&#39;s](schemas.md)
>* [Gegevenssets](datasets.md)
