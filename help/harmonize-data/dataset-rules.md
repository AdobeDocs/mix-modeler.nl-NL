---
title: Gegevensregels
description: Leer hoe te om datasetregels te bepalen als deel van het harmoniseren van uw gegevens in Mix Modeler te gebruiken.
feature: Harmonized Data, Dataset Rules
exl-id: 57d7940a-2900-4814-a30d-bb02bff7615d
source-git-commit: 86732fe30637aa72ced232d9f331a3cc64baa39b
workflow-type: tm+mt
source-wordcount: '980'
ht-degree: 0%

---

# Gegevensregels

De gegevenssetregels helpen u bij het in kaart brengen van uw geharmoniseerde gebieden met gebieden van de gegevens u in Mix Modeler hebt opgenomen.

* Voor geaggregeerde gegevens die u in Adobe Experience Platform hebt ingevoerd, wijst u een of meer van de beschikbare gegevenssetvelden toe aan de juiste geharmoniseerde velden.
* Voor gebeurtenisgegevens kunt u een of meer geharmoniseerde velden afzonderlijk toewijzen aan velden uit de gegevensset, rechtstreeks of met behulp van voorwaarden.


## Gegevenssetregels beheren

Om een lijst van de beschikbare datasetregels, in de interface van de Mix Modeler te zien:

1. Selecteren ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** van de linkerspoorstaaf.

1. Selecteren **[!UICONTROL Dataset rules]** in de bovenste balk. U ziet een lijst van de datasetregels.

De tabelkolommen geven details over de gegevenssetregels op:

| Kolomnaam | Details |
| ---------------------- | ----------|
| Gegevensset | De naam van de gegevensset. |
| Bron | De bron van de dataset, die Adobe Analytics, de Gebeurtenissen van de Ervaring, Samenvatting (bijeengevoegde), of de Gebeurtenissen van de Ervaring van de Consumenten kan zijn. |
| Schema | Het schema waaraan de dataset voldoet. U kunt de schemanaam snel selecteren om het schema in een nieuw lusje in de schemaredacteur in Mix Modeler te openen - Schema&#39;s. |
| Korreligheid | De granulariteit van gegevens in de dataset. Mogelijke waarden zijn Dagelijks, Wekelijks, Maandelijks of Jaarlijks. |
| Begin van de week | Geeft aan welke dag van de week wordt beschouwd als het begin van een nieuwe week voor de specifieke gegevensset. |
| Status | De status van het veld: <p><span style="color:gray">●</span> Concept of <p><span style="color:green">●</span> Actief |
| Laatst gewijzigd | Gegevens en tijd van de laatste wijziging van de gegevenssetregel. |

{style="table-layout:auto"}

### Een gegevenssetregel maken

Om een datasetregel tot stand te brengen, in ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** interface in Mix Modeler, selecteert u **[!UICONTROL Create Dataset rule]** in de **[!UICONTROL Dataset rules configuration]** wizard.

In de **[!UICONTROL Create]** scherm,

1. In **[!UICONTROL Dataset details]** selecteert u een gegevensset uit **[!UICONTROL Select dataset]** om met configuratie te beginnen. In de lijst worden datasets gecategoriseerd in **[!UICONTROL Consumer Experience Events]**, **[!UICONTROL Adobe Analytics]**, **[!UICONTROL Experience Event]** en **[!UICONTROL Summary]**.

1. Selecteer een dag voor de **[!UICONTROL Start of the week]**.

1. Selecteren **[!UICONTROL Daily]**, **[!UICONTROL Weekly]**, **[!UICONTROL Monthly]** of **[!UICONTROL Yearly]** for **[!UICONTROL Granularity]**.

1. Wanneer u een dataset van hebt geselecteerd **[!UICONTROL Summary]** categorie:

   1. Wijs elk van de **[!UICONTROL Available dataset fields]** voor **[!UICONTROL Standard harmonized fields]** in **[!UICONTROL Map to harmonized fields]**. Als u een gegevenssetveld niet wilt toewijzen aan een geharmoniseerd veld, selecteert u expliciet **[!UICONTROL -- None --]**.

   1. Als u een nieuw geharmoniseerd veld nodig hebt dat niet beschikbaar is in de lijst, selecteert u **[!UICONTROL Create New]** een nieuw geharmoniseerd veld tot stand te brengen. U ziet het dialoogvenster zoals beschreven in [Een nieuw geharmoniseerd veld toevoegen](fields.md#add-a-harmonized-field) om snel een nieuw geharmoniseerd veld toe te voegen.

   1. Wanneer de toewijzing voor alle gebieden voor de regel wordt voltooid, selecteer **[!UICONTROL Save as draft]** om een conceptversie van de regel op te slaan of **[!UICONTROL Save]** om de regel op te slaan en te activeren.  Selecteren **[!UICONTROL Cancel]** om de regelconfiguratie te annuleren.

      ![Gegevenssetregels maken](../assets/dataset-create-summary.png)

1. Als u een gegevensset met gebeurteniscategorieën hebt geselecteerd (**[!UICONTROL Experience Events]**, **[!UICONTROL Adobe Analytics]**, **[!UICONTROL Consumer Experience Events]**), in het vak eronder **[!UICONTROL Map to harmonized fields]**:

   1. Een geharmoniseerd veld selecteren vanuit **[!UICONTROL Standard harmonized field]**.

   1. Wanneer het geselecteerde geharmoniseerde veld metrisch is:

      1. Selecteren **[!UICONTROL Count]** of **[!UICONTROL Sum]** van **[!UICONTROL Mapping type]**.

      1. Selecteer een **[!UICONTROL *Veld voor AEP-gegevensset *]**dat u het geharmoniseerde veld standaard wilt koppelen.

   1. Wanneer het geselecteerde veld van het type afmeting is:

      1. Selecteren **[!UICONTROL Map Into]** of **[!UICONTROL Case]** van **[!UICONTROL Mapping type]**.

      1. Wanneer u **[!UICONTROL Map Into]**, selecteert u **[!UICONTROL Field]** en **[!UICONTROL *Veld voor AEP-gegevensset *]**of **[!UICONTROL Value]**en een standaardwaarde om het geharmoniseerde veld standaard toe te wijzen aan het gegevenssetveld of de ingevoerde waarde.

      1. Wanneer u **[!UICONTROL Case]**, selecteert u **[!UICONTROL Field]** en **[!UICONTROL *Veld voor AEP-gegevensset *]**of **[!UICONTROL Value]**en een standaardwaarde om het geharmoniseerde veld standaard toe te wijzen aan het gegevenssetveld of de ingevoerde waarde.

         1. Bovendien definieert u een of meer gevallen, die bestaan uit een of meer voorwaarden om expliciet waarden in te stellen. Elke voorwaarde kan controleren op een specifieke **[!UICONTROL *Veld voor AEP-gegevensset *]**of **[!UICONTROL Exists]**of **[!UICONTROL Not Exists]**of **[!UICONTROL Contains]**,**[!UICONTROL Not Contains]**,**[!UICONTROL Equals]**,**[!UICONTROL Not Equals]**,**[!UICONTROL Starts With]**, of **[!UICONTROL Ends With]**een waarde ingevoerd om**[!UICONTROL * Voer de invoerwaarde in *]**.

         1. Selecteer ![Toevoegen](../assets/icons/AddCircle.svg) **[!UICONTROL Add case]** selecteert u ![Toevoegen](../assets/icons/AddCircle.svg) **[!UICONTROL Add condition]**.

         1. Als u een hoofdletter of voorwaarde wilt verwijderen, selecteert u ![Sluiten](../assets/icons/Close.svg) in de bijbehorende container.

         1. Om te selecteren of om het even welke of alle voorwaarden voor een geval zouden moeten van toepassing zijn, selecteer **[!UICONTROL Any of]** of **[!UICONTROL All of]**.

         1. Voer de waarde in op **[!UICONTROL Then]**.

      Het onderstaande voorbeeld

      * gebruikt een **[!UICONTROL Map Into]** **[!UICONTROL Mapping type]** om de **[!UICONTROL Channel Type At Source]** het geharmoniseerde gebied **[!UICONTROL channel_type]** veld van de **[!DNL Luma Transactions]** dataset.

      * gebruikt een **[!UICONTROL Case]** **[!UICONTROL Mapping type]** om de waarde van de **[!UICONTROL marketing.campaignName]** in het veld **[!DNL Luma Transactions]** gegevensset aan de **[!UICONTROL Campaign]** geharmoniseerd veld. Het geharmoniseerde veld Campagne is ingesteld op:

         * `Black Friday` wanneer de **[!UICONTROL marketing.campaignName]** is `_black_friday` of `BlackFriday`.
         * op de waarde van de **[!UICONTROL marketing.campaignName]** in alle andere gevallen.

        ![Dataset-regelgebeurtenis](../assets/dataset-create-event.png)

1. Selecteren ![Toevoegen](../assets/icons/AddCircle.svg) **[!UICONTROL Add field]** om extra velden te definiëren.

Als u klaar bent, selecteert u **[!UICONTROL Save as draft]** om een conceptversie van de regel op te slaan of **[!UICONTROL Save]** om de regel op te slaan en te activeren.  Selecteren **[!UICONTROL Cancel]** om de regelconfiguratie te annuleren.


### Een gegevenssetregel bewerken

Om een datasetregel uit te geven, in ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** interface in Mix Modeler:

1. Selecteren ![Meer](../assets/icons/More.svg) in de **[!UICONTROL Dataset]** kolom voor de datasetregel die u wilt uitgeven.
1. Selecteer in het contextmenu de optie ![Bewerken](../assets/icons/Edit.svg) **[!UICONTROL Edit]** om de gegevenssetregel te gaan bewerken. Zie [Een gegevenssetregel maken](#create-a-dataset-rule) voor meer informatie .


### Een gegevenssetregel verwijderen

Om een datasetregel te schrappen, in ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** interface in Mix Modeler:

1. Selecteren ![Meer](../assets/icons/More.svg) in de **[!UICONTROL Dataset]** kolom voor de datasetregel die u wilt schrappen.
1. Selecteer in het contextmenu de optie ![Verwijderen](../assets/icons/Delete.svg) **[!UICONTROL Delete]** om de datasetregel te schrappen. U wordt gevraagd dit te bevestigen. Selecteren **[!UICONTROL Delete]** om de geselecteerde datasetregel permanent te schrappen.


## Gegevens synchroniseren

Om gegevens tussen uw geharmoniseerde gegevens en samenvatting en/of gebeurtenisdatasets, na alle logica in uw datasetregels te synchroniseren:

1. Selecteren **[!UICONTROL Sync data]**.

1. Van de **[!UICONTROL Sync data for dataset rules]** dialoogvenster selecteert u een van de **[!UICONTROL Refresh harmonized data for summary datasets]**, **[!UICONTROL Refresh harmonized data for event datasets]**, of **[!UICONTROL Refresh harmonized data for both summary + event datasets]**.

1. Selecteren **[!UICONTROL Sync]** om de synchronisatie te starten op basis van de gedefinieerde gegevenssetregels tussen geharmoniseerde gegevens en gegevens in gegevensreeksen. Selecteer **[!UICONTROL Cancel]**.

   ![Gegevens synchroniseren](../assets/sync-data.png)


## Voorkeuren voor gegevenssamenvoeging

U kunt voorkeuren definiëren om conflicten op te lossen als gegevens uit een overzicht en gebeurtenisbronnen worden samengevoegd. Dit doet u als volgt:

1. Selecteren ![Voorkeuren voor gegevenssamenvoeging](../assets/icons/Merge.svg) **Voorkeuren voor gegevenssamenvoeging**.

1. In de **[!UICONTROL Data merge preferences]** dialoogvenster:

   ![Voorkeuren voor gegevenssamenvoeging](../assets/data-merge-preferences.png)

   1. Selecteer een standaardmetrische voorkeur van **[!UICONTROL Default metric preference]** lijst. <p>Een standaardvoorkeur wordt toegepast wanneer tijdens harmonisatie, veelvoudige bronnen van gegevens proberen om een metrisch gebied voor een bepaald kanaal bij te werken. Deze voorkeur wordt toegepast op het niveau van de zandbak tenzij met voeten getreden voor bepaalde metrische voorkeur die bij wordt bepaald **[!UICONTROL Metric based preference]**.

   1. Gebruiken ![Plus](../assets/icons/AddCircle.svg) **[!UICONTROL Add a metric]**, om een of meer van de onderstaande cijfers toe te voegen **[!UICONTROL Metric based preference]**.



      * Selecteer een metrische waarde in het menu **[!UICONTROL _Metrische selectie_]** lijst, en
      * Selecteren **[!UICONTROL Summary]** of **[!UICONTROL Event]**.

      Gebruiken ![Verwijderen](../assets/icons/Close.svg) om een item uit de lijst te verwijderen.

   1. Selecteren **[!UICONTROL Save]** om de voorkeuren voor gegevenssamenvoeging op te slaan. Selecteren **[!UICONTROL Cancel]** om te annuleren.
