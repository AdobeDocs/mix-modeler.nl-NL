---
title: Modellen
description: Leer hoe te om modellen in Mix Modeler te vormen en te gebruiken.
feature: Models
exl-id: c43d9bc9-4429-45c2-9247-bd24510a24be
source-git-commit: d5d9ec6b7b1222b3da9dcecaf3fa1cf2b2198881
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 0%

---

# Modellen

De modelfunctionaliteit in Mix Modeler staat u toe om, modellen te vormen op te leiden en te scoren AI/ML specifiek voor uw bedrijfsdoelstellingen. De training en scoring ondersteunen het leren van overdracht via AI tussen multitouch-attributie en marketingmixmodellering.

De modellen zijn gebaseerd op de geharmoniseerde gegevens die u maakt als onderdeel van de workflow van de Mix Modeler-toepassing.

Een model in de Mix Modeler is een model voor machinaal leren dat wordt gebruikt om een bepaald resultaat te meten en/of te voorspellen op basis van de investeringen van een marketeter. Marketing-aanraakpunten en gegevens op overzichtsniveau kunnen als invoer worden gebruikt. Met Mix Modeler kunt u varianten van modellen maken op basis van verschillende sets variabelen, dimensies en resultaten, zoals inkomsten, verkochte eenheden en leads.

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


## Een model maken

Als u een model wilt maken, gebruikt u de stapsgewijze configuratiestroom met instructies van de Mix Modeler die beschikbaar is wanneer u **[!UICONTROL Open model canvas]** selecteert. Zie [ een model ](create.md) voor meer details creëren.

## Modellen beheren

Om een lijst van uw huidige modellen, in de interface van de Mix Modeler te bekijken:

1. Selecteer ![](/help/assets//icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. U ziet een tabel met de huidige modellen.

   De tabelkolommen geven details over het model op.

   | Kolomnaam | Details |
   |---|---|
   | Naam | Naam van het model |
   | Beschrijving | Beschrijving van het model |
   | Conversion-gebeurtenis | De conversie die u voor het model hebt geselecteerd. |
   | Uitvoerfrequentie | De lopende frequentie van opleiding het model. |
   | Laatste uitvoering | De datum en het tijdstip van de laatste training voor het model. |
   | Status | De status van de laatste run van de training van het model. <br/>![ StatusGreen ](/help/assets/icons/StatusGreen.svg) De kwestie van de Opleiding <br/>![ StatusOrange ](/help/assets/icons/StatusOrange.svg) <br/> ![ StatusOrange ](/help/assets/icons/StatusOrange.svg) wachtend opleiding <br/>![ StatusRed ](/help/assets/icons/StatusRed.svg) Mislukte <br/>![ StatusGreen ](/help/assets/icons/StatusGray.svg) _ (wanneer laatste looppas lopend is) |

   {style="table-layout:auto"}

1. Om de kolommen te veranderen die voor de lijst worden getoond, selecteer ![ montages van de Kolom ](/help/assets//icons/ColumnSetting.svg) en knevel kolommen op ![ Controle ](/help/assets//icons/Checkmark.svg) of weg.

U kunt de volgende handelingen uitvoeren op een specifiek model.

### Details weergeven

Meer details van een model bekijken:

1. Selecteer ![](/help/assets//icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer ![ Info ](/help/assets//icons/Info.svg) voor een model om pop-up met details te tonen.



### Dupliceren

U kunt snel een model dupliceren.

1. Selecteer ![](/help/assets//icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer ![ Meer ](/help/assets/icons/More.svg) voor een model, en van het contextmenu uitgezocht **[!UICONTROL Duplicate]**.


### Modelinzichten

De functie voor inzicht in modellen is alleen beschikbaar voor goed opgeleide en gescoreerde modellen. De inzichten van een model weergeven:

1. Selecteer ![](/help/assets//icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer de modelnaam.

U wordt opnieuw gericht aan [ ModelInzichten ](insights.md).


### Nieuwe treinen

Een model opnieuw trainen is alleen beschikbaar voor goed opgeleide modellen. Een model opnieuw trainen:

1. Selecteer ![](/help/assets//icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer ![ Meer ](/help/assets/icons/More.svg) voor een model, en van het contextmenu uitgezocht **[!UICONTROL Train]**. Alternatief, selecteer ![ DataRefresh ](/help/assets/icons/DataRefresh.svg) **[!UICONTROL Train]** van de blauwe actiebar.

   Selecteer in het dialoogvenster **[!UICONTROL Train model]** de optie die u wilt:

   * **[!UICONTROL Train model with last 2 years of marketing data]** , of
   * **[!UICONTROL Train model using specific date range of data]**.
Geef het datumbereik op. U kunt de ![ Kalender ](/help/assets/icons/Calendar.svg) gebruiken om een datumwaaier te selecteren. U moet een gegevensbereik selecteren met minimaal één jaar.

   ![ re-train een model ](../assets/re-train-model.png)

1. Selecteer **[!UICONTROL Train]** om het model opnieuw te trainen.


### Score of re-score


U kunt een model stapsgewijs score behalen op basis van nieuwe marketinggegevens of een model opnieuw scoren voor een specifieke datumreeks. Een model scoren of opnieuw scoren:

1. Selecteer ![](/help/assets//icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer ![ Meer ](/help/assets/icons/More.svg) voor een model, en van het contextmenu uitgezocht **[!UICONTROL Score]**. Alternatief, selecteer ![ DataRefresh ](/help/assets/icons/DataRefresh.svg) **[!UICONTROL Score]** van de blauwe actiebar.

   Selecteer in het dialoogvenster **[!UICONTROL Score marketing data]** de optie die u wilt:

   * **[!UICONTROL Score new marketing data from *mm/dd/yyyy *]**, om uw model incrementeel te behalen gebruikend nieuwe marketing gegevens, of
   * **[!UICONTROL Score specific date range of marketing data]** om opnieuw te scoren voor een bepaald datumbereik.
Geef het datumbereik op. U kunt de ![ Kalender ](/help/assets/icons/Calendar.svg) gebruiken om een datumwaaier te selecteren.

   ![ re-train een model ](../assets/re-score-model.png)

1. Selecteer **[!UICONTROL Score]** . Wanneer u een model opnieuw scant met een specifiek gegevensbereik, wordt een dialoogvenster **[!UICONTROL Existing model is replaced]** weergegeven waarin u wordt gevraagd te bevestigen dat u het model wilt vervangen door nieuwe scores voor het geselecteerde datumbereik. Selecteer **[!UICONTROL Replace model]** om te bevestigen.


### Een model verwijderen

Een model verwijderen:

1. Selecteer ![](/help/assets//icons/FileData.svg) **[!UICONTROL Models]** in het linkerspoor.

1. Selecteer ![ Meer ](/help/assets/icons/More.svg) voor een model, en van het contextmenu uitgezocht **[!UICONTROL Delete]**. Alternatief, selecteer ![ Schrapping ](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** van de blauwe actiebar.

Meerdere modellen verwijderen:

1. Selecteer meerdere modellen.

1. Van de blauwe actiebar, uitgezochte ![ Schrapping ](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** om de modellen te schrappen.

   >[!WARNING]
   >
   >Het model wordt onmiddellijk verwijderd.


