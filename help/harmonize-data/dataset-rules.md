---
title: Gegevensregels
description: Leer hoe te om datasetregels te bepalen als deel van het harmoniseren van uw gegevens in Mix Modeler te gebruiken.
feature: Harmonized Data, Dataset Rules
exl-id: 57d7940a-2900-4814-a30d-bb02bff7615d
source-git-commit: 9a6c1f1c12ab29da80a1997cfd31ca07b38eaa22
workflow-type: tm+mt
source-wordcount: '1313'
ht-degree: 0%

---

# Gegevensregels

De gegevenssetregels helpen u bij het in kaart brengen van uw geharmoniseerde gebieden met gebieden van de gegevens u in Mix Modeler hebt opgenomen.

* Voor geaggregeerde gegevens die u in Adobe Experience Platform hebt ingevoerd, wijst u een of meer van de beschikbare gegevenssetvelden toe aan de juiste geharmoniseerde velden.
* Voor gebeurtenisgegevens kunt u een of meer geharmoniseerde velden afzonderlijk toewijzen aan velden uit de gegevensset, rechtstreeks of met behulp van voorwaarden.


## Gegevenssetregels beheren

Om een lijst van de beschikbare datasetregels, in de interface van de Mix Modeler te zien:

1. Selecteer ![ DataSearch ](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** van het linkerspoor.

1. Selecteer **[!UICONTROL Dataset rules]** in de bovenste balk. U ziet een lijst van de datasetregels.

De tabelkolommen geven details over de gegevenssetregels op:

| Kolomnaam | Details |
| ---------------------- | ----------|
| Gegevensset | De naam van de gegevensset. |
| Source | De bron van de gegevensset: Adobe Analytics, Experience Events, Summary (aggregaat) of Consumer Experience Events. |
| Schema | Het schema waaraan de dataset voldoet. U kunt de schemanaam snel selecteren om het schema in een nieuw lusje in de schemaredacteur in ](/help/assets/icons/Schemas.svg) Schema [ Schema&#39;s ](../ingest-data/schemas.md) te openen.![ |
| Korreligheid | De granulariteit van gegevens in de dataset. Mogelijke waarden zijn Dagelijks, Wekelijks, Maandelijks of Jaarlijks. |
| Begin van de week | Geeft aan welke dag van de week wordt beschouwd als het begin van een nieuwe week voor de specifieke gegevensset. |
| Status | De status van het veld: <p><span style="color:gray"> ・</span> Concept of <p><span style="color:green"> ・</span> Actief |
| Laatst gewijzigd | Gegevens en tijd van de laatste wijziging van de gegevenssetregel. |

{style="table-layout:auto"}

### Een gegevenssetregel maken

Om een datasetregel tot stand te brengen, in ![ DataSearch ](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** interface in Mix Modeler, selecteer **[!UICONTROL Create a dataset rule]** in de **[!UICONTROL Dataset rules configuration]** tovenaar.

In het **[!UICONTROL Create]** -scherm

1. Selecteer in **[!UICONTROL Dataset details]** een gegevensset in **[!UICONTROL Select dataset]** om de configuratie te starten. In de lijst worden datasets gecategoriseerd in **[!UICONTROL Consumer Experience Events]** , **[!UICONTROL Adobe Analytics]** , **[!UICONTROL Experience Event]** en **[!UICONTROL Summary]** .

1. Selecteer een dag voor **[!UICONTROL Start of the week]**.

1. Selecteer **[!UICONTROL Daily]** , **[!UICONTROL Weekly]** , **[!UICONTROL Monthly]** of **[!UICONTROL Yearly]** for **[!UICONTROL Granularity]** .

1. Wanneer u een dataset van de **[!UICONTROL Summary]** categorie hebt geselecteerd:

   1. Selecteer **[!UICONTROL Aggregation]** of **[!UICONTROL Replacement]** for **[!UICONTROL Data restatement is by]** om te bepalen of gegevens voor de gegevensset bestaande gegevens aggregeren of vervangen.

   1. Wijs elk van de **[!UICONTROL Available dataset fields]** toe aan de overeenkomende **[!UICONTROL Standard harmonized fields]** in **[!UICONTROL Map to harmonized fields]** . Als u een gegevenssetveld niet wilt toewijzen aan een geharmoniseerd veld, selecteert u expliciet **[!UICONTROL -- None --]** .

   1. Als u een nieuw geharmoniseerd veld nodig hebt dat niet in de lijst beschikbaar is, selecteert u **[!UICONTROL Create New]** om een nieuw geharmoniseerd veld te maken. U ziet de dialoog zoals geschetst in [ een nieuw geharmoniseerd gebied ](fields.md#add-a-harmonized-field) toevoegen.

   1. Wanneer de toewijzing voor alle gebieden voor de regel wordt voltooid, uitgezocht **[!UICONTROL Save as draft]** om een ontwerp versie van de regel te bewaren of **[!UICONTROL Save]** om de regel te bewaren en te activeren. Selecteer **[!UICONTROL Cancel]** om de regelconfiguratie te annuleren.

      ![ creeer datasetregels ](/help/assets/dataset-create-summary.png)

1. Wanneer u een gegevensset met gebeurteniscategorieën (**[!UICONTROL Experience Events]**, **[!UICONTROL Adobe Analytics]**, **[!UICONTROL Consumer Experience Events]**) hebt geselecteerd in het vak onder **[!UICONTROL Map to harmonized fields]** :

   1. Selecteer een geharmoniseerd veld in **[!UICONTROL Standard harmonized field]** .

   1. Wanneer het geselecteerde geharmoniseerde veld metrisch is:

      1. Selecteer **[!UICONTROL Count]** of **[!UICONTROL Sum]** vanuit **[!UICONTROL Mapping type]** .

      1. Selecteer een **[!UICONTROL *gebied van de dataset van AEP *]**dat u het geharmoniseerde gebied aan door gebrek wilt in kaart brengen.

   1. Wanneer het geselecteerde veld van het type afmeting is:

      1. Selecteer **[!UICONTROL Map Into]** of **[!UICONTROL Case]** vanuit **[!UICONTROL Mapping type]** .

      1. Wanneer u **[!UICONTROL Map Into]** hebt geselecteerd, selecteer **[!UICONTROL Field]** en **[!UICONTROL *AEP datasetgebied *]**of **[!UICONTROL Value]**en een standaardwaarde om het geharmoniseerde gebied door gebrek aan het datasetgebied in kaart te brengen of waarde ingegaan.

      1. Wanneer u **[!UICONTROL Case]** selecteert, selecteer **[!UICONTROL Field]** en **[!UICONTROL *AEP datasetgebied *]**of **[!UICONTROL Value]**en een standaardwaarde om het geharmoniseerde gebied door gebrek aan het datasetgebied of de ingegaan waarde in kaart te brengen.

         1. Als u waarden expliciet wilt instellen, definieert u een of meer gevallen, die uit een of meer voorwaarden bestaan. Elke voorwaarde kan voor een specifiek **[!UICONTROL *AEP datasetgebied *]**controleren of het **[!UICONTROL Exists]**of **[!UICONTROL Not Exists]**of het **[!UICONTROL Contains]**,**[!UICONTROL Not Contains]**,**[!UICONTROL Equals]**,**[!UICONTROL Not Equals]**,**[!UICONTROL Starts With]**, of **[!UICONTROL Ends With]**een waarde ingegaan bij**[!UICONTROL * gaat inputwaarde *]** in.

         1. Om een ander geval toe te voegen, voegt de uitgezochte ![ ](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add case]** toe, om een andere voorwaarde toe te voegen, ![ toe ](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add condition]**.

         1. Om een geval of een voorwaarde te schrappen, uitgezochte ![ Sluiten ](/help/assets/icons/Close.svg) in de overeenkomstige container.

         1. Selecteer **[!UICONTROL Any of]** of **[!UICONTROL All of]** om te bepalen of een of alle voorwaarden voor een hoofdlettergebruik moeten gelden.

         1. Als u de resultaatwaarde voor een hoofdlettergebruik wilt instellen, voert u de waarde in op **[!UICONTROL Then]** .

      Het onderstaande voorbeeld

      * gebruikt een **[!UICONTROL Map Into]** **[!UICONTROL Mapping type]** om het geharmoniseerde veld **[!UICONTROL Channel Type At Source]** toe te wijzen aan het veld **[!UICONTROL channel_type]** in de gegevensset **[!DNL Luma Transactions]** .

      * gebruikt een **[!UICONTROL Case]** **[!UICONTROL Mapping type]** om de waarde van het veld **[!UICONTROL marketing.campaignName]** in de **[!DNL Luma Transactions]** dataset voorwaardelijk toe te wijzen aan het geharmoniseerde veld **[!UICONTROL Campaign]** . Het geharmoniseerde veld Campagne is ingesteld op:

         * `Black Friday` wanneer **[!UICONTROL marketing.campaignName]** is `_black_friday` of `BlackFriday`.
         * in alle andere gevallen op de waarde van de **[!UICONTROL marketing.campaignName]** .

        ![ gebeurtenis van de de regelregel van de Dataset ](/help/assets/dataset-create-event.png)

1. Selecteer ![ toevoegen ](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add field]** om extra gebieden te bepalen.

Als u klaar bent, selecteert u **[!UICONTROL Save as draft]** om een conceptversie van de regel op te slaan of **[!UICONTROL Save]** om de regel op te slaan en te activeren. Selecteer **[!UICONTROL Cancel]** om de regelconfiguratie te annuleren.


### Een gegevenssetregel bewerken

Om een datasetregel uit te geven, in ![ DataSearch ](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** interface in Mix Modeler:

1. Selecteer ![ Meer ](/help/assets/icons/More.svg) in de **[!UICONTROL Dataset]** kolom voor de datasetregel die u wilt uitgeven.
1. Van het contextmenu, uitgezocht ![ geef ](/help/assets/icons/Edit.svg) **[!UICONTROL Edit]** uit beginnen de datasetregel uit te geven. Verwijs naar [ creeer een datasetregel ](#create-a-dataset-rule) voor meer details.


### Een gegevenssetregel verwijderen

Om een datasetregel te schrappen, in ![ DataSearch ](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** interface in Mix Modeler:

1. Selecteer ![ Meer ](/help/assets/icons/More.svg) in de **[!UICONTROL Dataset]** kolom voor de datasetregel die u wilt schrappen.
1. Van het contextmenu, uitgezochte ![ Schrapping ](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** om de datasetregel te schrappen. U wordt om bevestiging gevraagd. Selecteer **[!UICONTROL Delete]** om de geselecteerde gegevenssetregel permanent te verwijderen.


## Gegevens synchroniseren

Om gegevens tussen uw geharmoniseerde gegevens en samenvatting en/of gebeurtenisdatasets te synchroniseren terwijl het toepassen van de logica in uw datasetregels:

1. Selecteer **[!UICONTROL Sync data]** .

1. Selecteer in het dialoogvenster **[!UICONTROL Sync data for dataset rules]** de optie
   * **[!UICONTROL Refresh harmonized data for summary datasets]** ,
   * **[!UICONTROL Refresh harmonized data for event datasets]** , of
   * **[!UICONTROL Refresh harmonized data for both summary + event datasets]**.

1. Selecteer **[!UICONTROL Sync]** om de synchronisatie te starten op basis van de gedefinieerde gegevenssetregels tussen geharmoniseerde gegevens en gegevens in gegevenssets. Selecteer **[!UICONTROL Cancel]** om de synchronisatie te annuleren.

   ![ gegevens van de Synchronisatie ](/help/assets/sync-data.png)


## Voorkeuren voor gegevenssamenvoeging

>[!NOTE]
>
>[!BADGE  bèta ]{type=Informative}

Voorkeuren voor gegevenssamenvoeging helpen u conflicten op te lossen wanneer gegevens uit een overzicht en gebeurtenisgegevensbronnen worden samengevoegd. Gebruiksscenario&#39;s zijn:

* dezelfde advertentiemetrie in meerdere gegevensreeksen wordt gemeten en gerapporteerd, of
* metrische metingen kunnen in sommige gegevensreeksen onvolledig zijn, terwijl een andere dataset een superset van een bepaalde metrische waarde kan zijn, resulterend in dubbeltelling.

Voor nauwkeurige modelvoorspelling kunt u voorkeuren voor gegevenssamenvoeging definiëren:

1. Selecteer ![ de voorkeur van de Fusie van Gegevens ](/help/assets/icons/Merge.svg) [!BADGE  bèta ].

1. In **[!UICONTROL Data merge preferences]** [!BADGE  bèta ]{type=Informative}

   ![ de fusievoorkeur van Gegevens ](/help/assets/data-merge-preferences.png)

   * Selecteer een **[!UICONTROL Default metric preference]** . De geselecteerde standaard metrische voorkeur wordt toegepast wanneer, tijdens harmonisatie, de veelvoudige bronnen van gegevens een metrisch gebied voor een bepaald kanaal bijwerken. De voorkeur wordt toegepast op het niveau van de zandbak, tenzij met voeten getreden voor specifieke metrische gebaseerde voorkeur. U kunt kiezen tussen **[!UICONTROL Summary data]** , **[!UICONTROL Event data]** en **[!UICONTROL Sum of summary and event data]** .

   * Specifieke op metrische basis gebaseerde voorkeuren toevoegen:

      1. Selecteer ![ plus ](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add a metric]**.
         1. Selecteer metrisch van de **[!UICONTROL *Metrische selectie *]**lijst.
         1. Selecteer **[!UICONTROL CHANNELS]** of **[!UICONTROL CONVERSION TYPES]** . Selecteer in de lijst **[!UICONTROL All]** of een specifiek kanaal of conversietype.
         1. Selecteer **[!UICONTROL Summary]** of **[!UICONTROL Event]** om op te geven of summiere gegevens of gebeurtenisgegevens bij het samenvoegen van gegevens de voorkeur hebben voor de metrische gegevens (en voor alle gegevens of voor het geselecteerde kanaal).

         Een of meer extra kanaal- of conversietypen toevoegen:

         1. Selecteer ![ plus ](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add a channel]** of ![ plus ](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add a conversion type]**.
         1. Selecteer **[!UICONTROL Summary]** of **[!UICONTROL Event]** .

         Om een kanaal of omzettingstype te schrappen, uitgezochte ![ Kruis ](/help/assets/icons/Close.svg).

      1. Herhaal de vorige stap als u meer specifieke, op metrische basis gebaseerde voorkeuren wilt toevoegen.

   * Om een bestaande specifieke metrische gebaseerde voorkeur te schrappen, uitgezochte ![ Schrapping ](/help/assets/icons/Delete.svg).

1. Selecteer **[!UICONTROL Save]** om de voorkeuren voor gegevenssamenvoeging op te slaan. De gegevens worden opnieuw gesynchroniseerd. <br/> Uitgezocht **[!UICONTROL Cancel]** om te annuleren.

## Een brongegevensset verwijderen

Wanneer u een brondataset schrapt die in uw geharmoniseerde gegevens wordt gebruikt, worden de onderliggende ingangen op die brondataset verwijderd uit [[!UICONTROL Harmonized data]](/help/harmonize-data/overview.md). Nochtans, blijft de datasetregel met de geschrapte brondataset in de datasetregel config lijst met een pictogram ![ DataRemove ](/help/assets/icons/DataRemove.svg) erop wijzend dat de brondataset is geschrapt. Voor meer details:

* Selecteer ![ Meer ](/help/assets/icons/More.svg) en ![ Voorproef ](/help/assets/icons/Preview.svg) **[!UICONTROL View]** van het contextmenu.
In het dialoogvenster **[!UICONTROL Dataset rule mapping - Fields]** wordt informatie weergegeven over de verwijderde brongegevensset en de velden die worden gebruikt in de configuratie van de gegevenssetregel.

Wanneer u terugkeert naar uw **[!UICONTROL Dataset rules]** configuratie, ziet u een dialoog verklarend dat één of meerdere brondatasets zijn geschrapt. De geharmoniseerde gegevens worden beïnvloed bij een volgende ad-hoc of geplande synchronisatie. Controleer de configuratie van de gegevenssetregel.

De geharmoniseerde gegevens worden zonder de verwijderde brongegevens bijgewerkt bij de volgende ad-hocsynchronisatie of geplande synchronisatie. Nochtans, blijft u waarschuwingsdialogen zien die u ertoe aanzetten om de datasetregel te schrappen die op de geschrapte brondataset wordt gebaseerd. Met deze waarschuwing kunnen gebruikers de desbetreffende velden in de verwijderde gegevensset bekijken en evalueren. En om het effect te bepalen op het op de markt brengen van aanraakpunten of omzettingen die in om het even welke modellen kunnen worden gebruikt. Zodra u voor dit effect hebt herzien en verlicht, zou u de datasetregel van de de regel config lijst van de datasetregel moeten schrappen.
