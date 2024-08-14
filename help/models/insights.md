---
title: Modelinzichten
description: Leer hoe u meer details over uw model krijgt, zoals historisch overzicht, modelinzichten en modelkwaliteit in de Mix Modeler.
feature: Models
exl-id: d99852f9-ba0d-4a2e-b5f3-ca0efe6002fd
source-git-commit: 6897f27520705f54d3f23018903a52536083b339
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 0%

---

# Modelinzichten

Om modelinzichten, in de ![ Modellen ](/help/assets//icons/FileData.svg) **[!UICONTROL Models]** interface in Mix Modeler te bekijken:

1. Van de **[!UICONTROL Models]** lijst, selecteer de naam van een model dat a **[!UICONTROL Last run status]** van <span style="color:green"> heeft </span> **[!UICONTROL Success]**.

1. Selecteer **[!UICONTROL Model Insights]** in het contextmenu.

![ Model inzichten lusjebar ](/help/assets//model-insights-tabbar.png)

U ziet wanneer het gespecificeerde model het laatst verfrist is en widgets gebruikend vier lusjes worden getoond: [ Modelinzichten ](#model-insights), [ Attributie ](#attribution), [ Factoren ](#factors), [ Diagnose ](#diagnostics), en [ Historisch overzicht ](#historical-overview).

U kunt de datumperiode wijzigen waarop de widgets op elk tabblad zijn gebaseerd. Ga een datumperiode in of selecteer ![ Kalender ](/help/assets//icons/Calendar.svg) om een datumperiode te selecteren.

## [!UICONTROL Model insights]

Het tabblad Modelinzichten bevat widgets voor:

* Bijdrage op datum en basismedia. De gestapelde grafiek is geordend: Basis bij de bodem, niet-bestede kanalen in het midden, en de kanalen van de Besteed op de bovenkant.

* Bijdrage per kanaal.

* Overzicht van de marketingprestaties.

* Marginale responscurven.  Zowel de curve als de bijbehorende waarden worden berekend op basis van het geselecteerde gegevensbereik. Bovendien toont deze widget het punt van marginale break even en het punt van dalende winst.
  <br/> selecteer een kanaal van de **[!UICONTROL Channel]** dropdown lijst om widget voor een specifiek kanaal bij te werken.

![ Model - Modelinzichten ](/help/assets//model-insights-insights.png)

U kunt de muisaanwijzer boven afzonderlijke diagramelementen in elke widget plaatsen om een pop-up met meer details weer te geven.

Om een Csv- dossier te downloaden dat de gegevens voor widget bevat, uitgezochte ![ Download ](/help/assets//icons/Download.svg).

Om de volledige gegevens van modelinzichten in Microsoft® Excel formaat te downloaden, selecteer ![ Download ](/help/assets//icons/Download.svg) **[!UICONTROL Download data]**.

## [!UICONTROL Attribution]

Met het tabblad [!UICONTROL Attribution] kunt u de effectiviteit begrijpen van aanraakpunten en marketingcampagnes die gegevens op gebeurtenisniveau bevatten. De volgende attribuutmodellen worden ondersteund:

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

Selecteer een of meer toewijzingsmodellen in de vervolgkeuzelijst **[!UICONTROL Attribution Model]** . De geselecteerde attributiemodellen zijn van toepassing op alle widgets op het tabblad Kenmerken.

![ Attributie ](/help/assets//model-insights-attribution.png)

De Mix Modeler multi-touch attributie granulaire gebeurtenisscores richten zich op de algemene scores van de Mix Modeler en ROIs. Deze scores worden ook beschikbaar gesteld als datasets in Experience Platform.

Het tabblad Kenmerken bestaat uit de volgende widgets:

### [!UICONTROL Overview]

De [!UICONTROL Overview] -widget geeft voor de geselecteerde attributiemodellen de totalen en percentages van de omzettingen weer. Als u meer modellen selecteert, worden extra cirkels aan de visualisatie toegevoegd, elk met een eigen kleur die overeenkomt met de legenda.

Als u een pop-up met details voor een attributiemodel wilt zien, houdt u de muisaanwijzer boven een van de cirkels in de visualisatie.

### [!UICONTROL Trends]

De widget [!UICONTROL Daily trends] , [!UICONTROL Weekly trends] of [!UICONTROL Monthly trends] geeft voor de geselecteerde attributiemodellen de dagelijkse, wekelijkse of maandelijkse conversietrends weer.

Om de periode te kiezen, selecteer **[!UICONTROL Daily trends]**, **[!UICONTROL Weekly trends]** of **[!UICONTROL Monthly trends]** van ![ Meer ](/help/assets//icons/More.svg).

Als u details wilt zien, houdt u de muisaanwijzer boven de gegevensregel van een specifiek toewijzingsmodel om een pop-up weer te geven met het totale aantal conversies voor die gegevens.

### [!UICONTROL Breakdown]

De [!UICONTROL Breakdown] -widget is een uitsplitsing naar kanaal of aanraakpunt van de conversies voor elk van de geselecteerde attributiemodellen. Deze widget kan nuttig zijn om beslissingen te nemen over de doeltreffendheid van elk kanaal of aanraakpunt.

Om het verdelingstype te kiezen, selecteer **[!UICONTROL Breakdown by channel]** of **[!UICONTROL Breakdown by touchpoint]** van ![ Meer ](/help/assets//icons/More.svg).

Houd de muisaanwijzer boven de diagramelementen om de details weer te geven.

### [!UICONTROL Top campaigns]

De belangrijkste campagnewidget toont een lijst van de hoogste campagnes met kolommen voor de naam van de Campagne, het Kanaal, het type van Media en Incrementele omzettingen. Deze widget kan u helpen uw team te informeren over de effectiviteit van een specifieke campagne voor een bepaald kanaal en u kunt inzichten verschaffen over welke campagnes u verder moet investeren.

Als u de tabel in oplopende ↑ of aflopende volgorde ↓ wilt sorteren voor Kanaal, Mediatype of Incrementele conversies, selecteert u de kolomkop en schakelt u de sortering in of uit.

Om de lijst in een afzonderlijke dialoog uit te breiden, selecteer **[!UICONTROL Expand]** van ![ Meer ](/help/assets//icons/More.svg).

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
>De som van de procentuele bijdrage voor een toewijzingsmodel voor alle aanraakpunten en posities moet gelijk zijn aan 100.


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

## **[!UICONTROL Factors]**

Op het tabblad Factoren staan inzichten met betrekking tot externe factoren.

![ Factoren ](/help/assets/factors.png)

Om een Csv- dossier te downloaden dat de gegevens voor de lijst bevat, uitgezochte ![ Download ](/help/assets//icons/Download.svg).

Als geen gegevens beschikbaar zijn ziet u een bericht ![ TableAndChart ](/help/assets/icons/TableAndChart.svg) **[!UICONTROL No data is available, you may need to retrain your model, or change the date range to view insights]**.

## [!UICONTROL Diagnostics]

Het tabblad Diagnostiek bevat widgets voor:

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

  Om een Csv- dossier te downloaden dat de gegevens voor de lijst bevat, uitgezochte ![ Download ](/help/assets//icons/Download.svg).

* [!UICONTROL Touchpoint effectiveness] , die het resultaat van het algoritmische model van de Attribution AI vertegenwoordigt. De gegevens voor deze tabel worden alleen voor specifieke tijdsperioden gegenereerd. Selecteer **[!UICONTROL As of *xx/xx/xx, xx:xx TZ *]**![ Info ](/help/assets//icons/InfoOutline.svg) voor meer details.

  De visualisatie toont, in dalende orde van [!UICONTROL Efficiency measure] ![ Aflopende Orde ](/help/assets//icons/SortOrderDown.svg), voor elk touchpoint:

   * [!UICONTROL Paths touched]: visualiseert het percentage paden dat omgezet en het percentage paden dat geen omzetting bereikt. Voor een aanraakpunt ziet u meer toegeschreven omzettingen wanneer de hoogte van de conversieverhouding van de eigenschap is. Deze verhouding vergelijkt het percentage wegen die tot omzetting tegenover het percentage wegen leiden die *niet* tot omzetting leiden.
   * [!UICONTROL Efficiency measure]: wordt gegenereerd door het algoritmische toewijzingsmodel. De efficiëntiemaatstaf geeft het relatieve belang aan van een aanraakpunt voor conversie, onafhankelijk van het aanraakpuntvolume. De efficiëntie wordt gemeten op een schaal van 1 tot 5. Het hogere aanraakpuntvolume garandeert geen hogere efficiëntiemaatstaf.
   * [!UICONTROL Total volume]: Het totale aantal keren dat een gebruiker een aanraakpunt aanraakt. Het aantal is inclusief van aanraakpunten die op een weg verschijnen die omzetting evenals wegen *bereiken niet* resulterend in omzetting.

![ Diagnose ](/help/assets//model-insights-diagnostics.png)


## [!UICONTROL Historical overview]

Het tabblad Historisch overzicht bevat widgets voor:

* Omzetting en besteding per fiscaal Qtr en product.

* Besteed via kanaal.

* Besteed aanraakpunt.

  U kunt een alternatief op uitgaven gebaseerd kanaal selecteren om voor deze widget te tonen. Selecteer een kanaal in **[!UICONTROL Channels]** .

* Volume aanraakpunt.

  U kunt een alternatief op volume gebaseerd kanaal selecteren om voor deze widget weer te geven. Selecteer een kanaal in **[!UICONTROL Channels]** .

![ Model - Historisch overzicht ](/help/assets//model-insights-historical-overview.png)
