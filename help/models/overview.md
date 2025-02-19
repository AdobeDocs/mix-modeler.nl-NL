---
title: Overzicht van modellen
description: Leer hoe u modellen maakt en gebruikt in Mix Modeler.
feature: Models
exl-id: c43d9bc9-4429-45c2-9247-bd24510a24be
source-git-commit: 39ea5ed145678d6ac7e5263b38255e725e488f8d
workflow-type: tm+mt
source-wordcount: '1090'
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


## Modellen maken

Als u een model wilt maken, gebruikt u de stapsgewijze configuratiestroom van het model met instructies van Mix Modeler die beschikbaar is wanneer u **[!UICONTROL Open model canvas]** selecteert. Zie [ modellen bouwen ](build.md) voor meer details.

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

   * ![ Vinkje ](/help/assets/icons/Checkmark.svg) - wijst op een succesvolle uitvoering van een stap in de modellevenscyclus.
   * ![ Klok ](/help/assets/icons/Clock.svg) - wijst op een huidige aan de gang zijnde uitvoering van een stap in de modellevenscyclus.
   * ![ dicht ](/help/assets/icons/Close.svg) - wijst op een ontbroken uitvoering van een stap in de modellevenscyclus.

   | Status | Maken | Trein | Score | Nieuwe treinen | Opnieuw score |
   |---|:---:|:---:|:---:|:---:|:---:|
   | In uitvoering | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | | | | |
   | In uitvoering | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Klok ](/help/assets/icons/Clock.svg) | | | |
   | In uitvoering | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Klok ](/help/assets/icons/Clock.svg) | | |
   | In uitvoering | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Klok ](/help/assets/icons/Clock.svg) | |
   | In uitvoering | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Klok ](/help/assets/icons/Clock.svg) |
   | Training mislukt | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ dicht ](/help/assets/icons/Close.svg) | | | |
   | Training mislukt | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ dicht ](/help/assets/icons/Close.svg) | |
   | Training voltooid | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | | | |
   | Training voltooid | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | |
   | Scores mislukt | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ dicht ](/help/assets/icons/Close.svg) | | |
   | Scores mislukt | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ dicht ](/help/assets/icons/Close.svg) |
   | Scores gelukt | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | | |
   | Scores gelukt | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) | ![ Vinkje ](/help/assets/icons/Checkmark.svg) |

1. Om de kolommen te veranderen die voor de lijst worden getoond, selecteer ![ montages van de Kolom ](/help/assets/icons/ColumnSetting.svg) en knevel kolommen op ![ Controle ](/help/assets/icons/Checkmark.svg) of weg.

U kunt de volgende handelingen uitvoeren op een specifiek model.

### Modelinzichten

De functie voor inzicht in modellen is alleen beschikbaar voor goed opgeleide en gescoreerde modellen.

De inzichten van een model weergeven:

1. Selecteer ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer de modelnaam.

U wordt opnieuw gericht aan [ ModelInzichten ](insights.md).


### Details weergeven

Meer details van een model bekijken:

1. Selecteer ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer ![ Info ](/help/assets/icons/Info.svg) voor een model om pop-up met details te tonen.


### Dupliceren

U kunt snel een model dupliceren.

1. Selecteer ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer ![ Meer ](/help/assets/icons/More.svg) voor een model, en van het contextmenu uitgezocht **[!UICONTROL Duplicate]**.

U wordt opnieuw gericht aan de stappen om een nieuw model, met een voorgestelde naam tot stand te brengen die uit de originele die naam van het model wordt samengesteld met **[!UICONTROL (Copy)](_n_)** wordt toegevoegd.

### Bewerken

U kunt de naam, beschrijving en het plannen van opleiding en het noteren van een model uitgeven.

1. Selecteer ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer ![ Meer ](/help/assets/icons/More.svg) voor een model, en van het contextmenu uitgezocht **[!UICONTROL Edit]**.

   In het dialoogvenster **[!UICONTROL Edit model]** :

   * Voer een nieuwe **[!UICONTROL Name]** en **[!UICONTROL Description]** in.

   * Schakel **[!UICONTROL Status]** in om planning in te schakelen. U kunt het plannen voor modellen slechts toelaten die worden opgeleid en worden gescoord.

      1. Selecteer een **[!UICONTROL Scoring frequency]** :

         * **[!UICONTROL Daily]**: Ga een geldige tijd (bijvoorbeeld `05:22 pm`) in of gebruik ![ Klok ](/help/assets/icons/Clock.svg).
         * **[!UICONTROL Weekly]**: Selecteer een dag van de week en ga een geldige tijd (bijvoorbeeld `05:22 pm`) in of gebruik ![ Klok ](/help/assets/icons/Clock.svg).
         * **[!UICONTROL Monthly]**: Selecteer een dag van de maand van de Looppas op elk dropdown menu en ga een geldige tijd (bijvoorbeeld `05:22 pm`) in of gebruik ![ Klok ](/help/assets/icons/Clock.svg).

      1. Selecteer een **[!UICONTROL Training frequency]** in de vervolgkeuzelijst: **[!UICONTROL Monthly]** , **[!UICONTROL Quarterly]** , **[!UICONTROL Yearly]** of **[!UICONTROL None]** .

     ![ geef een model ](../assets/model-edit.png) uit

1. Selecteer **[!UICONTROL Save]** .



### Nieuwe treinen


Een model opnieuw trainen is alleen beschikbaar voor goed opgeleide modellen.

Overweeg een model opnieuw op te leiden wanneer u wilt:

* Nieuwe incrementele marketing en factorgegevens opnemen. In het laatste kwartaal is bijvoorbeeld de marktdynamiek veranderd of is de verspreiding van uw marketinggegevens aanzienlijk veranderd.

Een model opnieuw trainen:

1. Selecteer ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer ![ Meer ](/help/assets/icons/More.svg) voor een model, en van het contextmenu uitgezocht **[!UICONTROL Train]**. Alternatief, selecteer ![ DataRefresh ](/help/assets/icons/DataRefresh.svg) **[!UICONTROL Train]** van de blauwe actiebar.

   Selecteer in het dialoogvenster **[!UICONTROL Train model]** de optie die u wilt:

   * **[!UICONTROL Train model with last 2 years of marketing data]** , of
   * **[!UICONTROL Train model using specific date range of data]**.
Geef het datumbereik op. U kunt de ![ Kalender ](/help/assets/icons/Calendar.svg) gebruiken om een datumwaaier te selecteren. U moet een gegevensbereik selecteren met minimaal één jaar.

   ![ re-train een model ](../assets/re-train-model.png)

1. Selecteer **[!UICONTROL Train]** om het model opnieuw te trainen.


### Score of re-score


U kunt een model stapsgewijs score behalen op basis van nieuwe marketinggegevens of een model opnieuw scoren voor een specifieke datumreeks.

U kunt overwegen een model opnieuw te scoren als u wilt:

* Corrigeer onjuiste marketinggegevens. Zo hebben de recente betaalde zoekgegevens die u hebt opgenomen in de training en scoring van het model een week aan gegevens gemist.
* Gebruik nieuwe stijgende marketing gegevens die door updates in de datasets beschikbaar zijn geworden u als deel van uw geharmoniseerde gegevens hebt gevormd.

Een model scoren of opnieuw scoren:

1. Selecteer ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer ![ Meer ](/help/assets/icons/More.svg) voor een model, en van het contextmenu uitgezocht **[!UICONTROL Score]**. Alternatief, selecteer ![ DataRefresh ](/help/assets/icons/DataRefresh.svg) **[!UICONTROL Score]** van de blauwe actiebar.

   Selecteer in het dialoogvenster **[!UICONTROL Score marketing data]** de optie die u wilt:

   * **[!UICONTROL Score new marketing data from *mm/dd/yyyy *]**, om uw model incrementeel te behalen gebruikend nieuwe marketing gegevens, of
   * **[!UICONTROL Score specific date range of marketing data]** om opnieuw te scoren voor een bepaald datumbereik.
Geef het datumbereik op. U kunt de ![ Kalender ](/help/assets/icons/Calendar.svg) gebruiken om een datumwaaier te selecteren.

   ![ re-train een model ](../assets/re-score-model.png)

1. Selecteer **[!UICONTROL Score]** . Wanneer u een model opnieuw scant met een specifiek gegevensbereik, wordt een dialoogvenster **[!UICONTROL Existing model is replaced]** weergegeven waarin u wordt gevraagd te bevestigen dat u het model wilt vervangen door nieuwe scores voor het geselecteerde datumbereik. Selecteer **[!UICONTROL Replace model]** om te bevestigen.


### Modellen verwijderen

Een model verwijderen:

1. Selecteer ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.
1. Selecteer ![ Meer ](/help/assets/icons/More.svg) voor een model, en van het contextmenu uitgezocht **[!UICONTROL Delete]**. Alternatief, selecteer ![ Schrapping ](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** van de blauwe actiebar.
1. Selecteer **[!UICONTROL Delete]** in het bevestigingsdialoogvenster van **[!UICONTROL Delete model]** om het model te verwijderen. Selecteer **[!UICONTROL Cancel]** om te annuleren.

Meerdere modellen verwijderen:

1. Selecteer meerdere modellen.
1. Van de blauwe actiebar, uitgezochte ![ Schrapping ](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** om de modellen te schrappen.
1. Selecteer **[!UICONTROL Delete]** in de **[!UICONTROL Delete *x *modellen]**bevestigingsdialoog om de modellen te schrappen. Selecteer **[!UICONTROL Cancel]**om te annuleren.

