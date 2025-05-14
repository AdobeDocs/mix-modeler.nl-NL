---
title: Abonnementen maken
description: Leer hoe u plannen maakt in Mix Modeler.
feature: Plans
exl-id: 6d61d0b2-5871-4d00-9a35-73fff0a1c3e5
source-git-commit: 3545a7045478108db4d9f6bb87df679bfede5a45
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 0%

---


# Abonnementen maken

In Mix Modeler maakt u een abonnement met behulp van het plancanvas. In het plancanvas, kunt u opstelling de details en de begrotingen van uw plan en het onderliggende model voor uw plan gebruiken. Nadat u details, budget en model hebt opgegeven, kunt u doorgaan met een door AI aanbevolen plan of de uitgave via het kanaal bewerken.

Om een plan, in de ![ PLan ](/help/assets/icons/FileChart.svg) **[!UICONTROL Plans]** interface in Mix Modeler tot stand te brengen, selecteer **[!UICONTROL Create plan]**.


1. In het **[!UICONTROL Plan creation]** -scherm:

   1. In de sectie **[!UICONTROL Setup]** :

      1. Voer een **[!UICONTROL Plan name]** in, bijvoorbeeld `Demo plan` . Voer een **[!UICONTROL Description]** in, bijvoorbeeld `Demo plan for Luma company` .
      1. Selecteer a **[!UICONTROL Model]** van **[!UICONTROL _Uitgezocht een optie._.]**
      1. U kunt ![ LinkOut ](/help/assets/icons/LinkOut.svg) selecteren **[!UICONTROL Create model]** om een model van binnen de planverwezenlijking direct tot stand te brengen. Dit zal een nieuw lusje in uw browser openen en zal de [ Modellen ](../models/overview.md) interface tonen.

         ![ Opstelling van het Plan ](/help/assets/plan-setup.png)

   1. In de sectie **[!UICONTROL Budget]** :

      1. Specificeer een datumwaaier, of door data te typen of een datumwaaier te selecteren gebruikend ![ Kalender ](/help/assets/icons/Calendar.svg).
      1. Voer een budget in.

      Om extra datumwaaiers, elk met hun begroting toe te voegen, selecteer ![ CalendarAdd ](/help/assets/icons/CalendarAdd.svg) **[!UICONTROL Add row]**.

      Om een datumwaaier en een bijbehorend budget te schrappen, uitgezochte ![ Sluiten ](/help/assets/icons/Close.svg).

      Een bepaald maximumbudget definiëren:

      1. Schakel **[!UICONTROL Maximize budget]** in.
      1. Geef het bedrag van de maximumbegroting op. Het bedrag moet gelijk zijn aan of hoger zijn dan het totale bedrag van de begrotingen die voor de datumbereiken zijn gespecificeerd.

         ![ begroting van het Plan ](/help/assets/plan-budget.png)

   1. Selecteer **[!UICONTROL Next]** .

1. In het dialoogvenster **[!UICONTROL Done with all required fields]** :

   ![ Plan Gereed ](/help/assets/plan-done-required-fields.png)

   * Selecteer ![ NewPlan ](../assets/icons/NewPlan.svg) **[!UICONTROL Create plan now]** als u een AI geadviseerd plan met voorspelde ROI wilt produceren.

     Selecteer **[!UICONTROL OK]** . Uw abonnement is gemaakt.


   * Selecteer ![ TableEdit ](/help/assets/icons/TableEdit.svg) **[!UICONTROL Edit channel budgets first]** als u kanaalbegroting wilt uitgeven en geavanceerde configuraties bepalen alvorens een plan met voorspelde ROI wordt gecreeerd.

     Selecteer **[!UICONTROL OK]** , zodat u in de volgende stap het kanaal kunt definiëren dat u in **[!UICONTROL Spend selection]** uitgeeft.



1. In de **[!UICONTROL Spend selection]** sectie, voor elke waaier van de begrotingsdatum, gebruik ![ Chevron ](/help/assets/icons/ChevronRight.svg) bovenkant open de mening van de kanaaldistributie voor die gegevenswaaier.

   1. Als u budgetten voor elk kanaal wilt definiëren, voert u een waarde in voor **[!UICONTROL Min]** en **[!UICONTROL Max]** of gebruikt u de schuifregelaars.

   1. Als u wilt schakelen tussen valuta- of percentageinvoer, selecteert u **[!UICONTROL $]** of **[!UICONTROL %]** for **[!UICONTROL View spend by]** .

      ![ besteedt selectie ](/help/assets/plan-spend-selection.png)

   1. Selecteer **[!UICONTROL Next]** .


1. In de sectie **[!UICONTROL Advanced configurations]** kunt u optionele geavanceerde configuraties invoeren.

   ![ Overzicht van het Plan ](../assets/plan-advanced-configurations.png)

   * De naam, het model, het datumbereik en het totale budget van uw abonnement worden samengevat.

   * Mix Modeler berekent standaard automatisch de gemiddelde omzet per conversie aan de hand van de meest recente seizoensgebonden gegevens. In **[!UICONTROL Average Revenue per conversion]** kunt u specifieke gemiddelde omzet per omzetting bepalen.

      1. Voor elk datumbereik in uw budget:

         1. Selecteer een datumbereik in het vervolgkeuzemenu **[!UICONTROL Date range]** .
         1. Voer een **[!UICONTROL Average revenue]** -waarde in.

      1. Selecteer ![ AddCircle ](/help/assets/icons/AddCircle.svg) voeg douanegemiddelde opbrengst per omzettingseenheid toe om een datumwaaier toe te voegen.
      1. Selecteer ![ RemoveCircle ](/help/assets/icons/RemoveCircle.svg) om een datumwaaier te verwijderen.

     >[!NOTE]
     >
     >Als uw model geen historische opbrengstgegevens omvat, moet u een gemiddelde opbrengst per omzetting voor elke datumwaaier bepalen u voor uw begroting specificeerde.
     >

   * Standaard berekent Mix Modeler automatisch kanaalkosten aan de hand van de meest recente seizoensgebonden gegevens. In **[!UICONTROL Channel costs]** kunt u aangepaste kanaalkosten definiëren.

      1. Voor elk kanaal in uw model, bepaal de kosten van het douanekanaal.

         1. Selecteer een kanaal in het vervolgkeuzemenu **[!UICONTROL Channel]** .
         1. Voor elk datumbereik in uw budget:
            1. Selecteer een datumbereik in het vervolgkeuzemenu **[!UICONTROL Date range]** .
            1. Voer een **[!UICONTROL Average revenue]** -waarde in.
         1. Selecteer ![ AddCircle ](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add custom average revenue per conversion unit]** om een datumwaaier toe te voegen.
         1. Selecteer ![ RemoveCircle ](/help/assets/icons/RemoveCircle.svg) om een datumwaaier te verwijderen.

      1. Selecteer ![ AddCircle ](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add custom channel cost]** om een kanaal toe te voegen.
      1. Selecteer ![ CrossSize400 ](/help/assets/icons/CrossSize400.svg) om een douanekanaal te verwijderen.


   1. Selecteer **[!UICONTROL Create]** als u klaar bent.

   1. Selecteer **[!UICONTROL Create plan]** in het dialoogvenster **[!UICONTROL Create plan]** om uw abonnement te maken. Selecteer **[!UICONTROL Cancel]** om het maken van uw abonnement te annuleren. Er wordt een dialoogvenster **[!UICONTROL No work is saved]** weergegeven ter bevestiging.

