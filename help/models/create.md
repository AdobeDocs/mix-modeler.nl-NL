---
title: Een model maken
description: Leer hoe u een model maakt in de Mix Modeler.
feature: Models
exl-id: e1093c09-1e23-460b-92de-cfb0061112fd
source-git-commit: 9085363e951a4e306c64ad28f56e2c15b4a6029a
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# Een model maken

Om een model te creëren, in ![Modellen](/help/assets//icons/FileData.svg) **[!UICONTROL Models]** interface in Mix Modeler, selecteert u **[!UICONTROL Open model canvas]**.

Om uw douaneAI-aangedreven modellen te bouwen, verstrekt de interface een stap-voor-stap geleide modelconfiguratiestroom.

1. In de **[!UICONTROL Setup]** stap:

   1. Voer uw model in **[!UICONTROL Name]** bijvoorbeeld `Demo model`. Voer een **[!UICONTROL Description]** bijvoorbeeld `Demo model to explore AI featues of Mix Modeler`.

      ![Modelnaam en -beschrijving](/help/assets//model-name-description.png)

   1. Selecteren **[!UICONTROL Next]** om door te gaan met de volgende stap. Selecteren **[!UICONTROL Cancel]** om de modelconfiguratie te annuleren.

1. In de **[!UICONTROL Configure]** stap:

   1. In de **[!UICONTROL Conversion goal]** in de container:

      1. Voer een **[!UICONTROL Conversion name]** voor de conversie, bijvoorbeeld `Conversion`

      1. Een conversie selecteren vanuit **[!UICONTROL *Geharmoniseerd veld selecteren *]**met de beschikbare omzettingen die u als onderdeel van [Conversies](../harmonize-data/conversions.md) in [!UICONTROL Harmonized datasets]. Bijvoorbeeld:**[!UICONTROL Online Conversion]**.

      1. U kunt ![Antwoord](/help/assets//icons/Reply.svg) **[!UICONTROL Create new conversion]** om een omzetting direct van binnen de modelconfiguratie tot stand te brengen.

         ![Model - conversiefase](/help/assets//model-conversion-step.png)

   1. In de **[!UICONTROL Marketing touchpoints]** in, ziet u een aantal marketingcontainers voor aanraakpunten die overeenkomen met de marketingaanraakpunten die u hebt gedefinieerd als onderdeel van [Marketing-aanraakpunten](../harmonize-data/marketing-touchpoints.md) in [!UICONTROL Harmonized datasets].

      * Voor elke container:

         1. U kunt de **[!UICONTROL Marketing touchpoint name]**.

         1. Een marketingaanraakpunt selecteren vanuit **[!UICONTROL _Aanraakpunt voor marketing selecteren_]**.

         1. U kunt ![Antwoord](/help/assets//icons/Reply.svg) **[!UICONTROL Create new marketing touchpoint]** om een marketing contactpunt van binnen de modelconfiguratie direct tot stand te brengen.

      * Als u een touchpoint-container voor marketingdoeleinden wilt toevoegen, selecteert u ![Toevoegen](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add marketing touchpoint]**.

      * Om een marketing touchpoint container, binnen de container te verwijderen, selecteer ![Meer](/help/assets//icons/More.svg)en selecteert u **[!UICONTROL Remove container]** in het contextmenu.

        ![Model - het in de handel brengen van touchpoints](/help/assets//model-marketing-touchpoint-step.png)

   1. Standaard wordt een score gegenereerd voor alle gegevens in de geharmoniseerde weergave. Als u alleen een subset van de populatie wilt scoren, definieert u een of meer filters met behulp van containers in het dialoogvenster **[!UICONTROL Eligible data population]** sectie.

      * Definieer voor elke container een of meer gebeurtenissen.

         1. Voor elke gebeurtenis:

            1. Selecteer een metrische of een afmeting van **[!UICONTROL _Geharmoniseerd veld selecteren_]**.

            1. Selecteer de juiste operator: **[!UICONTROL equals]**, **[!UICONTROL not equals]**, **[!UICONTROL less than]**, **[!UICONTROL greater than]**, **[!UICONTROL starts with]**, **[!UICONTROL doesn't start with]**, **[!UICONTROL ends with]**, **[!UICONTROL doesn't end with]**, **[!UICONTROL contains]**, **[!UICONTROL doesn't contain]**, **[!UICONTROL is in]**, of **[!UICONTROL is not in]**.

            1. Voer een waarde in of selecteer een waarde bij **[!UICONTROL _Waarde invoeren of selecteren_]**.

         1. Als u een extra gebeurtenis in de container wilt toevoegen, selecteert u ![Toevoegen](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add event]**.

         1. Selecteer ![Sluiten](/help/assets//icons/Close.svg).

         1. Als u wilt filteren met alle of meerdere gebeurtenissen die in de container zijn gedefinieerd, selecteert u **[!UICONTROL Any of]** of **[!UICONTROL All of]**. Het label verandert dienovereenkomstig van **[!UICONTROL Include ... Or ...]** tot **[!UICONTROL Include ... And ...]**.

      * Als u een in aanmerking komende container voor gegevenspopulatie wilt toevoegen, selecteert u ![Toevoegen](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add eligible population]**.

      * Als u een in aanmerking komende container voor een gegevenspopulatie wilt verwijderen, selecteert u ![Meer](/help/assets//icons/More.svg)en selecteert u **[!UICONTROL Remove marketing touchpoint]** in het contextmenu.

        ![Model - In aanmerking komende gegevenspopulatie](/help/assets//model-eligible-data-population-step.png)

   1. Om datasets toe te voegen die externe factoren aan uw model bevatten, gebruik één of meerdere containers in **[!UICONTROL External factors dataset]** sectie.

      * Voor elke container:

         1. Voer een **[!UICONTROL Factor name]** om **[!UICONTROL _Factor invoeren_]**.

         1. Een gegevensset selecteren vanuit **[!UICONTROL _Een gegevensset selecteren_]**. U kunt ![Gegevens](/help/assets//icons/Data.svg) om gegevenssets te beheren. Zie [Gegevenssets](../ingest-data/datasets.md) voor meer informatie .

      * Als u een extra container voor externe factoren wilt toevoegen, selecteert u ![Toevoegen](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add external factor]**.

      * Om een externe container van de factordataset, binnen de container te verwijderen, selecteer ![Meer](/help/assets//icons/More.svg)en selecteert u **[!UICONTROL Remove external factor]** in het contextmenu.

        ![Model - Gegevensset externe factoren](/help/assets//model-external-factors-dataset-step.png)


   1. Om datasets toe te voegen die interne factoren aan uw model bevatten, gebruik één of meerdere containers in **[!UICONTROL Internal factors dataset]** sectie.

      * Voor elke container:

         1. Voer een **[!UICONTROL Factor name]** om **[!UICONTROL _Factor invoeren_]**.

         1. Een gegevensset selecteren vanuit **[!UICONTROL _Een gegevensset selecteren_]**. U kunt ![Gegevens](/help/assets//icons/Data.svg) om gegevenssets te beheren. Zie [Gegevenssets](../ingest-data/datasets.md) voor meer informatie .

      * Als u een extra gegevenssetcontainer met interne factoren wilt toevoegen, selecteert u ![Toevoegen](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add internal factor]**.

      * Om een extra interne container van de factorendataset, binnen de container te verwijderen, selecteer ![Meer](/help/assets//icons/More.svg), en **[!UICONTROL Remove internal factor]** in het contextmenu.

        ![Model - Gegevensset met interne factoren](/help/assets//model-internal-factors-dataset-step.png)

   1. Voer een waarde in tussen `1` en `52` in **[!UICONTROL Give contribution credit to touchpoints occurring within]** ... **[!UICONTROL weeks prior to the conversion]**.

   1. Selecteren **[!UICONTROL Next]** om door te gaan met de volgende stap. Als er meer configuratie nodig is, wordt met een rode omtrek en tekst uitgelegd welke aanvullende configuratie vereist is. <br/>Selecteren **[!UICONTROL Back]** om terug te gaan naar de vorige stap. <br/>Selecteren **[!UICONTROL Cancel]** om de modelconfiguratie te annuleren.

1. In de **[!UICONTROL Advanced]** stap:

   1. In de **[!UICONTROL Define training window]** sectie selecteert u tussen

      * **[!UICONTROL Have Mix Modeler select a helpful training window]** en

      * **[!UICONTROL Manually input a training window]**. Indien geselecteerd, bepaal het aantal jaren in **[!UICONTROL Include events the following years prior to a conversion]**.

        ![Model - Het trainingsvenster definiëren](/help/assets//model-define-training-window.png)

   1. In de **[!UICONTROL Spend share]** sectie:

      * Als u historische investeringsverhoudingen voor marketing wilt gebruiken om het model te informeren wanneer marketinggegevens gering zijn, activeert u **[!UICONTROL Allow spend share]**.

   1. In de **[!UICONTROL Prior knowledge]** sectie:

      1. Selecteer de **[!UICONTROL Rule type]**.

      1. Geef bijdragepercentages op voor de kanalen die onder **[!UICONTROL Name]**, met de **[!UICONTROL Contribution proportion]** kolom.

      1. Indien nodig kunt u voor elk kanaal een **[!UICONTROL Level of confidence]** percentage.

      1. Indien nodig, gebruik **[!UICONTROL Clear all]** om alle invoerwaarden voor de **[!UICONTROL Contribution proportion]** en **[!UICONTROL Level of confidence]** kolommen.

         ![Model - Voorafgaande kennis](/help/assets//model-prior-knowledge-step.png)

1. Selecteren **[!UICONTROL Finish]** om uw modelconfiguratie te voltooien.

   * In de **[!UICONTROL Create instance?]** dialoogvenster, selecteren **[!UICONTROL Ok]** om de eerste reeks training en scoring onmiddellijk te starten. Uw model wordt weergegeven met de status <span style="color:orange">●</span> **[!UICONTROL Awaiting training]**.

     Selecteren **[!UICONTROL Cancel]** om te annuleren.

   * Als er meer configuratie nodig is, wordt met een rode omtrek en tekst uitgelegd welke aanvullende configuratie vereist is.

   Selecteren **[!UICONTROL Back]** om terug te gaan naar de vorige stap.

   Selecteren **[!UICONTROL Cancel]** om de modelconfiguratie te annuleren.
