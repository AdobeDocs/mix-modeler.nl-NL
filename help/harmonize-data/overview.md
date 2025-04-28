---
title: Overzicht van gegevenssets harmoniseren
description: Leer hoe u gegevens in Mix Modeler kunt harmoniseren.
feature: Harmonized Data
exl-id: 6cb70762-e3b2-46a0-b028-1d6daf3edae5
source-git-commit: 857641f6c1db749f79056ce2a2ea35fc4d3e3a3c
workflow-type: tm+mt
source-wordcount: '1013'
ht-degree: 4%

---

# Overzicht van gegevenssets harmoniseren

De gegevens in Mix Modeler zijn van verschillende aard, afhankelijk van de gegevensbron. De gegevens kunnen zijn:

* geaggregeerde of samenvattende gegevens, bijvoorbeeld verzameld uit zogenaamde tuingegevensbronnen of offline advertentiegegevens die (zoals het uitgeven) zijn verzameld uit het voeren van een billboardcampagne, een evenement of een fysieke advertentiecampagne;
* gebeurtenisgegevens, bijvoorbeeld uit gegevensbronnen van de eerste partij. Deze gebeurtenisgegevens kunnen worden verzameld via de Adobe Analytics-bronconnector van Adobe Analytics, of via de Experience Platform Web-, Mobile SDK- of Edge Network-API, of via gegevens die via bronconnectors worden ingevoerd.

De harmonisatiedienst van Mix Modeler vergelijkt de geaggregeerde gegevens en de gebeurtenisgegevens in een consistent gegevensoverzicht. Deze gegevensmening, die met [ interne en externe factorgegevens ](#factors) wordt gecombineerd, is de bron voor de modellen in Mix Modeler. De dienst gebruikt de hoogste granulariteit over de verschillende datasets. Bijvoorbeeld, als één dataset een granulariteit van maandelijkse en resterende datasets wekelijkse en dagelijkse granulariteit heeft, leidt de harmonisatiedienst tot een gegevensmening gebruikend maandelijkse granulariteit.

## Factoren

Factoren zijn essentieel voor het maken van modellen en u wilt begrijpen welke invloed het bedrijf holistisch heeft. Factoren zijn mogelijk niet gerelateerd aan marketinggegevens.

* De interne factoren zijn specifiek voor uw organisatie en kunnen uw omzettingen beïnvloeden. Bijvoorbeeld het verkoopseizoen, de promoties en nog veel meer.

* Externe factoren zijn factoren buiten de controle van uw organisatie maar die nog steeds van invloed kunnen zijn op de omzettingen die u bereikt. Voorbeelden zijn CPI, S&amp;P 500, en meer.



## Een voorbeeld van geharmoniseerde gegevens

Stel dat de volgende datasets beschikbaar zijn voor Mix Modeler.

**Dataset 1**

Bevat een gegevensset van de marketinginspanning van YouTube, met een granulariteit van de geaggregeerde gegevensset tot dagelijks.

| Datum | Datumtype | Kanaal | Campaign | Merk | Geo | Klikken | Draaien |
|---|:--:|---|---|---|---|---:|---:|
| 31-12-2021 | dag | YouTube | Y_Fall_02 | MerkX | VS | 10000 | 100 |
| 01-01-2022 | dag | YouTube | Y_Fall_02 | MerkX | VS | 1000 | 10 |
| 01-03-2022 | dag | YouTube | Y_Fall_01 | MerkY | CA | 10000 | 100 |
| 01-04-2022 | dag | YouTube | Y_Summer_01 | Null | CA | 9000 | 80 |

{style="table-layout:auto"}


**Dataset 2**

Bevat gegevensset over marketinginspanningen van Facebook, met een granulariteit van de geaggregeerde gegevensset tot wekelijks.

| Datum | Datumtype | Kanaal | Campaign | Geo | Klikken | Draaien |
|--- |:---:|--- |---|---|---:|---:|
| 01-01-2022 | week | Facebook | FB_Fall_01 | VS | 8000 | 100 |
| 01-08-2022 | week | Facebook | FB_Fall_02 | VS | 1000 | 10 |
| 01-08-2022 | week | Facebook | FB_Fall_01 | VS | 7000 | 100 |
| 16-01-2022 | week | Facebook | FB_Summer_01 | CA | 10000 | 80 |

{style="table-layout:auto"}


**Dataset 3**

Een omzettingsdataset, met een granulariteit van de samengevoegde gegevensreeks aan dagelijks.

| Datum | Datumtype | Geo | Goal | Ontvangsten |
|--- |:---: |---|---|---:|
| 01-01-2022 | dag | VS | Mode | 200 |
| 01-08-2022 | dag | VS | Mode | 10 |
| 01-08-2022 | dag | VS | Juwelen | 1100 |
| 16-01-2022 | dag | CA | Juwelen | 80 |

{style="table-layout:auto"}


**Dataset 4**

Een steekproefervaring gebeurtenisdataset (de gebeurtenissen van SDK van het Web) van de klant.

| Tijdstempel | Naamruimte van identiteit | Identiteitskaart | Kanaal | Klikken |
|--- |--- |--- |--- |---:|
| 01-01-2022 00 :01: 1.000 | ECID | 64fd46ff-8c63-43b4-85a7-92b953113ba0 | CSE | 1 |
| 01-01-2022 00 :01: 1.000 | ECID | 64fd46ff-8c63-43b4-85a7-92b953113ba0 | CSE | 1 |
| 01-08-2022 00 :01: 1.000 | ECID | 2ca2a16e-caf0-4fa9-9a8b-9774b39547c4 | CSE | 1 |
| 01-08-2022 00 :01: 1.000 | ECID | 5ce99bfb-e44a-40d9-b8cd-c5408bda7cdc | CSE | 1 |

{style="table-layout:auto"}


U wilt een geharmoniseerde dataset bouwen, met een granulariteit die aan wekelijkse wordt geplaatst. De gebeurtenisgegevens worden geaggregeerd naar weekgranulariteit en toegevoegd aan de geharmoniseerde gegevensset. Het resultaat is:

**Geharmoniseerde dataset**

| Datum | Datumtype | Kanaal | Campaign | Merk | Geo | Goal | Klikken | Draaien | Ontvangsten |
|--- |:---:|--- |--- |--- |---|---|---:|---:|---:|
| 27-12-2021 | week | YouTube | Y_Fall_02 | MerkX | VS | Null | 11000 | 110 | Null |
| 01-03-2022 | week | YouTube | Y_Fall_01 | MerkY | CA | Null | 10000 | 100 | Null |
| 01-03-2022 | week | YouTube | Y_Summer_01 | Null | CA | Null | 9000 | 80 | Null |
| 01-01-2022 | week | Facebook | FB_Fall_01 | Null | VS | Null | 8000 | 100 | Null |
| 01-08-2022 | week | Facebook | FB_Fall_02 | Null | VS | Null | 1000 | 10 | Null |
| 01-08-2022 | week | Facebook | FB_Fall_01 | Null | VS | Null | 7000 | 100 | Null |
| 16-01-2022 | week | Facebook | FB_Summer_01 | Null | CA | Null | 10000 | 80 | Null |
| 27-12-2021 | week | Null | Null | Null | VS | Mode | Null | Null | 200 |
| 01-03-2022 | week | Null | Null | Null | VS | Mode | Null | Null | 10 |
| 01-03-2022 | week | Null | Null | Null | VS | Juwelen | Null | Null | 1100 |
| 10-01-2022 | week | Null | Null | Null | CA | Juwelen | Null | Null | 80 |
| 01-01-2022 | week | CSE | Null | Null | Null | Null | 2 | Null | Null |
| 01-08-2022 | week | CSE | Null | Null | Null | Null | 2 | Null | Null |

{style="table-layout:auto"}


## geharmoniseerde gegevens instellen

Om een geharmoniseerde dataset, als in het vereenvoudigde [ voorbeeld ](#an-example-of-harmonized-data) te bouwen, moet u deze stappen volgen:

1. Bepaal extra [ geharmoniseerde gebieden ](fields.md) die u voorbij de globale geharmoniseerde gebieden wilt gebruiken reeds beschikbaar.
1. De regels van de opstelling [ dataset ](dataset-rules.md) om gebieden van uw aggregaat of ervaringsgebeurtenisdatasets aan geharmoniseerde gebieden in kaart te brengen.
1. Bepaal [ marketing touchpoints ](marketing-touchpoints.md) gebruikend de standaard en extra geharmoniseerde gebieden die u bepaalde.
1. Bepaal [ omzettingen ](conversions.md) gebruikend de standaard en extra geharmoniseerde gebieden die u bepaalde.


## Geharmoniseerde gegevens weergeven

Om uw geharmoniseerde gegevens te zien, in de interface van Mix Modeler:

1. Selecteer ![ DataSearch ](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized datasets]** van het linkerspoor.

1. Selecteer **[!UICONTROL Harmonized data]** in de bovenste balk. Een overzicht van uw geharmoniseerde gegevens wordt getoond gebaseerd op de gebieden, datasetregels, marketing touchpoints en omzettingen u hebt bepaald.

   1. Om de periode opnieuw te bepalen waarop de rechthoek van geharmoniseerde gegevens gebaseerd is, ga een datumwaaier voor **[!UICONTROL Date range]** in of gebruik ![ Kalender ](/help/assets/icons/Calendar.svg) om een gegevenswaaier te selecteren.

   1. Om de geharmoniseerde gebiedskolommen te wijzigen die voor de Geharmoniseerde gegevenslijst worden getoond, gebruik ![ Montages ](/help/assets/icons/Setting.svg) om de **[!UICONTROL Column settings]** dialoog te openen.

      1. Selecteer ![ SelectBox ](/help/assets/icons/SelectBox.svg) één of meerdere kolommen van **[!UICONTROL AVAILABLE COLUMNS]** en gebruik ![ Schrap recht ](/help/assets/icons/ChevronRight.svg) om deze kolommen aan **[!UICONTROL SELECTED COLUMNS]** toe te voegen.

      1. Selecteer ![ SelectBox ](/help/assets/icons/SelectBox.svg) één of meerdere kolommen van **[!UICONTROL SELECTED COLUMNS]** en gebruik ![ Verduisteren verlaten ](/help/assets/icons/ChevronLeft.svg) om de geselecteerde kolommen te verwijderen en deze kolommen terug naar **[!UICONTROL AVAILABLE COLUMNS]** terug te keren.

      1. Selecteer een kolom in **[!UICONTROL DEFAULT SORT]** en schakel tussen **[!UICONTROL Ascending]** of **[!UICONTROL Descending]** .

      1. Als u de volgorde van de weergegeven kolommen wilt wijzigen, kunt u een kolom in **[!UICONTROL SELECTED COLUMNS]** omhoog en omlaag verplaatsen via slepen en neerzetten.

   1. Selecteer **[!UICONTROL Submit]** om de wijzigingen in de kolominstelling te verzenden. Selecteer **[!UICONTROL Close]** om de aangebrachte wijzigingen te annuleren.

1. Als meer pagina&#39;s beschikbaar zijn, gebruik ![ Pijl links ](/help/assets/icons/ChevronLeft.svg) of ![ Pijl rechts ](/help/assets/icons/ChevronRight.svg) bij **[!UICONTROL Page _x _van_ x_]** om zich tussen pagina&#39;s te bewegen.

1. U kunt de geharmoniseerde gegevens desgewenst downloaden.

   1. Selecteer ![ Download ](/help/assets/icons/Download.svg) [!BADGE  bèta ].
   1. In popup, uitgezochte ![ AddCircle ](/help/assets/icons/AddCircle.svg) **[!UICONTROL Create]**.
   1. Voer een **[!UICONTROL Report name]** in, bijvoorbeeld `Test Report` .
   1. Selecteer ![ FileCSV ](/help/assets/icons/FileCSV.svg) **[!UICONTROL Report]**.

   Een CSV-rapport met een titel die is gebaseerd op de door u opgegeven rapportnaam en huidige datum en tijd (bijvoorbeeld `Test Report_2025_04_23_9-5-18.csv`) wordt gedownload naar de standaarddownloadmap.

