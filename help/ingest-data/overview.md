---
title: Samenvattingsgegevens
description: Leer hoe u gegevens in Adobe Mix Modeler kunt opnemen.
feature: Datasets, Event Datasets, Summary Datasets, Aggregate Datasets
source-git-commit: ae1c74ed2edf1e69e7ab77d16aba797921c14ad9
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 10%

---


# Samenvattingsgegevens

Adobe Mix Modeler werkt met gegevens op gebeurtenisniveau en geaggregeerde gegevens over marketinginspanningen van verschillende gardens. Klanten kunnen alle soorten gegevens gebruiken die in Adobe Experience Platform als datasets worden opgenomen en die op op gebeurtenis-gebaseerde schema&#39;s van de Ervaring XDM zijn gebaseerd.

Bijvoorbeeld:

* gegevens die zijn verzameld via de Adobe Analytics-bronaansluiting en zijn omgezet in gegevenssets die overeenkomen met de standaardversie of een aangepaste versie van het Adobe Analytics-schema, of anders
* gegevens die zijn verzameld met de Adobe Experience Platform Web SDK, Mobile SDK of Edge Network Server API voor het verzamelen van klantinteracties op het web, mobiele apparaten of andere apparaten;
* samenvattingsgegevens van verschillende afgezette tuin/verkeersbronnen, gebaseerd op een schema dat de XDM Summiere klasse van Metriek met de het gebiedsgroep van de Samenvatting van het Verkeer en van de Omzetting omvat;
* niet-marketinggegevens (bijvoorbeeld macro-economische indicatoren) die nuttig zijn voor modelopbouw;

U kunt elk door Adobe Experience Platform ondersteund mechanisme gebruiken om uw ervaringsniveau en geaggregeerde gegevens over de marketinginspanning in te voeren. Zoals de SDK&#39;s van Adobe Experience Platform, API&#39;s, bronconnectors, streaming en batch-opname.


## Richtsnoeren

Volg de onderstaande richtlijnen om gegevens in te voeren in Adobe Experience Platform voor gebruik met Adobe Mix Modeler:

* De incrementele gegevens die aan de gegevenssets worden toegevoegd, mogen elkaar niet overlappen.
* Alle gegevens van één bron moeten dezelfde korreligheid hebben.
* Datum en granulariteit zijn verplichte velden in het onderliggende schema voor alle geaggregeerde gegevens die als datasets zijn opgenomen
* Kanaal is een verplicht veld in het onderliggende schema voor alle marketinginspanningen/bestedingsgegevens die als datasets worden ingevoerd.


## Voorbeelden

Hieronder vindt u enkele voorbeelden van gegevens die gewoonlijk worden gebruikt in Adobe Mix Modeler naast meer standaardervaringsgebeurtenisgegevens.

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

Om met gegevens in de Modelleur van de Mengeling van de Adobe te werken, hebt u gegevens nodig die in datasets worden verzameld en na schema&#39;s in Adobe Experience Platform worden gemodelleerd. De interface van de Modelleur van de Mengeling van de Adobe verleent gemakkelijke toegang tot zowel de Schema&#39;s als Datasets UI.

>[!MORELIKETHIS]
>
>Zie voor meer details over hoe te om schema&#39;s en datasets te beheren:
>
>* [Schema&#39;s](schemas.md)
>* [Gegevenssets](datasets.md)
