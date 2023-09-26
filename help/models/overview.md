---
title: Modellen
description: Leer hoe te om modellen in de Modelleur van de Adobe te vormen en te gebruiken.
feature: Models
source-git-commit: ac17f5a9fcf036c8e689879578e4b745b789cea3
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---


# Modellen

De modelfunctionaliteit in de Modelleur van de Mengeling van de Adobe staat u toe om, AI/ML modellen te vormen op te leiden en te scoren specifiek voor uw bedrijfsdoelstellingen en gesteund door AI-gedreven overdrachtsstudie tussen multitouch attributie en marketing mixmodellering.

De modellen zijn gebaseerd op de geharmoniseerde gegevens die u maakt als onderdeel van de toepassingsworkflow van de Adobe Mix Modeler.

Om een model tot stand te brengen, gebruik de reeks-door-stap geleide modelconfiguratiestroom van het Modelmodel van de Mengeling beschikbaar wanneer u selecteert **[!UICONTROL Guide me]**. Zie [Een model maken](create.md) voor meer informatie .

## Modellen beheren

Om een lijst van uw huidige modellen, in de interface van de Modelleur van de Adobe te bekijken:

1. Selecteren ![](../assets/icons/FileData.svg) **[!UICONTROL Models]** van de linkerspoorstaaf.

1. U ziet een tabel met de huidige modellen.

   De tabelkolommen geven details over het model op.

   | Kolomnaam | Details |
   |---|---|
   | Naam | Naam van het model |
   | Beschrijving | Beschrijving van het model |
   | Conversiegebeurtenissen | De conversie die u voor het model hebt geselecteerd. |
   | Gegevensset | De dataset die het model gebruikt om te trainen en te scoren. Dit is standaard de geharmoniseerde gegevensset. |
   | Uitvoerfrequentie | De lopende frequentie van opleiding het model. |
   | Laatste uitvoering | De datum en het tijdstip van de laatste training voor het model. |
   | Status van laatste uitvoering | De status van de laatste run van de training van het model. <br/><span style="color:green">●</span> Succes<br/><span style="color:orange">●</span> Trainingsprobleem<br/> <span style="color:orange">●</span> In afwachting van training <br/><span style="color:red">●</span> Mislukt |

   {style="table-layout:auto"}

1. Als u de kolommen voor de lijst wilt wijzigen, selecteert u ![Kolominstellingen](../assets/icons/ColumnSetting.svg) en kolommen in-/uitschakelen ![Controleren](../assets/icons/Checkmark.svg) of uit.

### Een model verwijderen

Een model verwijderen:

1. Selecteer de naam van het model dat u wilt verwijderen.

1. Selecteer in het contextmenu de optie **[!UICONTROL Delete]** om het model te verwijderen.

### Details van een model weergeven

Meer details van een model bekijken:

1. Selecteer de naam van het model waarvan u meer details wilt bekijken.

1. Selecteer in het contextmenu de optie **[!UICONTROL More]**. U ziet details van het geselecteerde model in de juiste ruit.



### Modelinzichten

>[!NOTE]
>
>Deze selectie is alleen beschikbaar voor geslaagde getrainde modellen (modellen met de status Laatste uitvoering als geslaagd).
>

Om inzichten van een model, in de interface van de Modelleur van de Adobe te bekijken:

1. Selecteren ![](../assets/icons/FileData.svg) **[!UICONTROL Models]** van de linkerspoorstaaf.

1. Selecteer de naam van een model met een **[!UICONTROL Last run status]** van <span style="color:green">●</span> **[!UICONTROL Success]** van de **[!UICONTROL Models]** table

1. Selecteer in het contextmenu de optie **[!UICONTROL Model Insights]**. U wordt omgeleid naar [Modelinzichten](insights.md).


