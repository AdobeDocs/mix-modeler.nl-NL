---
title: Modellen
description: Leer hoe te om modellen in Mix Modeler te vormen en te gebruiken.
feature: Models
exl-id: c43d9bc9-4429-45c2-9247-bd24510a24be
source-git-commit: 9085363e951a4e306c64ad28f56e2c15b4a6029a
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Modellen

De modelfunctionaliteit in Mix Modeler staat u toe om, AI/ML modellen te vormen op te leiden en te scoren specifiek voor uw bedrijfsdoelstellingen en gesteund door AI-gedreven overdrachtsstudie tussen multitouch attributie en marketing mixmodellering.

De modellen zijn gebaseerd op de geharmoniseerde gegevens die u maakt als onderdeel van de workflow van de Mix Modeler-toepassing.

Een model in de Mix Modeler is een model voor machinaal leren dat wordt gebruikt om een bepaald resultaat te meten en/of te voorspellen op basis van de investeringen van een marketeter. Marketing-aanraakpunten en gegevens op overzichtsniveau kunnen als invoer worden gebruikt. Met Mix Modeler kunt u varianten van modellen maken op basis van verschillende sets variabelen, dimensies en resultaten, zoals inkomsten, verkochte eenheden en leads.

Een model vereist:

* één conversie,
* een of meer marketingaanraakpunten (kanalen) bestaande uit gegevens op overzichtsniveau, marketingaanraakpuntgegevens (gebeurtenisgegevens) of beide;
* een configureerbaar terugzoekvenster voor
* een configureerbaar trainingsvenster.

Een model kan eventueel het volgende omvatten:

* externe factoren,
* interne factoren,
* zogenaamde &#39;priors&#39; (kansverdeling die kennis of onzekerheid van gegevens vóór of vóór de waarneming van die gegevens weergeeft), die eerdere omzettingen via het kanaal indexeert;
* geeft aandeel uit, dat relatief uitgeeft aandeel als volmacht gebruikt wanneer de marketing gegevens schaars is.


## Een model maken

Als u een model wilt maken, gebruikt u de stapsgewijze configuratiestroom met instructies van de Mix Modeler die beschikbaar is wanneer u **[!UICONTROL Open model canvas]**. Zie [Een model maken](create.md) voor meer informatie .

## Modellen beheren

Om een lijst van uw huidige modellen, in de interface van de Mix Modeler te bekijken:

1. Selecteren ![](/help/assets//icons/FileData.svg) **[!UICONTROL Models]** van de linkerspoorstaaf.

1. U ziet een tabel met de huidige modellen.

   De tabelkolommen geven details over het model op.

   | Kolomnaam | Details |
   |---|---|
   | Naam | Naam van het model |
   | Beschrijving | Beschrijving van het model |
   | Conversion-gebeurtenis | De conversie die u voor het model hebt geselecteerd. |
   | Uitvoerfrequentie | De lopende frequentie van opleiding het model. |
   | Laatste uitvoering | De datum en het tijdstip van de laatste training voor het model. |
   | Status | De status van de laatste run van de training van het model. <br/><span style="color:green">●</span> Succes<br/><span style="color:orange">●</span> Trainingsprobleem<br/> <span style="color:orange">●</span> In afwachting van training <br/><span style="color:red">●</span> Mislukt <br/><span style="color:gray">●</span> _ (wanneer een laatste run wordt uitgevoerd) |

   {style="table-layout:auto"}

1. Als u de kolommen voor de lijst wilt wijzigen, selecteert u ![Kolominstellingen](/help/assets//icons/ColumnSetting.svg) en kolommen in-/uitschakelen ![Controleren](/help/assets//icons/Checkmark.svg) of uit.


### Details van een model weergeven

Meer details van een model bekijken:

1. Selecteren ![Info](/help/assets//icons/Info.svg) voor een model om een pop-up met details te tonen.



### Modelinzichten

Om inzichten van een model, in de interface van de Mix Modeler te bekijken:

1. Selecteren ![](/help/assets//icons/FileData.svg) **[!UICONTROL Models]** van de linkerspoorstaaf.

1. Selecteer de naam van een model met een **[!UICONTROL Last run status]** van <span style="color:green">●</span> **[!UICONTROL Success]** van de **[!UICONTROL Models]** tabel. Modelinzichten zijn alleen beschikbaar voor goed opgeleide modellen.

1. Selecteer in het contextmenu de optie **[!UICONTROL Model Insights]**. U wordt omgeleid naar [Modelinzichten](insights.md).


### Opnieuw score


Om een model, in de interface van de Mix Modeler opnieuw te scoren:

1. Selecteren ![](/help/assets//icons/FileData.svg) **[!UICONTROL Models]** van de linkerspoorstaaf.

1. Selecteer de naam van een model met een **[!UICONTROL Last run status]** van <span style="color:green">●</span> **[!UICONTROL Success]** van de **[!UICONTROL Models]** tabel. Herscore is alleen beschikbaar voor goed opgeleide modellen.

1. Selecteer in het contextmenu de optie **[!UICONTROL Re-score]**. Het kan een paar minuten duren om een bijgewerkte status voor het model weer te geven.


### Een model verwijderen

Een model verwijderen:

1. Selecteer de naam van het model dat u wilt verwijderen.

1. Selecteer in het contextmenu de optie **[!UICONTROL Delete]** om het model te verwijderen.

   >[!WARNING]
   >
   >Het model wordt onmiddellijk verwijderd.


