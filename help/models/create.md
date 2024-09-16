---
title: Een model maken
description: Leer hoe u een model maakt in de Mix Modeler.
feature: Models
exl-id: e1093c09-1e23-460b-92de-cfb0061112fd
source-git-commit: 9a6c1f1c12ab29da80a1997cfd31ca07b38eaa22
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# Een model maken

Om een model, in de ![ Modellen ](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** interface in Mix Modeler tot stand te brengen, selecteer **[!UICONTROL Open model canvas]**.

Om uw douaneAI-aangedreven modellen te bouwen, verstrekt de interface een stap-voor-stap geleide modelconfiguratiestroom.

1. In de stap **[!UICONTROL Setup]** :

   1. Voer uw model in **[!UICONTROL Name]**, bijvoorbeeld `Demo model` . Voer een **[!UICONTROL Description]** in, bijvoorbeeld `Demo model to explore AI featues of Mix Modeler` .

      ![ Modelnaam en beschrijving ](/help/assets/model-name-description.png)

   1. Selecteer **[!UICONTROL Next]** om door te gaan naar de volgende stap. Selecteer **[!UICONTROL Cancel]** om de modelconfiguratie te annuleren.

1. In de stap **[!UICONTROL Configure]** :

   1. In de sectie **[!UICONTROL Conversion goal]** , in de container:

      1. Voer een **[!UICONTROL Conversion name]** in voor de conversie, bijvoorbeeld `Conversion`

      1. Selecteer een omzetting van **[!UICONTROL *Uitgezochte geharmoniseerd gebied *]**, die de beschikbare omzettingen bevatten u als deel van [ Conversies ](../harmonize-data/conversions.md) in [!UICONTROL Harmonized datasets] bepaalde. Bijvoorbeeld **[!UICONTROL Online Conversion]**.

      1. U kunt ![ Reageren ](/help/assets/icons/Reply.svg) selecteren **[!UICONTROL Create new conversion]** om een omzetting van binnen de modelconfiguratie direct tot stand te brengen.

         ![ Model - omzettingsstap ](/help/assets/model-conversion-step.png)

   1. In de **[!UICONTROL Marketing touchpoints]** sectie, ziet u een aantal marketing touchpoint containers, die aan de marketing touchpoints beantwoorden u als deel van [ de Aanbiedingspunten van de Marketing ](../harmonize-data/marketing-touchpoints.md) in [!UICONTROL Harmonized datasets] bepaalde.

      * Voor elke container:

         1. U kunt de **[!UICONTROL Marketing touchpoint name]** wijzigen.

         1. Selecteer een marketing aanraakpunt van **[!UICONTROL _Uitgezochte marketing aanraakpunt_]**.

         1. U kunt ![ Reageren ](/help/assets/icons/Reply.svg) selecteren **[!UICONTROL Create new marketing touchpoint]** om een marketing contactpunt van binnen de modelconfiguratie direct tot stand te brengen.

      * Om een marketing touchpoint container toe te voegen, voegt de uitgezochte ![ ](/help/assets/icons/AddCircle.svg) toe **[!UICONTROL Add marketing touchpoint]**.

      * Om een marketing touchpoint container, binnen de container te verwijderen, selecteer ![ Meer ](/help/assets/icons/More.svg), en selecteer **[!UICONTROL Remove container]** van het contextmenu.

        ![ Model - marketing touchpoints-stap ](/help/assets/model-marketing-touchpoint-step.png)

   1. Standaard wordt een score gegenereerd voor alle gegevens in de geharmoniseerde weergave. Als u alleen een subset van de populatie wilt scoren, definieert u een of meer filters met behulp van containers in de sectie **[!UICONTROL Eligible data population]** .

      * Definieer voor elke container een of meer gebeurtenissen.

         1. Voor elke gebeurtenis:

            1. Selecteer metrisch of afmeting van **[!UICONTROL _Uitgezochte geharmoniseerd gebied_]**.

            1. Selecteer de juiste operator: **[!UICONTROL equals]**, **[!UICONTROL not equals]**, **[!UICONTROL less than]**, **[!UICONTROL greater than]**, **[!UICONTROL starts with]**, **[!UICONTROL doesn't start with]**, **[!UICONTROL ends with]**, **[!UICONTROL doesn't end with]**, **[!UICONTROL contains]**, **[!UICONTROL doesn't contain]**, **[!UICONTROL is in]** of **[!UICONTROL is not in]** .

            1. Ga of selecteer een waarde bij **[!UICONTROL _binnen of selecteer waarde_]**.

         1. Om een extra gebeurtenis in de container toe te voegen, voegt de uitgezochte ![ ](/help/assets/icons/AddCircle.svg) toe **[!UICONTROL Add event]**.

         1. Om een gebeurtenis uit de container te verwijderen, uitgezochte ![ Sluiten ](/help/assets/icons/Close.svg).

         1. Selecteer **[!UICONTROL Any of]** of **[!UICONTROL All of]** als u wilt filteren met alle of een van de meerdere gebeurtenissen die in de container zijn gedefinieerd. Het label verandert dienovereenkomstig van **[!UICONTROL Include ... Or ...]** in **[!UICONTROL Include ... And ...]** .

      * Om een in aanmerking komende container van de gegevenspopulatie toe te voegen, voegt de uitgezochte ![ ](/help/assets/icons/AddCircle.svg) toe **[!UICONTROL Add eligible population]**.

      * Om een in aanmerking komende container van de gegevenspopulatie, binnen de container te verwijderen, selecteer ![ Meer ](/help/assets/icons/More.svg), en selecteer **[!UICONTROL Remove marketing touchpoint]** van het contextmenu.

        ![ Model - In aanmerking komende gegevenspopulatie ](/help/assets/model-eligible-data-population-step.png)

   1. Als u gegevenssets met externe factoren wilt toevoegen aan uw model, gebruikt u een of meer containers in de sectie **[!UICONTROL External factors dataset]** .

      * Voor elke container:

         1. Ga a **[!UICONTROL Factor name]** bij **[!UICONTROL _binnen factor_]**.

         1. Selecteer een dataset van **[!UICONTROL _Selecteer een dataset_]**. U kunt ![ Gegevens ](/help/assets/icons/Data.svg) selecteren om datasets te beheren. Zie [ Datasets ](../ingest-data/datasets.md) voor meer informatie.

      * Om een extra externe container van de factordataset toe te voegen, voegt de uitgezochte ![ ](/help/assets/icons/AddCircle.svg) toe **[!UICONTROL Add external factor]**.

      * Om een externe container van de factordataset, binnen de container te verwijderen, selecteer ![ Meer ](/help/assets/icons/More.svg), en selecteer **[!UICONTROL Remove external factor]** van het contextmenu.

        ![ Model - Externe factordataset ](/help/assets/model-external-factors-dataset-step.png)


   1. Als u gegevenssets met interne factoren wilt toevoegen aan uw model, gebruikt u een of meer containers in de sectie **[!UICONTROL Internal factors dataset]** .

      * Voor elke container:

         1. Ga a **[!UICONTROL Factor name]** bij **[!UICONTROL _binnen factor_]**.

         1. Selecteer een dataset van **[!UICONTROL _Selecteer een dataset_]**. U kunt ![ Gegevens ](/help/assets/icons/Data.svg) selecteren om datasets te beheren. Zie [ Datasets ](../ingest-data/datasets.md) voor meer informatie.

      * Om een extra interne container van de factordataset toe te voegen, voegt de uitgezochte ![ ](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add internal factor]** toe.

      * Om een extra interne container van de factordataset, binnen de container te verwijderen, selecteer ![ Meer ](/help/assets/icons/More.svg), en **[!UICONTROL Remove internal factor]** van het contextmenu.

        ![ Model - Interne factordataset ](/help/assets/model-internal-factors-dataset-step.png)

   1. Voer een waarde in tussen `1` en `52` in **[!UICONTROL Give contribution credit to touchpoints occurring within]** ... **[!UICONTROL weeks prior to the conversion]** om het terugzoekvenster voor het model te definiëren.

   1. Selecteer **[!UICONTROL Next]** om door te gaan naar de volgende stap. Als er meer configuratie nodig is, wordt met een rode omtrek en tekst uitgelegd welke aanvullende configuratie vereist is. <br/> Uitgezocht **[!UICONTROL Back]** om naar de vorige stap terug te gaan. <br/> Uitgezocht **[!UICONTROL Cancel]** om de modelconfiguratie te annuleren.

1. In de stap **[!UICONTROL Advanced]** :

   1. Selecteer in de sectie **[!UICONTROL Define training window]** tussen

      * **[!UICONTROL Have Mix Modeler select a helpful training window]** en

      * **[!UICONTROL Manually input a training window]**. Wanneer deze optie is geselecteerd, definieert u het aantal jaren in **[!UICONTROL Include events the following years prior to a conversion]** .

        ![ Model - bepaal opleidingsvenster ](/help/assets/model-define-training-window.png)

   1. In de sectie **[!UICONTROL Spend share]** :

      * Activeer **[!UICONTROL Allow spend share]** als u historische investeringsverhoudingen voor marketing wilt gebruiken om het model op de hoogte te brengen wanneer er weinig marketinggegevens beschikbaar zijn.

   1. In de sectie **[!UICONTROL Prior knowledge]** :

      1. Selecteer de **[!UICONTROL Rule type]** .

      1. Geef met de kolom **[!UICONTROL Contribution proportion]** bijdragepercentages op voor elk van de kanalen die onder **[!UICONTROL Name]** worden vermeld.

      1. Indien van toepassing, kunt u voor elk kanaal een **[!UICONTROL Level of confidence]** percentage toevoegen.

      1. Gebruik indien nodig **[!UICONTROL Clear all]** om alle invoerwaarden voor de kolommen **[!UICONTROL Contribution proportion]** en **[!UICONTROL Level of confidence]** te wissen.

         ![ Model - Voorafgaande kennis ](/help/assets/model-prior-knowledge-step.png)

1. Selecteer **[!UICONTROL Finish]** om de modelconfiguratie te voltooien.

   * Selecteer **[!UICONTROL Ok]** in het dialoogvenster **[!UICONTROL Create instance?]** om de eerste reeks training en scoring direct te starten. Uw model is vermeld met status <span style="color:orange"> ・ </span> **[!UICONTROL Awaiting training]**.

     Selecteer **[!UICONTROL Cancel]** om te annuleren.

   * Als er meer configuratie nodig is, wordt met een rode omtrek en tekst uitgelegd welke aanvullende configuratie vereist is.

   Selecteer **[!UICONTROL Back]** om terug te gaan naar de vorige stap.

   Selecteer **[!UICONTROL Cancel]** om de modelconfiguratie te annuleren.
