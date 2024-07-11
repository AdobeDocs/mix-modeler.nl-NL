---
title: Gegevensregels
description: Leer hoe te om datasetregels te bepalen als deel van het harmoniseren van uw gegevens in Mix Modeler te gebruiken.
feature: Harmonized Data, Dataset Rules
exl-id: 57d7940a-2900-4814-a30d-bb02bff7615d
source-git-commit: 9085363e951a4e306c64ad28f56e2c15b4a6029a
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 0%

---

# Gegevensregels

De gegevenssetregels helpen u bij het in kaart brengen van uw geharmoniseerde gebieden met gebieden van de gegevens u in Mix Modeler hebt opgenomen.

* Voor geaggregeerde gegevens die u in Adobe Experience Platform hebt ingevoerd, wijst u een of meer van de beschikbare gegevenssetvelden toe aan de juiste geharmoniseerde velden.
* Voor gebeurtenisgegevens kunt u een of meer geharmoniseerde velden afzonderlijk toewijzen aan velden uit de gegevensset, rechtstreeks of met behulp van voorwaarden.


## Gegevenssetregels beheren

Om een lijst van de beschikbare datasetregels, in de interface van de Mix Modeler te zien:

1. Selecteren ![DataSearch](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized data]** van de linkerspoorstaaf.

1. Selecteren **[!UICONTROL Dataset rules]** in de bovenste balk. U ziet een lijst van de datasetregels.

De tabelkolommen geven details over de gegevenssetregels op:

| Kolomnaam | Details |
| ---------------------- | ----------|
| Gegevensset | De naam van de gegevensset. |
| Source | De bron van de gegevensset: Adobe Analytics, Experience Events, Summary (aggregaat) of Consumer Experience Events. |
| Schema | Het schema waaraan de dataset voldoet. U kunt de schemanaam snel selecteren om het schema in een nieuw lusje in de schemaredacteur in te openen ![Schema](/help/assets//icons/Schemas.svg) [Schemas](../ingest-data/schemas.md). |
| Korreligheid | De granulariteit van gegevens in de dataset. Mogelijke waarden zijn Dagelijks, Wekelijks, Maandelijks of Jaarlijks. |
| Begin van de week | Geeft aan welke dag van de week wordt beschouwd als het begin van een nieuwe week voor de specifieke gegevensset. |
| Status | De status van het veld: <p><span style="color:gray">●</span> Concept of <p><span style="color:green">●</span> Actief |
| Laatst gewijzigd | Gegevens en tijd van de laatste wijziging van de gegevenssetregel. |

{style="table-layout:auto"}

### Een gegevenssetregel maken

Om een datasetregel tot stand te brengen, in ![DataSearch](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** interface in Mix Modeler, selecteert u **[!UICONTROL Create a dataset rule]** in de **[!UICONTROL Dataset rules configuration]** wizard.

In de **[!UICONTROL Create]** scherm,

1. In **[!UICONTROL Dataset details]** selecteert u een gegevensset uit **[!UICONTROL Select dataset]** om met configuratie te beginnen. In de lijst worden datasets gecategoriseerd in **[!UICONTROL Consumer Experience Events]**, **[!UICONTROL Adobe Analytics]**, **[!UICONTROL Experience Event]** en **[!UICONTROL Summary]**.

1. Selecteer een dag voor de **[!UICONTROL Start of the week]**.

1. Selecteren **[!UICONTROL Daily]**, **[!UICONTROL Weekly]**, **[!UICONTROL Monthly]** of **[!UICONTROL Yearly]** for **[!UICONTROL Granularity]**.

1. Wanneer u een dataset van hebt geselecteerd **[!UICONTROL Summary]** categorie:

   1. Om te bepalen of de gegevens voor de dataset samenvoegen of bestaande gegevens vervangen, uitgezocht **[!UICONTROL Aggregation]** of **[!UICONTROL Replacement]** for **[!UICONTROL Data restatement is by]**.

   1. Wijs elk van de **[!UICONTROL Available dataset fields]** voor **[!UICONTROL Standard harmonized fields]** in **[!UICONTROL Map to harmonized fields]**. Als u een gegevenssetveld niet wilt toewijzen aan een geharmoniseerd veld, selecteert u expliciet **[!UICONTROL -- None --]**.

   1. Als u een nieuw geharmoniseerd veld nodig hebt dat niet beschikbaar is in de lijst, selecteert u **[!UICONTROL Create New]** een nieuw geharmoniseerd veld tot stand te brengen. U ziet het dialoogvenster zoals beschreven in [Een nieuw geharmoniseerd veld toevoegen](fields.md#add-a-harmonized-field).

   1. Wanneer de toewijzing voor alle gebieden voor de regel wordt voltooid, selecteer **[!UICONTROL Save as draft]** om een conceptversie van de regel op te slaan of **[!UICONTROL Save]** om de regel op te slaan en te activeren. Selecteren **[!UICONTROL Cancel]** om de regelconfiguratie te annuleren.

      ![Gegevenssetregels maken](/help/assets//dataset-create-summary.png)

1. Als u een gegevensset met gebeurteniscategorieën hebt geselecteerd (**[!UICONTROL Experience Events]**, **[!UICONTROL Adobe Analytics]**, **[!UICONTROL Consumer Experience Events]**), in het vak eronder **[!UICONTROL Map to harmonized fields]**:

   1. Een geharmoniseerd veld selecteren vanuit **[!UICONTROL Standard harmonized field]**.

   1. Wanneer het geselecteerde geharmoniseerde veld metrisch is:

      1. Selecteren **[!UICONTROL Count]** of **[!UICONTROL Sum]** van **[!UICONTROL Mapping type]**.

      1. Selecteer een **[!UICONTROL *Veld voor AEP-gegevensset *]**dat u het geharmoniseerde veld standaard wilt koppelen.

   1. Wanneer het geselecteerde veld van het type afmeting is:

      1. Selecteren **[!UICONTROL Map Into]** of **[!UICONTROL Case]** van **[!UICONTROL Mapping type]**.

      1. Wanneer u **[!UICONTROL Map Into]**, selecteert u **[!UICONTROL Field]** en **[!UICONTROL *Veld voor AEP-gegevensset *]**of **[!UICONTROL Value]**en een standaardwaarde om het geharmoniseerde veld standaard toe te wijzen aan het gegevenssetveld of de ingevoerde waarde.

      1. Wanneer u **[!UICONTROL Case]**, selecteert u **[!UICONTROL Field]** en **[!UICONTROL *Veld voor AEP-gegevensset *]**of **[!UICONTROL Value]**en een standaardwaarde om het geharmoniseerde veld standaard toe te wijzen aan het gegevenssetveld of de ingevoerde waarde.

         1. Als u waarden expliciet wilt instellen, definieert u een of meer gevallen, die uit een of meer voorwaarden bestaan. Elke voorwaarde kan controleren op een specifieke **[!UICONTROL *Veld voor AEP-gegevensset *]**of **[!UICONTROL Exists]**of **[!UICONTROL Not Exists]**of **[!UICONTROL Contains]**,**[!UICONTROL Not Contains]**,**[!UICONTROL Equals]**,**[!UICONTROL Not Equals]**,**[!UICONTROL Starts With]**, of **[!UICONTROL Ends With]**een waarde ingevoerd om**[!UICONTROL * Voer de invoerwaarde in *]**.

         1. Selecteer ![Toevoegen](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add case]** selecteert u ![Toevoegen](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add condition]**.

         1. Als u een hoofdletter of voorwaarde wilt verwijderen, selecteert u ![Sluiten](/help/assets//icons/Close.svg) in de bijbehorende container.

         1. Om te selecteren of om het even welke of alle voorwaarden voor een geval zouden moeten van toepassing zijn, selecteer **[!UICONTROL Any of]** of **[!UICONTROL All of]**.

         1. Voer de waarde in op **[!UICONTROL Then]**.

      Het onderstaande voorbeeld

      * gebruikt een **[!UICONTROL Map Into]** **[!UICONTROL Mapping type]** om de **[!UICONTROL Channel Type At Source]** het geharmoniseerde gebied **[!UICONTROL channel_type]** veld van de **[!DNL Luma Transactions]** dataset.

      * gebruikt een **[!UICONTROL Case]** **[!UICONTROL Mapping type]** om de waarde van de **[!UICONTROL marketing.campaignName]** in het veld **[!DNL Luma Transactions]** gegevensset aan de **[!UICONTROL Campaign]** geharmoniseerd veld. Het geharmoniseerde veld Campagne is ingesteld op:

         * `Black Friday` wanneer de **[!UICONTROL marketing.campaignName]** is `_black_friday` of `BlackFriday`.
         * op de waarde van de **[!UICONTROL marketing.campaignName]** in alle andere gevallen.

        ![Dataset-regelgebeurtenis](/help/assets//dataset-create-event.png)

1. Selecteren ![Toevoegen](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add field]** om extra velden te definiëren.

Selecteer **[!UICONTROL Save as draft]** om een conceptversie van de regel op te slaan of **[!UICONTROL Save]** om de regel op te slaan en te activeren. Selecteren **[!UICONTROL Cancel]** om de regelconfiguratie te annuleren.


### Een gegevenssetregel bewerken

Om een datasetregel uit te geven, in ![DataSearch](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** interface in Mix Modeler:

1. Selecteren ![Meer](/help/assets//icons/More.svg) in de **[!UICONTROL Dataset]** kolom voor de datasetregel die u wilt uitgeven.
1. Selecteer in het contextmenu de optie ![Bewerken](/help/assets//icons/Edit.svg) **[!UICONTROL Edit]** om de gegevenssetregel te gaan bewerken. Zie [Een gegevenssetregel maken](#create-a-dataset-rule) voor meer informatie .


### Een gegevenssetregel verwijderen

Om een datasetregel te schrappen, in ![DataSearch](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** interface in Mix Modeler:

1. Selecteren ![Meer](/help/assets//icons/More.svg) in de **[!UICONTROL Dataset]** kolom voor de datasetregel die u wilt schrappen.
1. Selecteer in het contextmenu de optie ![Verwijderen](/help/assets//icons/Delete.svg) **[!UICONTROL Delete]** om de datasetregel te schrappen. U wordt om bevestiging gevraagd. Selecteren **[!UICONTROL Delete]** om de geselecteerde datasetregel permanent te schrappen.


## Gegevens synchroniseren

Om gegevens tussen uw geharmoniseerde gegevens en samenvatting en/of gebeurtenisdatasets, na alle logica in uw datasetregels te synchroniseren:

1. Selecteren **[!UICONTROL Sync data]**.

1. Van de **[!UICONTROL Sync data for dataset rules]** dialoogvenster, selecteert u
   * **[!UICONTROL Refresh harmonized data for summary datasets]**,
   * **[!UICONTROL Refresh harmonized data for event datasets]**, of
   * **[!UICONTROL Refresh harmonized data for both summary + event datasets]**.

1. Selecteer **[!UICONTROL Sync]**. Selecteer **[!UICONTROL Cancel]**.

   ![Gegevens synchroniseren](/help/assets//sync-data.png)


## Voorkeuren voor gegevenssamenvoeging

>[!NOTE]
>
>[!BADGE bèta]{type=Informative}

Voorkeuren voor gegevenssamenvoeging helpen u conflicten op te lossen wanneer gegevens uit een overzicht en gebeurtenisgegevensbronnen worden samengevoegd. Gebruiksscenario&#39;s zijn:

* dezelfde advertentiemetrie in meerdere gegevensreeksen wordt gemeten en gerapporteerd, of
* metrische metingen kunnen in sommige gegevensreeksen onvolledig zijn, terwijl een andere dataset een superset van een bepaalde metrische waarde kan zijn, resulterend in dubbeltelling.

Voor nauwkeurige modelvoorspelling kunt u voorkeuren voor gegevenssamenvoeging definiëren:

1. Selecteren ![Voorkeuren voor gegevenssamenvoeging](/help/assets//icons/Merge.svg) [!BADGE bèta].

1. In de **[!UICONTROL Data merge preferences]** [!BADGE bèta]{type=Informative}

   ![Voorkeuren voor gegevenssamenvoeging](/help/assets//data-merge-preferences.png)

   * Selecteer een **[!UICONTROL Default metric preference]**. De geselecteerde standaard metrische voorkeur wordt toegepast wanneer, tijdens harmonisatie, de veelvoudige bronnen van gegevens een metrisch gebied voor een bepaald kanaal bijwerken. De voorkeur wordt toegepast op het niveau van de zandbak, tenzij met voeten getreden voor specifieke metrische gebaseerde voorkeur. U kunt kiezen tussen **[!UICONTROL Summary data]**, **[!UICONTROL Event data]** en **[!UICONTROL Sum of summmary and event data]**.

   * Specifieke op metrische basis gebaseerde voorkeuren toevoegen:

      1. Selecteren ![Plus](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add a metric]**.
         1. Selecteer een metrische waarde in het menu **[!UICONTROL *Metrische selectie *]**lijst.
         1. Selecteren **[!UICONTROL CHANNELS]** of **[!UICONTROL CONVERSION TYPES]**. Selecteer in de lijst **[!UICONTROL All]** of een specifiek kanaal of conversietype.
         1. Selecteren **[!UICONTROL Summary]** of **[!UICONTROL Event]** om op te geven of summiere gegevens of gebeurtenisgegevens bij het samenvoegen van gegevens de voorkeur hebben voor de metrische gegevens (en voor alle gegevens of voor het geselecteerde kanaal).

         Een of meer extra kanaal- of conversietypen toevoegen:

         1. Selecteren ![Plus](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add a channel]** of ![Plus](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add a conversion type]**.
         1. Selecteren **[!UICONTROL Summary]** of **[!UICONTROL Event]**.

         Als u een kanaal of conversietype wilt verwijderen, selecteert u ![Kruisje](/help/assets//icons/Close.svg).

      1. Herhaal de vorige stap als u meer specifieke, op metrische basis gebaseerde voorkeuren wilt toevoegen.

   * Als u een bestaande, specifieke voorkeur op basis van metrische gegevens wilt verwijderen, selecteert u ![Verwijderen](/help/assets//icons/Delete.svg).

1. Selecteren **[!UICONTROL Save]** om de voorkeuren voor gegevenssamenvoeging op te slaan. De gegevens worden opnieuw gesynchroniseerd. <br/>Selecteren **[!UICONTROL Cancel]** om te annuleren.


## Toegangsbeheer op veldniveau

Wanneer het vormen van datasetregels voor geharmoniseerde datasets, Experience Platform [kenmerkgebaseerd toegangsbeheer](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview) wordt afgedwongen op veldniveau. Een gebied wordt beperkt wanneer een etiket aan een schemagebied in bijlage is en een actief beleid wordt toegelaten dat toegang voor u tot dat gebied ontkent. Dientengevolge:

* u ziet niet de schemagebieden die voor u beperkt zijn wanneer u een datasetregel creeert,
* u kunt de afbeelding van een of meer schemavelden die voor u zijn beperkt, niet weergeven of bewerken. Wanneer u een datasetregel uitgeeft of bekijkt die dergelijke beperkte gebieden bevat, ziet u het volgende scherm.
  ![Actie niet toegestaan](/help/assets//action-not-permitted.png)
