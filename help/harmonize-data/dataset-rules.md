---
title: Gegevensregels
description: Leer hoe u gegevenssetregels definieert die u kunt gebruiken als onderdeel van het harmoniseren van uw gegevens in Mix Modeler.
feature: Harmonized Data, Dataset Rules
exl-id: 57d7940a-2900-4814-a30d-bb02bff7615d
source-git-commit: 9987c845414fa5a3abda201d55f7b1ed6e211780
workflow-type: tm+mt
source-wordcount: '2102'
ht-degree: 0%

---

# Gegevensregels

Met de gegevenssetregels kunt u geharmoniseerde velden toewijzen aan velden uit de gegevens die u hebt ingevoerd in Mix Modeler.

* Voor geaggregeerde gegevens die u in Adobe Experience Platform hebt ingevoerd, wijst u een of meer van de beschikbare gegevenssetvelden toe aan de juiste geharmoniseerde velden.
* Voor gebeurtenisgegevens kunt u een of meer geharmoniseerde velden afzonderlijk toewijzen aan velden uit de gegevensset, rechtstreeks of met behulp van voorwaarden.


## Gegevenssetregels beheren

Een lijst van de beschikbare datasetregels, in de interface van Mix Modeler zien:

1. Selecteer ![&#x200B; DataSearch &#x200B;](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** van het linkerspoor.

1. Selecteer **[!UICONTROL Dataset rules]** in de bovenste balk. U ziet een lijst van de datasetregels.

U kunt naar een dataset snel zoeken gebruikend ![&#x200B; Onderzoek &#x200B;](/help/assets/icons/Search.svg) **[!UICONTROL _ga een datasetnaam_]** in.

De tabelkolommen geven details over de gegevenssetregels op:

| Kolomnaam | Details |
| ---------------------- | ----------|
| **[!UICONTROL Dataset]** | De naam van de gegevensset.  Gebruik ![&#x200B; meer &#x200B;](/help/assets/icons/More.svg) om acties voor een dataset te selecteren. U kunt:<ul><li>![&#x200B; Voorproef &#x200B;](/help/assets/icons/Preview.svg) **[!UICONTROL View]** om de configuratie van de datasetregels te bekijken. Alle velden zijn uitgeschakeld.</li><li>![&#x200B; geef &#x200B;](/help/assets/icons/Edit.svg) **[!UICONTROL Edit]** uit om de configuratie van de datasetregels uit te geven.</li><li>![&#x200B; Schrapping &#x200B;](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** om de configuratie van de datasetregels te schrappen. U wordt gevraagd de verwijdering te bevestigen in het dialoogvenster Gegevensset verwijderen. Selecteer **[!UICONTROL Delete]** om de configuratie van de gegevenssetregel permanent te verwijderen.</li><ul> |
| **[!UICONTROL Source]** | De bron van de gegevensset: Adobe Analytics, Experience Events, Summary (aggregaat) of Consumer Experience Events. |
| **[!UICONTROL Schema]** | Het schema waaraan de dataset voldoet. U kunt de schemanaam snel selecteren om het schema in een nieuw lusje in de schemaredacteur in ![&#x200B; Schema &#x200B;](/help/assets/icons/Schemas.svg) Schema&#39;s [&#x200B; te openen.](../ingest-data/schemas.md) |
| **[!UICONTROL Granularity]** | De granulariteit van gegevens in de dataset. Mogelijke waarden zijn Dagelijks, Wekelijks, Maandelijks of Jaarlijks. |
| **[!UICONTROL Start of the week]** | Geeft aan welke dag van de week wordt beschouwd als het begin van een nieuwe week voor de specifieke gegevensset. |
| **[!UICONTROL Status]** | De status van het gebied: ![&#x200B; StatusGray &#x200B;](/help/assets/icons/StatusGray.svg) Ontwerp of ![&#x200B; StatusGreen &#x200B;](/help/assets/icons/StatusGreen.svg) Actief |
| **[!UICONTROL Last modified]** | Gegevens en tijd van de laatste wijziging van de gegevenssetregel. |

{style="table-layout:auto"}

### Een gegevenssetregel maken

Om een datasetregel tot stand te brengen, in ![&#x200B; DataSearch &#x200B;](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** interface in Mix Modeler, selecteer **[!UICONTROL Create a dataset rule]** in de **[!UICONTROL Dataset rules configuration]** tovenaar.

In het **[!UICONTROL Create]** -scherm

1. Selecteer in **[!UICONTROL Dataset details]** een gegevensset in **[!UICONTROL Select dataset]** om de configuratie te starten. In de lijst worden datasets gecategoriseerd in **[!UICONTROL Summary]**, **[!UICONTROL Adobe Analytics]**, **[!UICONTROL Experience Event]**, **[!UICONTROL Factors]** en **[!UICONTROL Consumer Experience Events]** .

1. Selecteer een dag voor **[!UICONTROL Start of the week]**.

1. Selecteer **[!UICONTROL Daily]** , **[!UICONTROL Weekly]** , **[!UICONTROL Monthly]** of **[!UICONTROL Yearly]** for **[!UICONTROL Granularity]** .

1. Wanneer u een gegevensset van de categorie **[!UICONTROL Summary]** of **[!UICONTROL Factors]** hebt geselecteerd, selecteert u **[!UICONTROL Aggregation]** of **[!UICONTROL Replacement]** for **[!UICONTROL Data restatement is by]** .

   Het rapporteren van gegevens van uitgevers is zeer belangrijk voor marketinganalisten, aangezien het werken met uitgevers vaak aanzienlijke uitgaven met zich meebrengt, en wijzigingen in de rapportagegegevens kunnen leiden tot zeer verschillende inzichten en investeringsplannen. Daarnaast hebben marketinganalisten nauwkeurige gegevens nodig om de juiste inzichten te verkrijgen en overtuigende voorstellen te doen om het vertrouwen van de belanghebbenden te winnen. Deze uitgevers, zoals Google en Facebook, hernoemen of verwijderen echter vaak de rapportgegevens omdat ze hun gegevens met elkaar in overeenstemming brengen. Het tijdsbestek voor de meeste wijzigingen ligt binnen 7 dagen na de mediaprestaties. Extra wijzigingen in de gegevens zijn mogelijk binnen 30 dagen. Over het algemeen worden boeken na 30 dagen als gesloten beschouwd en zijn de gegevens volledig.

   Mix Modeler ondersteunt gegevensherschikking. Om ervoor te zorgen dat de gegevens die voor rapportering, modellering, en planning worden gebruikt nauwkeurig zijn. En dat de gegevens in staat zijn om de verwachtingen en behoeften van de merk- en marketinganalist te ondersteunen.

   U kunt opnieuw vermelde rijen van summiere gegevens als stijgende rijen in een dataset van Experience Platform verzenden en de harmonisatiedienst werkt de geharmoniseerde dataset met die aangepaste gegevens bij. Op dezelfde manier kunt u rijen samenvattingsgegevens ook verwijderen die in de harmonisatiedienst moeten worden weerspiegeld.

1. Selecteer in de sectie **[!UICONTROL Map to harmonized fields]** een geharmoniseerd veld in **[!UICONTROL Standard harmonized field]** . Om [&#x200B; een nieuw geharmoniseerd gebied &#x200B;](/help/harmonize-data/fields.md#add-a-harmonized-field) snel tot stand te brengen, selecteer **[!UICONTROL Create new]**.

   * Wanneer het geselecteerde geharmoniseerde veld metrisch is:

      1. Selecteer **[!UICONTROL Count]** of **[!UICONTROL Sum]** vanuit **[!UICONTROL Mapping type]** .

      1. Selecteer een **[!UICONTROL *datasetgebied van AEP *]**&#x200B;dat u het geharmoniseerde gebied aan door gebrek wilt in kaart brengen.

   * Wanneer het geselecteerde veld van het type afmeting is:

      1. Selecteer **[!UICONTROL Map Into]** of **[!UICONTROL Case]** vanuit **[!UICONTROL Mapping type]** .

      1. Wanneer u **[!UICONTROL Map Into]** hebt geselecteerd, selecteer **[!UICONTROL Field]** en **[!UICONTROL *de datasetgebied van AEP *]**&#x200B;of **[!UICONTROL Value]**&#x200B;en een standaardwaarde om het geharmoniseerde gebied door gebrek aan het datasetgebied in kaart te brengen of waarde ingegaan.

      1. Wanneer u **[!UICONTROL Case]** selecteert, selecteer **[!UICONTROL Field]** en **[!UICONTROL *gebied van de dataset van AEP *]**&#x200B;of **[!UICONTROL Value]**&#x200B;en een standaardwaarde om het geharmoniseerde gebied door gebrek aan het datasetgebied of de ingegaan waarde in kaart te brengen.

         1. Als u waarden expliciet wilt instellen, definieert u een of meer gevallen, die uit een of meer voorwaarden bestaan. Elke voorwaarde kan voor een specifiek **[!UICONTROL *gebied van de dataset van AEP *]**&#x200B;controleren of het **[!UICONTROL Exists]**&#x200B;of **[!UICONTROL Not Exists]**&#x200B;of het **[!UICONTROL Contains]**,**[!UICONTROL Not Contains]**,**[!UICONTROL Equals]**,**[!UICONTROL Not Equals]**,**[!UICONTROL Starts With]**, of **[!UICONTROL Ends With]**&#x200B;een waarde ingegaan bij&#x200B;**[!UICONTROL * gaat inputwaarde *]** in.

         1. Om een ander geval toe te voegen, voegt de uitgezochte ![&#x200B; &#x200B;](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add case]** toe, om een andere voorwaarde toe te voegen, ![&#x200B; toe &#x200B;](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add condition]**.

         1. Om een geval of een voorwaarde te schrappen, uitgezochte ![&#x200B; Sluiten &#x200B;](/help/assets/icons/Close.svg) in de overeenkomstige container.

         1. Selecteer **[!UICONTROL Any of]** of **[!UICONTROL All of]** om te bepalen of een of alle voorwaarden voor een hoofdlettergebruik moeten gelden.

         1. Als u de resultaatwaarde voor een hoofdlettergebruik wilt instellen, voert u de waarde in op **[!UICONTROL Then]** .

     In het onderstaande voorbeeld:

      * gebruikt een **[!UICONTROL Map Into]** **[!UICONTROL Mapping type]** om het geharmoniseerde veld **[!UICONTROL Channel Type At Source]** toe te wijzen aan het veld **[!UICONTROL channel_type]** in de gegevensset **[!DNL Luma Transactions]** .

      * gebruikt een **[!UICONTROL Case]** **[!UICONTROL Mapping type]** om de waarde van het veld **[!UICONTROL marketing.campaignName]** in de **[!DNL Luma Transactions]** dataset voorwaardelijk toe te wijzen aan het geharmoniseerde veld **[!UICONTROL Campaign]** . Het geharmoniseerde veld Campagne is ingesteld op:

         * `Black Friday` wanneer **[!UICONTROL marketing.campaignName]** is `_black_friday` of `BlackFriday`.
         * in alle andere gevallen op de waarde van de **[!UICONTROL marketing.campaignName]** .

        ![&#x200B; gebeurtenis van de de regelregel van de Dataset &#x200B;](/help/assets/dataset-create-event.png)

1. Selecteer ![&#x200B; toevoegen &#x200B;](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add field]** om extra gebieden te bepalen.

Als u klaar bent, selecteert u **[!UICONTROL Save as draft]** om een conceptversie van de regel op te slaan of **[!UICONTROL Save]** om de regel op te slaan en te activeren. Selecteer **[!UICONTROL Cancel]** om de regelconfiguratie te annuleren.

>[!NOTE]
>
>De toegewezen **[!UICONTROL Map to harmonized fields]** ervaring voor samenvattingsregels voor gegevenssets is afgekeurd. Alle regels voor gegevenssets gebruiken nu een vergelijkbare **[!UICONTROL Map to harmonized fields]** ervaring, ongeacht het type gegevensset. Voor summiere datasets waarvoor u regels gebruikend verouderde **[!UICONTROL Map to harmonized fields]** ervaring hebt bepaald, zou u deze regels tegen de generische **[!UICONTROL Map to harmonized field]** ervaring kunnen willen verifiëren.
>

#### Samenvattingsgegevenssets

Wanneer u een standaard geharmoniseerd gebied van een summiere dataset in kaart brengt, probeert Mix Modeler om het overeenkomstige de datasetgebied van Experience Platform af te trekken. Wanneer gelukt:

* Als het veld een dimensie heeft, wordt **[!UICONTROL Map into]** geselecteerd als **[!UICONTROL Mapping type]** .
* Als het veld metrisch is, wordt **[!UICONTROL Sum]** geselecteerd als **[!UICONTROL Mapping type]** .
* **[!UICONTROL Field]** wordt geselecteerd als het **[!UICONTROL Default]** toewijzingstype.
* Het overeenkomstige de datasetgebied van Experience Platform wordt automatisch opgenomen voor *het Gebied van de Dataset van AEP*.

U kunt de voorgestelde waarden wijzigen als deze onjuist zijn of als dit uw specifieke gebruiksscenario niet ondersteunt.


#### Gegevensbestanden van de factor

U brengt geharmoniseerde gebieden aan gebieden in een factordataset in kaart, zodat kunt u [&#x200B; factoren als deel van uw modelconfiguratie &#x200B;](/help/models/build.md) toevoegen.

Wanneer u geharmoniseerde gebieden aan gebieden in een factordatasets in kaart brengt, is het volgende van toepassing:

##### Naam van factor

Wanneer u een standaard geharmoniseerd factorgebied van een factordataset in kaart brengt en de factordataset één enkele factor bevat, gebruik **[!UICONTROL Map into]** als **[!UICONTROL Mapping type]** en ga een standaardwaarde voor het **[!UICONTROL Factor Name]** geharmoniseerde gebied in.

![&#x200B; regel van de Dataset - kaart enige factordataset &#x200B;](../assets/dataset-create-rule-factor-single.png)

Als de factordataset veelvoudige factoren bevat, gebruik **[!UICONTROL Case As]** als **[!UICONTROL Mapping Type]** om een afbeelding tussen het geharmoniseerde gebied van de Naam van de Factor en elke afzonderlijke factornaam te bepalen.

![&#x200B; regel van de Dataset - kaart enige factordataset &#x200B;](../assets/dataset-create-rule-factor-multiple.png)


##### Type factor

Dit gebied is facultatief in de factordataset en het schema. Als **[!UICONTROL Factor type]** in de factordataset en het factorschema wordt bepaald en of **[!UICONTROL Internal]** of **[!UICONTROL External]** specificeert, wordt de verstrekte waarde gebruikt. Wanneer geen waarde is opgegeven, wordt de standaardwaarde **[!UICONTROL Internal]** gebruikt.

##### Type waarde

Dit gebied is facultatief in de factordataset en het schema. Als **[!UICONTROL Value type]** in de factordataset en het factorschema wordt bepaald en of **[!UICONTROL Actual]** of **[!UICONTROL Forecasted]** specificeert, wordt de verstrekte waarde gebruikt. Wanneer geen waarde is opgegeven, wordt de standaardwaarde **[!UICONTROL Actual]** gebruikt.


##### Korreligheid

U kunt een datasetregel voor de granulariteit van een factordataset bepalen wanneer alle factoren binnen de factordataset de zelfde brongranulariteit hebben.

Zodra de gegevensreeksen met factoren zijn geharmoniseerd, voldoen alle gegevensreeksen aan het hoogste niveau van granulariteit in de geharmoniseerde gegevensset.


##### Waarde van factor

Gebruik voor het geharmoniseerde veld van **[!UICONTROL Factor value]** een van de aggregatie-operatoren als de **[!UICONTROL Mapping Type]** . Wanneer meerdere factoren zijn gedefinieerd in een factorgegevensset, wordt de geaggregeerde operator toegepast op alle factoren.


##### Voorbeeld

* U hebt een factordataset, met de volgende steekproefgegevens:

  | Tijdstempel | Naam factor | Waarde factor |
  |---|---|---:|
  | 13 mrt. 2025 | _definedsp500 | 10 |
  | 13 mrt. 2025 | _cpi | 20 |
  | 14 mrt. 2025 | _definedsp500 | 30 |
  | 14 mrt. 2025 | _cpi | 40 |
  | 15 mrt. 2025 | _definedsp500 | 50 |
  | 15 mrt. 2025 | _cpi | 60 |


* En u definieert de volgende gegevenssetregels voor **[!UICONTROL Factor Name]** , **[!UICONTROL Factor Value]** en **[!UICONTROL Granularity]** :

  ![&#x200B; de regels van de Dataset - factor voorbeeld &#x200B;](../assets/dataset-create-rule-factor-example.png)

* Dit resulteert vervolgens in de volgende geharmoniseerde gegevens:

  | Naam factor | Waarde factor | Type factor | Type waarde |
  |---|---:|---|---|
  | CPI | 20 | Intern | Werkelijk |
  | S&amp;P 500 | 10 | Intern | Werkelijk |

  Aangezien er geen gegevenssetregels zijn gedefinieerd voor **[!UICONTROL Factor Type]** en **[!UICONTROL Value Type]** , worden de standaardwaarden gebruikt.

### Een gegevenssetregel bewerken

Om een datasetregel uit te geven, in ![&#x200B; DataSearch &#x200B;](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** interface in Mix Modeler:

1. Selecteer ![&#x200B; Meer &#x200B;](/help/assets/icons/More.svg) in de **[!UICONTROL Dataset]** kolom voor de datasetregel die u wilt uitgeven.
1. Van het contextmenu, uitgezocht ![&#x200B; geef &#x200B;](/help/assets/icons/Edit.svg) **[!UICONTROL Edit]** uit beginnen de datasetregel uit te geven. Verwijs naar [&#x200B; creeer een datasetregel &#x200B;](#create-a-dataset-rule) voor meer details.


### Een gegevenssetregel verwijderen

Om een datasetregel te schrappen, in ![&#x200B; DataSearch &#x200B;](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** interface in Mix Modeler:

1. Selecteer ![&#x200B; Meer &#x200B;](/help/assets/icons/More.svg) in de **[!UICONTROL Dataset]** kolom voor de datasetregel die u wilt schrappen.
1. Van het contextmenu, uitgezochte ![&#x200B; Schrapping &#x200B;](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** om de datasetregel te schrappen. U wordt om bevestiging gevraagd. Selecteer **[!UICONTROL Delete]** om de geselecteerde gegevenssetregel permanent te verwijderen.



## Gegevens synchroniseren

Om gegevens tussen uw geharmoniseerde gegevens en samenvatting en/of gebeurtenisdatasets te synchroniseren terwijl het toepassen van de logica in uw datasetregels:

1. Selecteer **[!UICONTROL Sync data]**.

1. Selecteer in het dialoogvenster **[!UICONTROL Sync data for dataset rules]** de optie
   * **[!UICONTROL Refresh harmonized data for summary datasets]** ,
   * **[!UICONTROL Refresh harmonized data for event datasets]** , of
   * **[!UICONTROL Refresh harmonized data for both summary + event datasets]**.

1. Selecteer **[!UICONTROL Sync]** om de synchronisatie te starten op basis van de gedefinieerde gegevenssetregels tussen geharmoniseerde gegevens en gegevens in gegevenssets. Selecteer **[!UICONTROL Cancel]** om de synchronisatie te annuleren.

   ![&#x200B; gegevens van de Synchronisatie &#x200B;](/help/assets/sync-data.png)


## Voorkeuren voor gegevenssamenvoeging {#data-merge-preferences}


>[!CONTEXTUALHELP]
>id="harmonizeddata_datasetrules_datamergepreferences"
>title="Standaardmetrische voorkeur"
>abstract="De standaardvoorkeur wordt toegepast wanneer tijdens harmonisatie, veelvoudige bronnen van gegevens proberen om een metrisch gebied voor een bepaald kanaal bij te werken. Deze voorkeur wordt toegepast op het niveau van de zandbak tenzij met voeten getreden voor bepaalde metrische voorkeur indien hieronder bepaald."


>[!NOTE]
>
>[!BADGE &#x200B; bèta &#x200B;]{type=Informative} De voorkeur van de fusie van Gegevens is een bètaeigenschap en zijn functionaliteit is onderworpen aan verandering.

Voor nauwkeurige modelvoorspellingen kunt u voorkeuren voor gegevenssamenvoeging definiëren. Met deze functionaliteit kunnen gebruikers eventuele conflicten oplossen na het samenvoegen van gegevens op overzichtsniveau en op gebeurtenisniveau.

U kunt een standaard metrische voorkeur vormen die in het geval van conflicterende updates moet worden toegepast. Deze standaard metrische waarde kan één van drie opties zijn:

* **[!UICONTROL Summary data]**
* **[!UICONTROL Sum of summary and event data]**
* **[!UICONTROL Event data]**

Wanneer, tijdens harmonisatie, de veelvoudige bronnen van gegevens proberen om een metrisch gebied voor een bepaald kanaal bij te werken, wordt de standaardvoorkeur die door de gebruiker wordt gevormd toegepast. Deze voorkeur wordt toegepast op het zandbakniveau tenzij met voeten getreden voor bepaalde metrische gebaseerde voorkeur die extra wordt gevormd.

Onder **[!UICONTROL Metric based preferences]**, kan de gebruiker de specifieke bron (**[!UICONTROL Summary]** of **[!UICONTROL Event]**) voor bepaalde metrisch en het overeenkomstige omzettingstype voor die metrisch vormen.

De meest voorkomende gebruiksgevallen zijn:

* dezelfde advertentiemetrie in meerdere gegevensreeksen wordt gemeten en gerapporteerd, of
* metrische metingen kunnen in sommige gegevensreeksen onvolledig zijn, terwijl een andere dataset een superset van een bepaalde metrische waarde kan zijn, resulterend in dubbeltelling.

### Configureren

Voorkeuren voor gegevenssamenvoeging configureren:


1. Selecteer ![&#x200B; de voorkeur van de Fusie van Gegevens &#x200B;](/help/assets/icons/Merge.svg) [!BADGE &#x200B; bèta &#x200B;].

1. In de **[!UICONTROL Data merge preferences]** [!BADGE &#x200B; bèta &#x200B;]{type=Informative} dialoog:

   ![&#x200B; de fusievoorkeur van Gegevens &#x200B;](/help/assets/data-merge-preferences.png)

   * Selecteer een **[!UICONTROL Default metric preference]** . De geselecteerde standaard metrische voorkeur wordt toegepast wanneer, tijdens harmonisatie, de veelvoudige bronnen van gegevens een metrisch gebied voor een bepaald kanaal bijwerken. De voorkeur wordt toegepast op het niveau van de zandbak, tenzij met voeten getreden voor specifieke metrische gebaseerde voorkeur. U kunt kiezen tussen **[!UICONTROL Summary data]** , **[!UICONTROL Event data]** en **[!UICONTROL Sum of summary and event data]** .

   * Specifieke op metrische basis gebaseerde voorkeuren toevoegen:

      1. Selecteer ![&#x200B; plus &#x200B;](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add a metric]**.
         1. Selecteer metrisch van de **[!UICONTROL *Metrische selectie *]**&#x200B;lijst.
         1. Selecteer **[!UICONTROL CHANNELS]** of **[!UICONTROL CONVERSION TYPES]** . Selecteer in de lijst **[!UICONTROL All]** of een specifiek kanaal of conversietype.
         1. Selecteer **[!UICONTROL Summary]** of **[!UICONTROL Event]** om op te geven of summiere gegevens of gebeurtenisgegevens bij het samenvoegen van gegevens de voorkeur hebben voor de metrische gegevens (en voor alle gegevens of voor het geselecteerde kanaal).

         Een of meer extra kanaal- of conversietypen toevoegen:

         1. Selecteer ![&#x200B; plus &#x200B;](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add a channel]** of ![&#x200B; plus &#x200B;](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add a conversion type]**.
         1. Selecteer **[!UICONTROL Summary]** of **[!UICONTROL Event]** .

         Om een kanaal of omzettingstype te schrappen, uitgezochte ![&#x200B; Kruis &#x200B;](/help/assets/icons/Close.svg).

      1. Herhaal de vorige stap als u meer specifieke, op metrische basis gebaseerde voorkeuren wilt toevoegen.

   * Om een bestaande specifieke metrische gebaseerde voorkeur te schrappen, uitgezochte ![&#x200B; Schrapping &#x200B;](/help/assets/icons/Delete.svg).

1. Selecteer **[!UICONTROL Save]** om de voorkeuren voor gegevenssamenvoeging op te slaan. De gegevens worden opnieuw gesynchroniseerd. <br/> Uitgezocht **[!UICONTROL Cancel]** om te annuleren.

## Een brongegevensset verwijderen

Wanneer u een brondataset schrapt die in uw geharmoniseerde gegevens wordt gebruikt, worden de onderliggende ingangen op die brondataset verwijderd uit [[!UICONTROL Harmonized data]](/help/harmonize-data/overview.md). Nochtans, blijft de datasetregel met de geschrapte brondataset in de datasetregel config lijst met een pictogram ![&#x200B; DataRemove &#x200B;](/help/assets/icons/DataRemove.svg) erop wijzend dat de brondataset is geschrapt. Voor meer details:

* Selecteer ![&#x200B; Meer &#x200B;](/help/assets/icons/More.svg) en ![&#x200B; Voorproef &#x200B;](/help/assets/icons/Preview.svg) **[!UICONTROL View]** van het contextmenu.
In het dialoogvenster **[!UICONTROL Dataset rule mapping - Fields]** wordt informatie weergegeven over de verwijderde brongegevensset en de velden die worden gebruikt in de configuratie van de gegevenssetregel.

Wanneer u terugkeert naar uw **[!UICONTROL Dataset rules]** configuratie, ziet u een dialoog verklarend dat één of meerdere brondatasets zijn geschrapt. De geharmoniseerde gegevens worden beïnvloed bij een volgende ad-hoc of geplande synchronisatie. Controleer de configuratie van de gegevenssetregel.

De geharmoniseerde gegevens worden zonder de verwijderde brongegevens bijgewerkt bij de volgende ad-hocsynchronisatie of geplande synchronisatie. Nochtans, blijft u waarschuwingsdialogen zien die u ertoe aanzetten om de datasetregel te schrappen die op de geschrapte brondataset wordt gebaseerd. Met deze waarschuwing kunnen gebruikers de desbetreffende velden in de verwijderde gegevensset bekijken en evalueren. En om het effect te bepalen op het op de markt brengen van aanraakpunten of omzettingen die in om het even welke modellen kunnen worden gebruikt. Zodra u voor dit effect hebt herzien en verlicht, zou u de datasetregel van de de regel config lijst van de datasetregel moeten schrappen.
