---
title: Train- en scoremodellen
description: Leer modellen op te leiden en te scoren.
feature: Models
source-git-commit: 6855d19347b7f6f1477a6265310df5950b8463c9
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# Train- en scoremodellen

Nadat u [ ](/help/models/build.md) een model hebt gebouwd, wordt het model automatisch getraind en gescoord. U kunt een model handmatig opnieuw trainen of opnieuw centreren.

## Trein

Overweeg een model opnieuw op te leiden wanneer u nieuwe incrementele marketing en factorgegevens wilt opnemen. In het laatste kwartaal is bijvoorbeeld de marktdynamiek veranderd of is de verspreiding van uw marketinggegevens aanzienlijk veranderd.

Een model omscholen:

1. Selecteer ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer ![ Meer ](/help/assets/icons/More.svg) voor een model, en van het contextmenu uitgezocht **[!UICONTROL Train]**. Alternatief, selecteer ![ DataRefresh ](/help/assets/icons/DataRefresh.svg) **[!UICONTROL Train]** van de blauwe actiebar.

   Selecteer in het dialoogvenster **[!UICONTROL Train model]** de optie die u wilt:

   * **[!UICONTROL Train model with last 2 years of marketing data]** , of
   * **[!UICONTROL Train model using specific date range of data]**.
Geef het datumbereik op. U kunt de ![ Kalender ](/help/assets/icons/Calendar.svg) gebruiken om een datumwaaier te selecteren. U moet een gegevensbereik selecteren met minimaal één jaar.

   ![ keert een model ](../assets/retrain-model.png) terug

1. Selecteer **[!UICONTROL Train]** om het model opnieuw te trainen.


U kunt een model alleen opnieuw trainen als het met succes is getraind.


## Score


U kunt een model incrementeel score behalen op basis van nieuwe marketinggegevens of een model opnieuw ordenen voor een specifieke datumreeks.

Denk na opnieuw te scoren een model wanneer u wilt:

* Corrigeer onjuiste marketinggegevens. Zo hebben de recente betaalde zoekgegevens die u hebt opgenomen in de training en scoring van het model een week aan gegevens gemist.
* Gebruik nieuwe stijgende marketing gegevens die door updates in de datasets beschikbaar zijn geworden u als deel van uw geharmoniseerde gegevens hebt gevormd.

Een model scoren of opnieuw centreren:

1. Selecteer ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer ![ Meer ](/help/assets/icons/More.svg) voor een model, en van het contextmenu uitgezocht **[!UICONTROL Score]**. Alternatief, selecteer ![ DataRefresh ](/help/assets/icons/DataRefresh.svg) **[!UICONTROL Score]** van de blauwe actiebar.

   Selecteer in het dialoogvenster **[!UICONTROL Score marketing data]** de optie die u wilt:

   * **[!UICONTROL Score new marketing data from *mm/dd/yyyy *]**, om uw model incrementeel te behalen gebruikend nieuwe marketing gegevens, of
   * **[!UICONTROL Score specific date range of marketing data]** om opnieuw te centreren voor een specifiek datumbereik.
Geef het datumbereik op. U kunt de ![ Kalender ](/help/assets/icons/Calendar.svg) gebruiken om een datumwaaier te selecteren.

   ![ Rescore a model ](../assets/rescore-model.png)

1. Selecteer **[!UICONTROL Score]** . Wanneer u een model opnieuw scant met een specifiek gegevensbereik, wordt een dialoogvenster **[!UICONTROL Existing model is replaced]** weergegeven waarin u wordt gevraagd te bevestigen dat u het model wilt vervangen door nieuwe scores voor het geselecteerde datumbereik. Selecteer **[!UICONTROL Replace model]** om te bevestigen.

>[!IMPORTANT]
>
>De recore van een model verandert geen Abonnementen die reeds gebaseerd op het opnieuw bestelde model worden gecreeerd. Om het nieuwe opnieuw begeleide model in een plan te gebruiken, moet u een nieuw plan tot stand brengen.

