---
title: Gegevens harmoniseren
description: Leer hoe u gegevens in de Mix Modeler kunt harmoniseren.
feature: Harmonized Data
exl-id: 6cb70762-e3b2-46a0-b028-1d6daf3edae5
source-git-commit: 33883626d8e7aca2eecc3571593be53ef41ac458
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 9%

---

# Gegevens harmoniseren

De gegevens in Mix Modeler zijn van verschillende aard afhankelijk van de gegevensbron. De gegevens kunnen zijn:

* geaggregeerde of samenvattende gegevens, bijvoorbeeld verzameld uit zogenaamde tuingegevensbronnen of offline advertentiegegevens die (zoals het uitgeven) zijn verzameld uit het voeren van een billboardcampagne, een evenement of een fysieke advertentiecampagne;
* gebeurtenisgegevens, bijvoorbeeld uit gegevensbronnen van de eerste partij. Deze gebeurtenisgegevens kunnen worden verzameld via de Adobe Analytics-bronconnector van Adobe Analytics, of via het Experience Platform Web of Mobile SDK of Edge Network API, of via gegevens die via bronconnectors worden ingevoerd.

De harmonisatiedienst van Mix Modeler vergelijkt de geaggregeerde gegevens en de gebeurtenisgegevens in een consistent gegevensoverzicht. Deze gegevensmening is de bron voor de plannen en de modellen in Mix Modeler.

## Een voorbeeld van geharmoniseerde gegevens

Stel dat u de volgende datasets beschikbaar hebt voor Mix Modeler.

**Dataset 1**

Bevat een gegevensset van de marketinginspanning van YouTube, met een granulariteit van de geaggregeerde gegevensset tot dagelijks.

| Datum | Datumtype | Kanaal | Campaign | Merk | Geo | Klikken | Draaien |
|---|:--:|---|---|---|---|---:|---:|
| 12-31-2021 | dag | YouTube | Y_Fall_02 | MerkX | VS | 10000 | 100 |
| 01-01-2022 | dag | YouTube | Y_Fall_02 | MerkX | VS | 1000 | 10 |
| 01-03-2022 | dag | YouTube | Y_Fall_01 | MerkY | CA | 10000 | 100 |
| 01-04-2022 | dag | YouTube | Y_Summer_01 | Null | CA | 9000 | 80 |

{style="table-layout:auto"}


**Gegevensset 2**

Bevat een gegevensset van de marketinginspanning van Facebook, met een granulariteit van de geaggregeerde gegevensset tot wekelijks.

| Datum | Datumtype | Kanaal | Campaign | Geo | Klikken | Draaien |
|--- |:---:|--- |---|---|---:|---:|
| 01-01-2022 | week | Facebook | FB_Fall_01 | VS | 8000 | 100 |
| 01-08-2022 | week | Facebook | FB_Fall_02 | VS | 1000 | 10 |
| 01-08-2022 | week | Facebook | FB_Fall_01 | VS | 7000 | 100 |
| 01-16-2022 | week | Facebook | FB_Summer_01 | CA | 10000 | 80 |

{style="table-layout:auto"}


**Gegevensset 3**

Een omzettingsdataset, met een granulariteit van de samengevoegde gegevensreeks aan dagelijks.

| Datum | Datumtype | Geo | Goal | Ontvangsten |
|--- |:---: |---|---|---:|
| 01-01-2022 | dag | VS | Mode | 200 |
| 01-08-2022 | dag | VS | Mode | 10 |
| 01-08-2022 | dag | VS | Juwelen | 1100 |
| 01-16-2022 | dag | CA | Juwelen | 80 |

{style="table-layout:auto"}


**Gegevensset 4**

Een dataset van de steekproefervaringsgebeurtenis (de gebeurtenissen van SDK van het Web) van de klant.

| Tijdstempel | Naamruimte van identiteit | Identiteitskaart | Kanaal | Klikken |
|--- |--- |--- |--- |---:|
| 01-01-2022 00:01:01.000 | ECID | 64fd46ff-8c63-43b4-85a7-92b953113ba0 | CSE | 1 |
| 01-01-2022 00:01:01.000 | ECID | 64fd46ff-8c63-43b4-85a7-92b953113ba0 | CSE | 1 |
| 01-08-2022 00:01:01.000 | ECID | 2ca2a16e-caf0-4fa9-9a8b-9774b39547c4 | CSE | 1 |
| 01-08-2022 00:01:01.000 | ECID | 5ce99bfb-e44a-40d9-b8cd-c5408bda7cdc | CSE | 1 |

{style="table-layout:auto"}


U wilt een geharmoniseerde dataset bouwen, met een granulariteit die aan wekelijkse wordt geplaatst. De gebeurtenisgegevens worden geaggregeerd naar weekgranulariteit en toegevoegd aan de geharmoniseerde gegevensset. Het resultaat is:

**Geharmoniseerde gegevensset**

| Datum | Datumtype | Kanaal | Campaign | Merk | Geo | Goal | Klikken | Draaien | Ontvangsten |
|--- |:---:|--- |--- |--- |---|---|---:|---:|---:|
| 12-27-2021 | week | YouTube | Y_Fall_02 | MerkX | VS | Null | 11000 | 110 | Null |
| 01-03-2022 | week | YouTube | Y_Fall_01 | MerkY | CA | Null | 10000 | 100 | Null |
| 01-03-2022 | week | YouTube | Y_Summer_01 | Null | CA | Null | 9000 | 80 | Null |
| 01-01-2022 | week | Facebook | FB_Fall_01 | Null | VS | Null | 8000 | 100 | Null |
| 01-08-2022 | week | Facebook | FB_Fall_02 | Null | VS | Null | 1000 | 10 | Null |
| 01-08-2022 | week | Facebook | FB_Fall_01 | Null | VS | Null | 7000 | 100 | Null |
| 01-16-2022 | week | Facebook | FB_Summer_01 | Null | CA | Null | 10000 | 80 | Null |
| 12-27-2021 | week | Null | Null | Null | VS | Mode | Null | Null | 200 |
| 01-03-2022 | week | Null | Null | Null | VS | Mode | Null | Null | 10 |
| 01-03-2022 | week | Null | Null | Null | VS | Juwelen | Null | Null | 1100 |
| 01-10-2022 | week | Null | Null | Null | CA | Juwelen | Null | Null | 80 |
| 01-01-2022 | week | CSE | Null | Null | Null | Null | 2 | Null | Null |
| 01-08-2022 | week | CSE | Null | Null | Null | Null | 2 | Null | Null |

{style="table-layout:auto"}


## geharmoniseerde gegevens instellen

Om een geharmoniseerde dataset te bouwen, zoals in vereenvoudigde [voorbeeld](#an-example-of-harmonized-data), moet u deze stappen volgen:

1. Extra definiëren [geharmoniseerde velden](fields.md) die u buiten de reeds beschikbare globale geharmoniseerde gebieden wilt gebruiken.
1. Instellen [gegevenssetregels](dataset-rules.md) om velden van uw aggregaat of ervaringsgegevenssets toe te wijzen aan geharmoniseerde velden.
1. Definiëren [marketingaanraakpunten](marketing-touchpoints.md) met de standaard en aanvullende geharmoniseerde velden die u hebt gedefinieerd.
1. Definiëren [conversies](conversions.md) met de standaard en aanvullende geharmoniseerde velden die u hebt gedefinieerd.


## Geharmoniseerde gegevens weergeven

Om uw geharmoniseerde gegevens te zien, in de interface van de Mix Modeler:

1. Selecteren ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized datasets]** van de linkerspoorstaaf.

1. Selecteren **[!UICONTROL Harmonized Data]** in de bovenste balk. U ziet een overzicht van uw geharmoniseerde gegevens die op de gebieden, datasetregels, marketing touchpoints en omzettingen worden gebaseerd u hebt bepaald.

   1. Om de periode te herdefiniëren waarop de samenloop van geharmoniseerde gegevens is gebaseerd, voert u een datumbereik in voor **[!UICONTROL Date range]** of gebruik ![Kalender](../assets/icons/Calendar.svg) om een gegevensbereik te selecteren.

   1. Als u de geharmoniseerde veldkolommen voor de tabel met geharmoniseerde gegevens wilt wijzigen, gebruikt u ![Instellingen](../assets/icons/Setting.svg) om de **[!UICONTROL Column settings]** in.

      1. Selecteren ![SelectBox](../assets/icons/SelectBox.svg) een of meer kolommen van **[!UICONTROL AVAILABLE COLUMNS]** en gebruik ![Chevron right](../assets/icons/ChevronRight.svg) deze kolommen toevoegen aan **[!UICONTROL SELECTED COLUMNS]**.

      1. Selecteren ![SelectBox](../assets/icons/SelectBox.svg) een of meer kolommen van **[!UICONTROL SELECTED COLUMNS]** en gebruik ![Chevron left](../assets/icons/ChevronLeft.svg) om de geselecteerde kolommen te verwijderen en deze kolommen terug te keren naar **[!UICONTROL AVAILABLE COLUMNS]**.

      1. Een kolom selecteren uit **[!UICONTROL DEFAULT SORT]** en schakelen tussen **[!UICONTROL Ascending]** of **[!UICONTROL Descending]**.

      1. Als u de volgorde van de weergegeven kolommen wilt wijzigen, kunt u een kolom verplaatsen in **[!UICONTROL SELECTED COLUMNS]** omhoog en omlaag door slepen en neerzetten.

   1. Selecteren **[!UICONTROL Submit]** om de wijzigingen in de kolominstelling te verzenden. Selecteren **[!UICONTROL Close]** om de aangebrachte wijzigingen te annuleren.
