---
title: Modelinzichten
description: Leer hoe u details over uw model kunt opvragen, zoals historisch overzicht, modelinzichten en modelkwaliteit in Mix Modeler.
feature: Models
exl-id: d99852f9-ba0d-4a2e-b5f3-ca0efe6002fd
source-git-commit: 0ee212a626986e4c721d0e58f2528d0ca1a9fdbf
workflow-type: tm+mt
source-wordcount: '1549'
ht-degree: 0%

---

# Modelinzichten

Om modelinzichten, in de ![ Modellen ](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** interface in Mix Modeler te bekijken:

1. Van de **[!UICONTROL Models]** lijst, selecteer de naam van een model dat a **[!UICONTROL Last run status]** van <span style="color:green"> heeft </span> **[!UICONTROL Success]**.

1. Selecteer **[!UICONTROL Model Insights]** in het contextmenu.

![ Model inzichten lusjebar ](/help/assets/model-insights-tabbar.png)

U ziet wanneer het gespecificeerde model laatste verfrist is en de visualisaties gebruikend vier lusjes worden getoond: [ Modelinzichten ](#model-insights), [ Attributie ](#attribution), [ Factoren ](#factors), [ Diagnose ](#diagnostics), en [ Historisch overzicht ](#historical-overview).

U kunt de datumperiode wijzigen waarop de visualisaties op elk tabblad zijn gebaseerd. Ga een datumperiode in of selecteer ![ Kalender ](/help/assets/icons/Calendar.svg) om een datumperiode te selecteren.

## [!UICONTROL Model insights]

Het modellusje van Inzichten toont visualisaties voor [ Bijdrage door datum en basismedia ](#contribution-by-date-and-base-media), [ Bijdrage door kanaal ](#contribution-by-channel), [ de prestatiessamenvatting van de Marketing ](#marketing-performance-summary), en [ Marginale reactiecurven ](#marginal-response-curves). Het lusje verstrekt ook a [ de onderbreking van het aanraakpunt ](#touchppint-breakdown) lijst.

![ Model - Modelinzichten ](/help/assets/model-insights-insights.png)

* U kunt de muis boven afzonderlijke diagramelementen in elke visualisatie houden om een popover met meer details weer te geven.

* Om een Csv- dossier te downloaden dat de gegevens voor visualisatie bevat, uitgezochte ![ Download ](/help/assets/icons/Download.svg).

* Om de volledige gegevens van modelinzichten in Microsoft® Excel formaat te downloaden, selecteer ![ Download ](/help/assets/icons/Download.svg) **[!UICONTROL Download data]**.


### Bijdrage op datum en basismedia.

De gestapelde grafiek is geordend: Basis bij de bodem, niet-bestede kanalen in het midden, en de kanalen van de Besteed op de bovenkant.

### Bijdrage per kanaal

De donutvisualisatie laat een verdeling van de bijdrage per kanaal zien.

### Overzicht van de marketingprestaties.

Een horizontale staafgrafiek die de prestaties van het rendement van investeringen per kanaal toont.

### Marginale responscurven.

Het lijndiagram visualiseert en vergelijkt de marginale opbrengsten die door de investering in uw marketing kanalen worden geproduceerd.  En identificeert het break-even punt waar uw stijgende terugkeer minder dan uw stijgende uitgave is. Hierdoor helpt deze visualisatie u te begrijpen wanneer uw marketinginvestering minder effect begint te sorteren.

De curve, het break-even punt en de bijbehorende waarden worden berekend op basis van het geselecteerde gegevensbereik en het kanaal dat u hebt geselecteerd.

Het kanaal wijzigen:

* Selecteer een kanaal in het vervolgkeuzemenu **[!UICONTROL Channel]** om de visualisatie voor een specifiek kanaal bij te werken.


### Uitsplitsing naar aanraakpunt

In de tabel met uitsplitsingen naar aanraakpunt worden wekelijks de uitsplitsingen naar aanraakpunt voor alle of geselecteerde kanalen weergegeven.

![ Uitsplitsing van het Aanraakpunt ](../assets/touchpoint-breakdown.png)

De volgende kolommen zijn beschikbaar:

| Kolom | Beschrijving |
|---|---|
| **[!UICONTROL Date range]** | De week waarin verslag moet worden uitgebracht. |
| **[!UICONTROL Touchpoint]** | Het specifieke aanraakpuntkanaal. |
| **[!UICONTROL ROI]** | Het percentage van (**[!UICONTROL Revenue]** - **[!UICONTROL Spend]**) / **[!UICONTROL Spend]**. |
| **[!UICONTROL Revenue]** | De inkomsten voor de datumreeks. |
| **[!UICONTROL CPA]** | **[!UICONTROL Spend]** / **[!UICONTROL Conversions]** . |
| **[!UICONTROL Conversions]** | De conversies voor het datumbereik. |
| **[!UICONTROL Spend]** | De uitgaven voor het gegevensbereik. |

Als u een specifiek kanaal of alle kanalen wilt selecteren, selecteert u een kanaal in het vervolgkeuzemenu **[!UICONTROL View]** .

Om de inhoud van de lijst van de de onderbreking van het Aanraakpunt te downloaden, selecteer ![ Download ](/help/assets/icons/Download.svg) **[!UICONTROL Download CSV]**.

## **[!UICONTROL Factors]** [!BADGE  bèta ]

Het lusje van de Factoren [!BADGE  bèta ] toont externe factor verwante inzichten.

![ Factoren ](/help/assets/factors.png)

Deze visualisatie helpt u om het stijgende effect te begrijpen dat diverse interne en externe factoren op de basislijn van omzettingen hebben. Bijvoorbeeld economische voorwaarden of promotieactiviteiten.

Selecteer in het vervolgkeuzemenu **[!UICONTROL Factors]** welke factoren u wilt weergeven.

<!-- need to update the image when we do have a proper example -->

Om een Csv- dossier te downloaden dat de gegevens voor de lijst bevat, uitgezochte ![ Download ](/help/assets/icons/Download.svg).

Als geen gegevens beschikbaar zijn ziet u een bericht ![ TableAndChart ](/help/assets/icons/TableAndChart.svg) **[!UICONTROL No data is available, you may need to retrain your model, or change the date range to view insights]**.

## [!UICONTROL Attribution]

>[!NOTE]
>
Het tabblad Attributie is alleen beschikbaar voor MTA-modellen.


Met het tabblad [!UICONTROL Attribution] kunt u de effectiviteit begrijpen van aanraakpunten en marketingcampagnes die gegevens op gebeurtenisniveau bevatten.  Zie [ model ](build.md) bouwen.

De volgende attribuutmodellen worden ondersteund:

* Gebaseerd op het geselecteerde model in Mix Modeler:
   * Algorithmic - Invloed
   * Algorithmic - Incrementeel
* Gebaseerde regel:
   * Vervaleenheden
   * Eerste aanraking
   * Laatste aanraking
   * Lineair
   * Ushape

Zie [ Multi-aanraking attributie ](../get-started/about.md#multi-touch-attribution) voor een inleiding op het multi-aanraak attributievermogen in Mix Modeler.

Selecteer een of meer toewijzingsmodellen in het vervolgkeuzemenu **[!UICONTROL Attribution Model]** . De geselecteerde attributiemodellen zijn van toepassing op alle visualisaties op het tabblad Kenmerken.

![ Attributie ](/help/assets/model-insights-attribution.png)

De granulaire gebeurtenisscores voor Mix Modeler-multitouch-kenmerk worden uitgelijnd op de algemene Mix Modeler-scores en -rendement. Deze scores worden ook beschikbaar gesteld als datasets in Experience Platform.

Het tabblad Kenmerken bestaat uit de volgende visualisaties:

### [!UICONTROL Overview]

De [!UICONTROL Overview] visualisatie toont, voor de geselecteerde attributiemodellen, de omzettingstotalen en de percentages. Als u meer modellen selecteert, worden extra cirkels aan de visualisatie toegevoegd, elk met een eigen kleur die overeenkomt met de legenda.

Als u een pop-up met details voor een attributiemodel wilt zien, houdt u de muisaanwijzer boven een van de cirkels in de visualisatie.

### [!UICONTROL Trends]

De visualisatie [!UICONTROL Daily trends] , [!UICONTROL Weekly trends] of [!UICONTROL Monthly trends] geeft voor de geselecteerde attributiemodellen de dagelijkse, wekelijkse of maandelijkse conversietrends weer.

Om de periode te kiezen, selecteer **[!UICONTROL Daily trends]**, **[!UICONTROL Weekly trends]** of **[!UICONTROL Monthly trends]** van ![ Meer ](/help/assets/icons/More.svg).

Als u details wilt zien, houdt u de muisaanwijzer boven de gegevensregel van een specifiek toewijzingsmodel om een pop-up weer te geven met het totale aantal conversies voor die gegevens.

### [!UICONTROL Breakdown]

De [!UICONTROL Breakdown] visualisatie is een uitsplitsing per kanaal of aanraakpunt van de conversies voor elk van de geselecteerde attributiemodellen. Deze visualisatie kan nuttig zijn om besluiten over de doeltreffendheid van elk kanaal of touchpoint te nemen.

Om het type uitsplitsing te kiezen, select **[!UICONTROL Breakdown by channel]** of **[!UICONTROL Breakdown by touchpoint]** van ![ Meer ](/help/assets/icons/More.svg).

Houd de muisaanwijzer boven de diagramelementen om de details weer te geven.

### [!UICONTROL Top campaigns]

De bovenste campagnes visualiseren toont een lijst van de bovenste campagnes met kolommen voor de naam van de Campagne, het Kanaal, het type van Media and Incrementele omzettingen. Deze visualisatie kan uw team helpen de doeltreffendheid van een specifieke campagne voor een bepaald kanaal te informeren en inzichten te verstrekken in welke campagnes u verder in zou moeten investeren.

De tabel in oplopende ↑ of aflopende volgorde ↓ sorteren voor Channel, mediatype or Incrementele omzettingen, selecteer de kolomkop en schakel de sortering in of uit.

Om de lijst in een afzonderlijke dialoog uit te breiden, selecteer **[!UICONTROL Expand]** van ![ Meer ](/help/assets/icons/More.svg).

Het uitgevouwen dialoogvenster Boven bevat dezelfde tabel met optelde kolommen voor

* Incrementele omzettingen
* Influente omzettingen
* Eerste aanraakconversies
* Laatste aanraakconversies

U kunt elk van de extra kolomkoppen selecteren om de tabel in oplopende of aflopende volgorde te sorteren.

Selecteer **[!UICONTROL Close]** om het uitgevouwen dialoogvenster Bovenste campagnes te sluiten.


### [!UICONTROL Breakdown by touchpoint position]

De visualisatie van [!UICONTROL Breakdown by touchpoint position] is een uitsplitsing van toegewezen omzettingen naar positie van het aanraakpunt en aanraakpunt over alle conversiepaden. Met dit diagram kunt u vergelijken of een aanraakpunt op een positie beter bijdraagt dan de resterende positie en andere aanraakpunten op een willekeurige positie.

>[!NOTE]
>
De som van de procentuele bijdrage voor een toewijzingsmodel voor alle aanraakpunten en posities moet gelijk zijn aan 100.


De posities [!UICONTROL Starter], [!UICONTROL Player] en [!UICONTROL Closer] worden als volgt gedefinieerd:

| Positie | Beschrijving |
|---|---|
| [!UICONTROL Starter] | Deze positie geeft aan of het aanraakpunt de eerste aanraking in een conversiepad is. |
| [!UICONTROL Player] | Deze positie geeft aan of het aanraakpunt niet het eerste of laatste aanraakpunt is dat wordt omgezet. |
| [!UICONTROL Closer] | Deze positie geeft aan of het aanraakpunt het laatste aanraakpunt is vóór de conversie. |


### [!UICONTROL Top conversion paths]

De [!UICONTROL Top conversion paths] visualisatie toont de bovenste 5 omzettingspaden op basis van de geselecteerde attributiemodellen.

Voor elk conversiepad ziet u:

* het aantal kanalen dat wel van invloed is;
* het totaal van de toegewezen paden;
* het percentage toegewezen paden voor dit conversiepad versus het totale toegewezen pad;
* voor elk kanaal, het bijdragepercentage van het toewijzingsmodel, en
* de som van deze bijdragepercentages van het kanaaltoewijzingsmodel.


## [!UICONTROL Diagnostics]

Op het tabblad Diagnostiek worden visualisaties weergegeven voor:

* [!UICONTROL Model Assessment] visualisatie, die u kunt onderverdelen op Ware versus Voorspelde of Resterende omzettingen.

Selecteer **[!UICONTROL Actual vs. Predicted]** of **[!UICONTROL Residuals]** in de lijst **[!UICONTROL Breakdown]** om de visualisatie te onderbreken.

* [!UICONTROL Model fitting metrics] tabel met de volgende kolommen voor elke metrische conversie:

   * Werkelijke omzetting

   * Modelomzetting

   * Restomzetting (verschil tussen werkelijke en gemodelleerde omzetting)

   * Waarden voor modelkwaliteitsscore:

      * R2 (R-kwadraat), dat vertelt hoe goed de gegevens in het regressiemodel passen (de goedheid van fit).

      * MAPE (gemiddelde absolute percentagefout), een van de meest gebruikte PKI&#39;s om de nauwkeurigheid van de voorspelling te meten en geeft de voorspelde fout weer als percentage van de werkelijke waarde.

      * RMSE (Root Mean Square Error): geeft de gemiddelde fout aan, gewogen volgens het vierkant van de fout.

Om een Csv- dossier te downloaden dat de gegevens voor de lijst bevat, uitgezochte ![ Download ](/help/assets/icons/Download.svg).

* [!UICONTROL Touchpoint effectiveness] , die het resultaat van het algoritmische model van Attribution AI vertegenwoordigt. De gegevens voor deze tabel worden alleen voor specifieke tijdsperioden gegenereerd. Selecteer **[!UICONTROL As of *xx/xx/xx, xx:xx TZ *]**![ Info ](/help/assets/icons/InfoOutline.svg) voor meer details.

De visualisatie toont, in dalende orde van [!UICONTROL Efficiency measure] ![ Aflopende Orde ](/help/assets/icons/SortOrderDown.svg), voor elk touchpoint:

   * [!UICONTROL Paths touched]: visualiseert het percentage paden dat omgezet en het percentage paden dat geen omzetting bereikt. Voor een aanraakpunt ziet u meer toegeschreven omzettingen wanneer de hoogte van de conversieverhouding van de eigenschap is. Deze verhouding vergelijkt het percentage wegen die tot omzetting tegenover het percentage wegen leiden die *niet* tot omzetting leiden.
   * [!UICONTROL Efficiency measure]: wordt gegenereerd door het algoritmische toewijzingsmodel. De efficiëntiemaatstaf geeft het relatieve belang aan van een aanraakpunt voor conversie, onafhankelijk van het aanraakpuntvolume. De efficiëntie wordt gemeten op een schaal van 1 tot 5. Het hogere aanraakpuntvolume garandeert geen hogere efficiëntiemaatstaf.
   * [!UICONTROL Total volume]: Het totale aantal keren dat een gebruiker een aanraakpunt aanraakt. Het aantal is inclusief van aanraakpunten die op een weg verschijnen die omzetting evenals wegen *bereiken niet* resulterend in omzetting.

![ Diagnose ](/help/assets/model-insights-diagnostics.png)


## [!UICONTROL Historical overview]

Op het tabblad Historisch overzicht ziet u visualisaties voor:

* Omzetting en besteding per fiscaal Qtr en product.

* Besteed via kanaal.

* Besteed aanraakpunt.

U kunt een alternatief op uitgaven-gebaseerd kanaal selecteren om voor deze visualisatie te tonen. Selecteer een kanaal in **[!UICONTROL Channels]** .

* Volume aanraakpunt.

U kunt een alternatief op volume-gebaseerd kanaal selecteren om voor deze visualisatie te tonen. Selecteer een kanaal in **[!UICONTROL Channels]** .

![ Model - Historisch overzicht ](/help/assets/model-insights-historical-overview.png)

## **[!UICONTROL Edit]**

U kunt de naam, beschrijving en het plannen van opleiding en het noteren van het model uitgeven.

1. Selecteer ![ uitgeven ](/help/assets/icons/Edit.svg) uitgeven

1. In het dialoogvenster **[!UICONTROL Edit model]** :

   * Voer een nieuwe **[!UICONTROL Name]** en **[!UICONTROL Description]** in.

   * Schakel **[!UICONTROL Status]** in om planning in te schakelen. U kunt het plannen voor modellen slechts toelaten die worden opgeleid en worden gescoord.

      1. Selecteer een **[!UICONTROL Scoring frequency]** :

         * **[!UICONTROL Daily]**: Ga een geldige tijd (bijvoorbeeld `05:22 pm`) in of gebruik ![ Klok ](/help/assets/icons/Clock.svg).
         * **[!UICONTROL Weekly]**: Selecteer een dag van de week en ga een geldige tijd (bijvoorbeeld `05:22 pm`) in of gebruik ![ Klok ](/help/assets/icons/Clock.svg).
         * **[!UICONTROL Monthly]**: Selecteer een dag van de maand van de Looppas op elk dropdown menu en ga een geldige tijd (bijvoorbeeld `05:22 pm`) in of gebruik ![ Klok ](/help/assets/icons/Clock.svg).

      1. Selecteer een **[!UICONTROL Training frequency]** in de vervolgkeuzelijst: **[!UICONTROL Monthly]** , **[!UICONTROL Quarterly]** , **[!UICONTROL Yearly]** of **[!UICONTROL None]** .

     ![ geef een model ](../assets/model-edit.png) uit

1. Selecteer **[!UICONTROL Save]** .
