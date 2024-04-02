---
title: Modelinzichten
description: Leer hoe u meer details over uw model krijgt, zoals historisch overzicht, modelinzichten en modelkwaliteit in de Mix Modeler.
feature: Models
exl-id: d99852f9-ba0d-4a2e-b5f3-ca0efe6002fd
source-git-commit: 4f4c7f05e90d73a0ab4865150b1ec4c2af88fc12
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Modelinzichten

Om modelinzichten te bekijken, in ![Modellen](../assets/icons/FileData.svg) **[!UICONTROL Models]** interface in Mix Modeler:

1. Selecteer de naam van een model met een **[!UICONTROL Last run status]** van <span style="color:green">●</span> **[!UICONTROL Success]** van de **[!UICONTROL Models]** tabel.

1. Selecteer in het contextmenu de optie **[!UICONTROL Model Insights]**.

U ziet wanneer het opgegeven model voor het laatst is vernieuwd en de widgets worden weergegeven met drie tabbladen: Historisch overzicht, Modelinzichten en Modelkwaliteit.

U kunt de datumperiode wijzigen waarop de widgets op elk tabblad zijn gebaseerd. Voer een datumpunt in of selecteer ![Kalender](../assets/icons/Calendar.svg) om een datumpunt te selecteren.


## Historisch overzicht

Het tabblad Historisch overzicht bevat widgets voor:

* Omzetting en besteding per fiscaal Qtr en product.

* Besteed via kanaal.

* Besteed aanraakpunt.

  U kunt een alternatief op uitgaven gebaseerd kanaal selecteren om voor deze widget te tonen. Een kanaal selecteren vanuit **[!UICONTROL Channels]**.

* Volume aanraakpunt.

  U kunt een alternatief op volume gebaseerd kanaal selecteren om voor deze widget weer te geven. Een kanaal selecteren vanuit **[!UICONTROL Channels]**.

![Model - Historisch overzicht](../assets/model-historical-overview.png)

## Modelinzichten

Het tabblad Modelinzichten bevat widgets voor:

* Bijdrage op datum en basismedia. De gestapelde grafiek is geordend: Basis bij de bodem, niet-bestede kanalen in het midden, en de kanalen van de Besteed op de bovenkant.

* Bijdrage per kanaal.

* Overzicht van de marketingprestaties.

* Marginale responscurven.

![Model - Modelinzichten](../assets/model-model-insights.png)

U kunt de muisaanwijzer boven afzonderlijke diagramelementen in elke widget plaatsen om een pop-up met meer details weer te geven.

Als u een CSV-bestand met de gegevens voor de widget wilt downloaden, selecteert u ![Downloaden](../assets/icons/Download.svg).

Als u gegevens van volledige modelinzichten wilt downloaden in Microsoft® Excel, selecteert u ![Downloaden](../assets/icons/Download.svg) **[!UICONTROL Download data]**.


## Modelkwaliteit

![Modelkwaliteitsbeoordeling](/help/assets/model-quality-assessment.png)
Het tabblad Modelkwaliteit bevat een

* [!UICONTROL Model Assessment] visualisatie, die u kunt afbreken bij Ware versus Voorspelde of Resterende omzettingen.

  Selecteer **[!UICONTROL Actual vs. Predicted]** of **[!UICONTROL Residuals]** van de **[!UICONTROL Breakdown]** lijst.

* [!UICONTROL Model fitting metrics] tabel met de volgende kolommen voor elke metrische omzetting:

   * Werkelijke omzetting

   * Modelomzetting

   * Restomzetting (verschil tussen werkelijke en gemodelleerde omzetting)

   * Waarden voor modelkwaliteitsscore:

      * R2 (R-kwadraat), dat vertelt hoe goed de gegevens in het regressiemodel passen (de goedheid van fit).

      * MAPE (gemiddelde absolute percentagefout), een van de meest gebruikte PKI&#39;s om de nauwkeurigheid van de voorspelling te meten en geeft de voorspelde fout weer als percentage van de werkelijke waarde.

      * RMSE (Root Mean Square Error): geeft de gemiddelde &quot;error&quot; aan, gewogen volgens het vierkant van de fout.

  Selecteer ![Downloaden](../assets/icons/Download.svg).
