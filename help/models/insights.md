---
title: Modelinzichten
description: Leer hoe u meer details over uw model krijgt, zoals historisch overzicht, modelinzichten en modelkwaliteit in de Mix Modeler.
feature: Models
exl-id: d99852f9-ba0d-4a2e-b5f3-ca0efe6002fd
source-git-commit: 9085363e951a4e306c64ad28f56e2c15b4a6029a
workflow-type: tm+mt
source-wordcount: '1159'
ht-degree: 0%

---

# Modelinzichten

Om modelinzichten te bekijken, in ![Modellen](/help/assets//icons/FileData.svg) **[!UICONTROL Models]** interface in Mix Modeler:

1. Van de **[!UICONTROL Models]** in de tabel, selecteert u de naam van een model met een **[!UICONTROL Last run status]** van <span style="color:green">●</span> **[!UICONTROL Success]**.

1. Selecteer in het contextmenu de optie **[!UICONTROL Model Insights]**.

![Tabbalk Modelinzichten](/help/assets//model-insights-tabbar.png)

U ziet wanneer het opgegeven model voor het laatst is vernieuwd en widgets worden weergegeven met vier tabbladen: [Modelinzichten](#model-insights), [Attributie](#attribution), [Diagnostiek](#diagnostics), en [Historisch overzicht](#historical-overview).

U kunt de datumperiode wijzigen waarop de widgets op elk tabblad zijn gebaseerd. Voer een datumpunt in of selecteer ![Kalender](/help/assets//icons/Calendar.svg) om een datumpunt te selecteren.

## [!UICONTROL Model insights]

Het tabblad Modelinzichten bevat widgets voor:

* Bijdrage op datum en basismedia. De gestapelde grafiek is geordend: Basis bij de bodem, niet-bestede kanalen in het midden, en de kanalen van de Besteed op de bovenkant.

* Bijdrage per kanaal.

* Overzicht van de marketingprestaties.

* Marginale responscurven.
  <br/>Selecteer een kanaal in het menu **[!UICONTROL Channel]** vervolgkeuzelijst om de widget voor een specifiek kanaal bij te werken.

![Model - Modelinzichten](/help/assets//model-insights-insights.png)

U kunt de muisaanwijzer boven afzonderlijke diagramelementen in elke widget plaatsen om een pop-up met meer details weer te geven.

Als u een CSV-bestand met de gegevens voor de widget wilt downloaden, selecteert u ![Downloaden](/help/assets//icons/Download.svg).

Als u gegevens van volledige modelinzichten wilt downloaden in Microsoft® Excel, selecteert u ![Downloaden](/help/assets//icons/Download.svg) **[!UICONTROL Download data]**.

## [!UICONTROL Attribution]

Met de [!UICONTROL Attribution] kunt u de doeltreffendheid begrijpen van aanraakpunten en marketingcampagnes die gegevens op gebeurtenisniveau bevatten. De volgende attribuutmodellen worden ondersteund:

* Gebaseerd op het geselecteerde model in Mix Modeler:
   * Algorithmic - Invloed
   * Algorithmic - Incrementeel
* Gebaseerde regel:
   * Vervaleenheden
   * Eerste aanraking
   * Laatste aanraking
   * Lineair
   * Ushape

Zie [Multi-touch-kenmerk](../get-started/about.md#multi-touch-attribution) voor een inleiding over de multitouch-attributie-mogelijkheid in Mix Modeler.

Selecteer een of meer toewijzingsmodellen in het menu **[!UICONTROL Attribution Model]** vervolgkeuzelijst. De geselecteerde attributiemodellen zijn van toepassing op alle widgets op het tabblad Kenmerken.

![Attributie](/help/assets//model-insights-attribution.png)

De Mix Modeler multi-touch attributie granulaire gebeurtenisscores richten zich op de algemene scores van de Mix Modeler en ROIs. Deze scores worden ook beschikbaar gesteld als datasets in Experience Platform.

Het tabblad Kenmerken bestaat uit de volgende widgets:

### [!UICONTROL Overview]

De [!UICONTROL Overview] widget geeft voor de geselecteerde attributiemodellen de totalen en percentages van de omzettingen weer. Als u meer modellen selecteert, worden extra cirkels aan de visualisatie toegevoegd, elk met een eigen kleur die overeenkomt met de legenda.

Als u een pop-up met details voor een attributiemodel wilt zien, houdt u de muisaanwijzer boven een van de cirkels in de visualisatie.

### [!UICONTROL Trends]

De [!UICONTROL Daily trends], [!UICONTROL Weekly trends], of [!UICONTROL Monthly trends] widget geeft voor de geselecteerde attributiemodellen de dagelijkse, wekelijkse of maandelijkse conversietrends weer.

Selecteer **[!UICONTROL Daily trends]**, **[!UICONTROL Weekly trends]** of **[!UICONTROL Monthly trends]** van ![Meer](/help/assets//icons/More.svg).

Als u details wilt zien, houdt u de muisaanwijzer boven de gegevensregel van een specifiek toewijzingsmodel om een pop-up weer te geven met het totale aantal conversies voor die gegevens.

### [!UICONTROL Breakdown]

De [!UICONTROL Breakdown] widget is een uitsplitsing per kanaal of aanraakpunt van de omzettingen voor elk van de geselecteerde attributiemodellen. Deze widget kan nuttig zijn om beslissingen te nemen over de doeltreffendheid van elk kanaal of aanraakpunt.

Selecteer **[!UICONTROL Breakdown by channel]** of **[!UICONTROL Breakdown by touchpoint]** van ![Meer](/help/assets//icons/More.svg).

Houd de muisaanwijzer boven de diagramelementen om de details weer te geven.

### [!UICONTROL Top campaigns]

De belangrijkste campagnewidget toont een lijst van de hoogste campagnes met kolommen voor de naam van de Campagne, het Kanaal, het type van Media en Incrementele omzettingen. Deze widget kan u helpen uw team te informeren over de effectiviteit van een specifieke campagne voor een bepaald kanaal en u kunt inzichten verschaffen over welke campagnes u verder moet investeren.

Als u de tabel in oplopende ↑ of aflopende volgorde ↓ wilt sorteren voor Kanaal, Mediatype of Incrementele conversies, selecteert u de kolomkop en schakelt u de sortering in of uit.

Als u de tabel in een afzonderlijk dialoogvenster wilt uitvouwen, selecteert u **[!UICONTROL Expand]** van ![Meer](/help/assets//icons/More.svg).

Het uitgevouwen dialoogvenster Boven bevat dezelfde tabel met optelde kolommen voor

* Incrementele omzettingen
* Influente omzettingen
* Eerste aanraakconversies
* Laatste aanraakconversies

  U kunt elk van de extra kolomkoppen selecteren om de tabel in oplopende of aflopende volgorde te sorteren.

Als u het uitgevouwen dialoogvenster Bovenste campagnes wilt sluiten, selecteert u **[!UICONTROL Close]**.


### [!UICONTROL Breakdown by touchpoint position]

De [!UICONTROL Breakdown by touchpoint position] visualisatie is een uitsplitsing van toegerekende omzettingen naar positie van het aanraakpunt en het aanraakpunt over alle omzettingspaden. Met dit diagram kunt u vergelijken of een aanraakpunt op een positie beter bijdraagt dan de resterende positie en andere aanraakpunten op een willekeurige positie.

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

De [!UICONTROL Top conversion paths] bij visualisatie worden de bovenste 5 conversiepaden weergegeven op basis van de geselecteerde toewijzingsmodellen.

Voor elk conversiepad ziet u:

* het aantal kanalen dat wel van invloed is;
* het totaal van de toegewezen paden;
* het percentage toegewezen paden voor dit conversiepad versus het totale toegewezen pad;
* voor elk kanaal, het bijdragepercentage van het toewijzingsmodel, en
* de som van deze bijdragepercentages van het kanaaltoewijzingsmodel.


## [!UICONTROL Diagnostics]

Het tabblad Diagnostiek bevat widgets voor:

* [!UICONTROL Model Assessment] visualisatie, die u kunt afbreken bij Ware versus Voorspelde of Resterende omzettingen.

  Selecteer **[!UICONTROL Actual vs. Predicted]** of **[!UICONTROL Residuals]** van de **[!UICONTROL Breakdown]** lijst.

* [!UICONTROL Model fitting metrics] tabel met de volgende kolommen voor elke metrische omzetting:

   * Werkelijke omzetting

   * Modelomzetting

   * Restomzetting (verschil tussen werkelijke en gemodelleerde omzetting)

   * Waarden voor modelkwaliteitsscore:

      * R2 (R-kwadraat), dat vertelt hoe goed de gegevens in het regressiemodel passen (de goedheid van fit).

      * MAPE (gemiddelde absolute percentagefout), een van de meest gebruikte PKI&#39;s om de nauwkeurigheid van de voorspelling te meten en geeft de voorspelde fout weer als percentage van de werkelijke waarde.

      * RMSE (Root Mean Square Error): geeft de gemiddelde fout aan, gewogen volgens het vierkant van de fout.

  Selecteer ![Downloaden](/help/assets//icons/Download.svg).

* [!UICONTROL Touchpoint effectiveness] tabel, die het resultaat van het algoritmische model Attribution AI vertegenwoordigt. De gegevens voor deze tabel worden alleen voor specifieke tijdsperioden gegenereerd. Selecteren **[!UICONTROL As of *xx/xx/xx, xx:xx TZ *]**![Info](/help/assets//icons/InfoOutline.svg) voor meer informatie .

  De visualisatie wordt in aflopende volgorde weergegeven van [!UICONTROL Efficiency measure] ![Aflopende volgorde](/help/assets//icons/SortOrderDown.svg)voor elk aanraakpunt:

   * [!UICONTROL Paths touched]: visualiseert het percentage paden dat omzetting bereikt en het percentage paden dat geen omzetting bereikt. Voor een aanraakpunt ziet u meer toegeschreven omzettingen wanneer de hoogte van de conversieverhouding van de eigenschap is. Met deze verhouding vergelijkt u het percentage paden dat tot omzetting leidt, met het percentage paden dat dit doet *niet* leiden tot conversie.
   * [!UICONTROL Efficiency measure]: gegenereerd door het algoritmische toewijzingsmodel, geeft de efficiëntiemaatregel het relatieve belang aan van een aanraakpunt voor conversie, onafhankelijk van het aanraakpuntvolume. De efficiëntie wordt gemeten op een schaal van 1 tot 5. Het hogere aanraakpuntvolume garandeert geen hogere efficiëntiemaatstaf.
   * [!UICONTROL Total volume]: Het totale aantal keren dat een gebruiker een aanraakpunt aanraakt. Het aantal is inclusief aanraakpunten op een pad dat conversie en paden mogelijk maakt *niet* resulterend in conversie.

![Diagnostiek](/help/assets//model-insights-diagnostics.png)


## [!UICONTROL Historical overview]

Het tabblad Historisch overzicht bevat widgets voor:

* Omzetting en besteding per fiscaal Qtr en product.

* Besteed via kanaal.

* Besteed aanraakpunt.

  U kunt een alternatief op uitgaven gebaseerd kanaal selecteren om voor deze widget te tonen. Een kanaal selecteren vanuit **[!UICONTROL Channels]**.

* Volume aanraakpunt.

  U kunt een alternatief op volume gebaseerd kanaal selecteren om voor deze widget weer te geven. Een kanaal selecteren vanuit **[!UICONTROL Channels]**.

![Model - Historisch overzicht](/help/assets//model-insights-historical-overview.png)
