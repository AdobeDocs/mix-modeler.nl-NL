---
title: Marketing-aanraakpunten
description: Leer hoe u marketingaanraakpunten maakt die u kunt gebruiken als onderdeel van het harmoniseren van uw gegevens in Mix Modeler.
feature: Harmonized Data, Marketing Touch Points
exl-id: 42851107-7568-4bc9-92ca-3cba713a522e
source-git-commit: 6751cea9155bab54c9c8405a57151323f570c477
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Marketing-aanraakpunten {#marketing-touchpoints}

>[!CONTEXTUALHELP]
>id="harmonizeddata_marketingtouchpoints_create"
>title="Marketing-aanraakpunten"
>abstract="Marketing-aanraakpunten zijn marketinggebeurtenissen op het niveau van ontvangers, individuen en cookies die worden gebruikt om het effect van marketinginvesteringen op numerieke of op inkomsten gebaseerde conversies te evalueren.<br/><br/> u kunt niet het model met touchpoints plaatsen die overlappende gegevens hebben en er moet minstens één aanraakpunt met uitgaven zijn."


Marketing-aanraakpunten zijn marketinggebeurtenissen op het niveau van ontvangers, individuen en cookies die worden gebruikt om het effect van marketinginvesteringen op numerieke of op inkomsten gebaseerde conversies te evalueren.

U bepaalt marketing aanraakpunten om u bij attributieanalyse te helpen.

## Marketing-aanraakpunten beheren

Een tabel weergeven met de beschikbare marketingaanraakpunten in de Mix Modeler-interface:

1. Selecteer ![&#x200B; DataSearch &#x200B;](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** van het linkerspoor.

1. Selecteer **[!UICONTROL Marketing touchpoint]** in de bovenste balk. U ziet een lijst van de marketing touchpoints. Als meer pagina&#39;s beschikbaar zijn, gebruik ![&#x200B; Pijl links &#x200B;](/help/assets/icons/ChevronLeft.svg) of ![&#x200B; Pijl rechts &#x200B;](/help/assets/icons/ChevronRight.svg) bij **[!UICONTROL Page _x _van_ x_]** om tussen pagina&#39;s van de lijst te bewegen.

De tabelkolommen geven details over het marketingaanraakpunt:

| Kolomnaam | Details |
| --- | ---|
| Naam | De naam van het marketingpunt. |
| Metrisch draaien | De geharmoniseerde metrische gegevens die moeten worden gebruikt om het bestede aanraakpunt te berekenen. |
| Volume metrisch | De geharmoniseerde metrische gegevens die moeten worden gebruikt om het aanraakpuntvolume te berekenen. |
| Regel | De aanraakpuntregel die moet worden gebruikt. |
| Gemaakt | Datum en tijdstip waarop het marketingaanraakpunt is gecreëerd. |
| Laatst gewijzigd | Datum en tijdstip van de laatste wijziging van het marketingaanraakpunt. |


## Een marketingaanraakpunt toevoegen

Om een marketing aanraakpunt toe te voegen, in ![&#x200B; DataSearch &#x200B;](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Marketing touchpoint]** interface in Mix Modeler:

1. Selecteer ![&#x200B; toevoegen &#x200B;](/help/assets/icons/AddCircle.svg) marketing touchpoint.

1. In het dialoogvenster **[!UICONTROL Marketing touchpoint]** .

   1. Voer een naam in voor **[!UICONTROL Touchpoint Name]**, bijvoorbeeld `Luma Touchpoint` .

   1. Definieer een **[!UICONTROL Touchpoint rule]** .

      1. Selecteer een waarde van **[!UICONTROL *Uitgezochte geharmoniseerde *]**, bijvoorbeeld **[!UICONTROL Brand]**.

      1. Selecteer een waarde voor exploitant ![&#x200B; Chevron &#x200B;](/help/assets/icons/ChevronDown.svg), bijvoorbeeld **[!UICONTROL is]**.

      1. Selecteer een waarde van **[!UICONTROL *Uitgezochte waarde *]**&#x200B;of ga een waarde in, bijvoorbeeld **[!DNL Luma]**.

   1. Selecteer een geharmoniseerd veld in **[!UICONTROL Touchpoint volume]**, bijvoorbeeld **[!UICONTROL Impressions]** .

   1. Selecteer een geharmoniseerd veld in **[!UICONTROL Touchpoint spend]**, bijvoorbeeld **[!UICONTROL Cost]** .

      ![&#x200B; Marketing touchpoint &#x200B;](/help/assets/create-touchpoint.png)

   1. Selecteer **[!UICONTROL Create]** om het marketingaanraakpunt te maken. Als u het maken van een marketingaanraakpunt wilt annuleren, selecteert u **[!UICONTROL Cancel]** .

1. Wanneer gecreeerd, wordt touchpoint toegevoegd aan de marketing touchpoints lijst.


## Details weergeven

Details van een marketingaanraakpunt weergeven:

1. Selecteer ![&#x200B; Meer &#x200B;](/help/assets/icons/More.svg) wanneer het bedekken over een marketing touchpoint naam in de lijst.

1. Selecteer ![&#x200B; Mening &#x200B;](/help/assets/icons/ViewDetail.svg) **Mening**. Een dialoogvenster bevat details over het marketingaanraakpunt. Zie [&#x200B; een marketing touchpoint &#x200B;](#add-a-marketing-touchpoint) voor meer informatie toevoegen. Selecteer **[!UICONTROL Cancel]** om het dialoogvenster te sluiten.


## Rapport weergeven

Een rapport van een marketingaanraakpunt weergeven:

1. Selecteer ![&#x200B; Meer &#x200B;](/help/assets/icons/More.svg) wanneer het bedekken over een marketing touchpoint naam in de lijst.

1. Selecteer ![&#x200B; GraphTrend &#x200B;](/help/assets/icons/GraphTrend.svg) **rapport van de Mening**. Een dialoog toont een rapport van het marketing aanraakpunt.

   ![&#x200B; de marketing touchpoint meningsrapport &#x200B;](../assets/marketingtouchpoint-view-report.png)

   * Selecteer een waarde in het vervolgkeuzemenu **[!UICONTROL Weekly]** als u de granulariteit wilt wijzigen waarop u wilt rapporteren.
   * Om de periode te veranderen om op te melden, ga een begin en einddatum in of gebruik ![&#x200B; Kalender &#x200B;](/help/assets/icons/Calendar.svg) om een periode in kalenderpopup te bepalen.

1. Selecteer **[!UICONTROL Close]** om het dialoogvenster te sluiten.

## Een marketingaanraakpunt verwijderen

Een marketingaanraakpunt verwijderen:

1. Selecteer ![&#x200B; Schrapping &#x200B;](/help/assets/icons/Delete.svg) **Schrapping** wanneer het hangen over een marketing touchpoint naam in de lijst.
1. Selecteer **[!UICONTROL Delete touchpoint]** in het dialoogvenster voor bevestiging van het dialoogvenster **[!UICONTROL Delete]** om het marketingaanraakpunt permanent te verwijderen.

