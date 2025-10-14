---
title: Overzicht van modellen
description: Leer hoe u modellen maakt en gebruikt in Mix Modeler.
feature: Models
exl-id: c43d9bc9-4429-45c2-9247-bd24510a24be
source-git-commit: 6855d19347b7f6f1477a6265310df5950b8463c9
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# Overzicht van modellen

Met de modelfunctionaliteit in Mix Modeler kunt u modellen configureren, trainen en behalen die specifiek zijn voor uw bedrijfsdoelstellingen. De training en scoring ondersteunen het leren van overdracht via AI tussen multitouch-attributie en marketingmixmodellering.

De modellen zijn gebaseerd op de geharmoniseerde gegevens die u maakt als onderdeel van de Mix Modeler-toepassingsworkflow.

Een model in Mix Modeler is een model voor machinaal leren dat wordt gebruikt om een bepaald resultaat te meten en te voorspellen op basis van de investeringen van een marketeer. Marketing-aanraakpunten en gegevens op overzichtsniveau kunnen als invoer worden gebruikt. Met Mix Modeler kunt u varianten van modellen maken op basis van verschillende sets variabelen, dimensies en resultaten, zoals inkomsten, verkochte eenheden en leads.

Een model vereist:

* Eén conversie.
* Een of meer marketingaanraakpunten (kanalen) bestaan uit gegevens op overzichtsniveau, marketingaanraakpuntgegevens (gebeurtenisgegevens) of beide.
* Een configureerbaar terugzoekvenster.
* Een configureerbaar trainingsvenster.

Een model kan eventueel het volgende omvatten:

* Externe factoren.
* Interne factoren.
* Eerdere kennis van marketingbijdragen uit andere bronnen, zoals ervaring van belanghebbenden in het verleden, incrementele tests en andere modellen.
* Het aandeel van de uitgaven, dat relatieve uitgavenaandeel als volmacht gebruikt wanneer de marketing gegevens schaars is.

Wanneer een model voor de eerste keer wordt gemaakt, wordt het maken onmiddellijk afgebroken tijdens het training- en scoring-proces. Nadat de initiële training en scoring zijn voltooid, zijn modelinzichten beschikbaar voor evaluatie. Een model kan vervolgens opnieuw worden opgeleid. Ook, kunnen de gegevens aan het model worden toegevoegd dat u vereist om het model manueel opnieuw te centreren. Herscholing en herscholing zijn een herhalend proces, aangezien nieuwe bevindingen en informatie zich voordoen en aanpassingen nodig zijn om een model te verkrijgen dat het meest geschikt is voor uw bedrijfsdoelstellingen.


## Modellen maken

Als u een model wilt maken, gebruikt u de stapsgewijze configuratiestroom van het model met instructies van Mix Modeler die beschikbaar is wanneer u **[!UICONTROL Open model canvas]** selecteert. Zie [&#x200B; modellen bouwen &#x200B;](build.md) voor meer details.

## Modellen beheren

Als u een tabel met uw huidige modellen wilt weergeven, gaat u naar de Mix Modeler-interface:

1. Selecteer ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. U ziet een tabel met de huidige modellen.

   De tabelkolommen geven details over het model op.

   | Kolomnaam | Details |
   |---|---|
   | Naam | Naam van het model |
   | Beschrijving | Beschrijving van het model |
   | Conversion-gebeurtenis | De conversie die u voor het model hebt geselecteerd. |
   | Uitvoerfrequentie | De lopende frequentie van opleiding het model. |
   | Laatste uitvoering | De datum en het tijdstip van de laatste training voor het model. |
   | Status | De status van het model. |

   {style="table-layout:auto"}

   De gerapporteerde status van het model is afhankelijk van de plaats waar een model zich in de levenscyclus bevindt. Of een model bijvoorbeeld is gemaakt, (opnieuw) is opgeleid of niet, of (opnieuw) met succes of niet.

   In de onderstaande tabel:

   * ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) - wijst op een succesvolle uitvoering van een stap in de modellevenscyclus.
   * ![&#x200B; Klok &#x200B;](/help/assets/icons/Clock.svg) - wijst op een huidige aan de gang zijnde uitvoering van een stap in de modellevenscyclus.
   * ![&#x200B; dicht &#x200B;](/help/assets/icons/Close.svg) - wijst op een ontbroken uitvoering van een stap in de modellevenscyclus.

   | Status | [&#x200B; bouwt &#x200B;](/help/models/build.md) | [&#x200B; Lijn &#x200B;](/help/models/train-score.md#train) | [&#x200B; Score &#x200B;](/help/models/train-score.md#score) | [&#x200B; gaat terug &#x200B;](/help/models/train-score.md#train) | [&#x200B; Rescore &#x200B;](/help/models/train-score.md#score) |
   |---|:---:|:---:|:---:|:---:|:---:|
   | In uitvoering | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | | | | |
   | In uitvoering | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Klok &#x200B;](/help/assets/icons/Clock.svg) | | | |
   | In uitvoering | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Klok &#x200B;](/help/assets/icons/Clock.svg) | | |
   | In uitvoering | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Klok &#x200B;](/help/assets/icons/Clock.svg) | |
   | In uitvoering | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Klok &#x200B;](/help/assets/icons/Clock.svg) |
   | Training mislukt | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; dicht &#x200B;](/help/assets/icons/Close.svg) | | | |
   | Training mislukt | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; dicht &#x200B;](/help/assets/icons/Close.svg) | |
   | Training voltooid | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | | | |
   | Training voltooid | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | |
   | Scores mislukt | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; dicht &#x200B;](/help/assets/icons/Close.svg) | | |
   | Scores mislukt | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; dicht &#x200B;](/help/assets/icons/Close.svg) |
   | Scores gelukt | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | | |
   | Scores gelukt | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) |

   {style="table-layout:fixed"}

1. Om de kolommen te veranderen die voor de lijst worden getoond, selecteer ![&#x200B; montages van de Kolom &#x200B;](/help/assets/icons/ColumnSetting.svg) en knevel kolommen op ![&#x200B; Controle &#x200B;](/help/assets/icons/Checkmark.svg) of weg.

U kunt de volgende handelingen uitvoeren op een specifiek model.

### Modelinzichten

De functie voor inzicht in modellen is alleen beschikbaar voor goed opgeleide en gescoreerde modellen.

De inzichten van een model weergeven:

1. Selecteer ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer de modelnaam.

U wordt opnieuw gericht aan [&#x200B; ModelInzichten &#x200B;](insights.md).


### Details weergeven

Meer details van een model bekijken:

1. Selecteer ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer ![&#x200B; Info &#x200B;](/help/assets/icons/Info.svg) voor een model om pop-up met details te tonen.


### Dupliceren

U kunt snel een model dupliceren.

1. Selecteer ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer ![&#x200B; Meer &#x200B;](/help/assets/icons/More.svg) voor een model, en van het contextmenu uitgezocht **[!UICONTROL Duplicate]**.

U wordt opnieuw gericht aan de stappen om een nieuw model, met een voorgestelde naam tot stand te brengen die uit de originele die naam van het model wordt samengesteld met **[!UICONTROL (Copy)] (_n_)** wordt toegevoegd.

### Bewerken

U kunt de naam, beschrijving en het plannen van opleiding en het noteren van een model uitgeven.

1. Selecteer ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer ![&#x200B; Meer &#x200B;](/help/assets/icons/More.svg) voor een model, en van het contextmenu uitgezocht **[!UICONTROL Edit]**.

   In het dialoogvenster **[!UICONTROL Edit model]** :

   * Voer een nieuwe **[!UICONTROL Name]** en **[!UICONTROL Description]** in.

   * Schakel **[!UICONTROL Status]** in om planning in te schakelen. U kunt het plannen voor modellen slechts toelaten die worden opgeleid en worden gescoord.

      1. Selecteer een **[!UICONTROL Scoring frequency]** :

         * **[!UICONTROL Daily]**: Ga een geldige tijd (bijvoorbeeld `05:22 pm`) in of gebruik ![&#x200B; Klok &#x200B;](/help/assets/icons/Clock.svg).
         * **[!UICONTROL Weekly]**: Selecteer een dag van de week en ga een geldige tijd (bijvoorbeeld `05:22 pm`) in of gebruik ![&#x200B; Klok &#x200B;](/help/assets/icons/Clock.svg).
         * **[!UICONTROL Monthly]**: Selecteer een dag van de maand van de Looppas op elk dropdown menu en ga een geldige tijd (bijvoorbeeld `05:22 pm`) in of gebruik ![&#x200B; Klok &#x200B;](/help/assets/icons/Clock.svg).

      1. Selecteer een **[!UICONTROL Training frequency]** in de vervolgkeuzelijst: **[!UICONTROL Monthly]** , **[!UICONTROL Quarterly]** , **[!UICONTROL Yearly]** of **[!UICONTROL None]** .

     ![&#x200B; geef een model &#x200B;](../assets/model-edit.png) uit

1. Selecteer **[!UICONTROL Save]** .



### Trein

Overweeg een model opnieuw op te leiden wanneer u nieuwe incrementele marketing en factorgegevens wilt opnemen. Zie [&#x200B; Lijn en scoremodellen &#x200B;](train-score.md#train) voor meer informatie.


### Score

U kunt een model incrementeel score behalen op basis van nieuwe marketinggegevens of een model opnieuw ordenen voor een specifieke datumreeks. Zie [&#x200B; Lijn en scoremodellen &#x200B;](train-score.md#score) voor meer informatie.


### Modellen verwijderen

Een model verwijderen:

1. Selecteer ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.
1. Selecteer ![&#x200B; Meer &#x200B;](/help/assets/icons/More.svg) voor een model, en van het contextmenu uitgezocht **[!UICONTROL Delete]**. Alternatief, selecteer ![&#x200B; Schrapping &#x200B;](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** van de blauwe actiebar.
1. Selecteer **[!UICONTROL Delete]** in het bevestigingsdialoogvenster van **[!UICONTROL Delete model]** om het model te verwijderen. Selecteer **[!UICONTROL Cancel]** om te annuleren.

Meerdere modellen verwijderen:

1. Selecteer meerdere modellen.
1. Van de blauwe actiebar, uitgezochte ![&#x200B; Schrapping &#x200B;](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** om de modellen te schrappen.
1. Selecteer **[!UICONTROL Delete]** in de **[!UICONTROL Delete *x *modellen]**&#x200B;bevestigingsdialoog om de modellen te schrappen. Selecteer **[!UICONTROL Cancel]**&#x200B;om te annuleren.

