---
title: Controlelogboeken
description: Leer hoe u controlelogboeken kunt openen vanuit Mix Modeler.
feature: Administration
exl-id: aa65aac5-bea4-43ff-b0d0-9e8a6a97d3ca
source-git-commit: 85f9b42a775006cd3566447b2bb9d0a806fa3e73
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 1%

---

# Controlelogboeken

Om de transparantie en zichtbaarheid van de activiteiten in het systeem te vergroten, wordt gebruikersactiviteit binnen de Mix Modeler-workflow vastgelegd in Experience Platform-auditlogboeken om te begrijpen welke door de gebruiker aangebrachte wijzigingen in de Mix Modeler-categorieën mogelijk zijn. Deze logboeken vormen een auditspoor dat met het oplossen van problemenkwesties kan helpen, en uw zaken kan helpen effectief aan het beleid van het collectieve gegevensbeheer en regelgevende vereisten voldoen.

<!-- DO WE HAVE TO ADD THIS
If you are subject to the Health Insurance Portability and Accountability Act (HIPAA) and create, receive, maintain, or transmit permitted sensitive personal data through Mix Modeler, you are responsible for executing a BAA with Adobe and licensing Healthcare Shield.
-->

Een controlelogboek deelt wie welke actie, en wanneer uitvoerde. Elke actie die in een logboek wordt geregistreerd bevat meta-gegevens die op het actietype, datum en tijd, e-mailidentiteitskaart van de gebruiker die de actie, en extra attributen relevant voor het actietype uitvoerde. Hiermee worden de acties bijgehouden die gebruikers in Mix Modeler hebben ondernomen om acties te maken, bij te werken en te verwijderen.

Om het controlelogboek te inspecteren, in de interface van Mix Modeler:

1. Selecteer ![ Lijst van de Taak ](/help/assets/icons/TaskList.svg) **[!UICONTROL Audits]** van **[!UICONTROL PRIVACY]**.

1. In **[!UICONTROL Audits]** vindt u de **[!UICONTROL Activity log]** . In het Activiteitenlogboek worden vermeldingen weergegeven voor de volgende categorieën, handelingen en status van Mix Modeler.

   | Categorie | Handeling | Status |
   |---|---|---|
   | Mix Modeler-regel voor gegevensset | Maken | Toestaan of Weigeren |
   | Mix Modeler-regel voor gegevensset | Bijwerken | Toestaan of Weigeren |
   | Mix Modeler-regel voor gegevensset | Verwijderen | Toestaan of Weigeren |
   | Mix Modeler-veld | Maken | Toestaan of Weigeren |
   | Mix Modeler-veld | Bijwerken | Toestaan of Weigeren |
   | Mix Modeler-veld | Verwijderen | Toestaan of Weigeren |
   | Mix Modeler Marketing TouchPoint | Maken | Toestaan of Weigeren |
   | Mix Modeler Marketing TouchPoint | Bijwerken | Toestaan of Weigeren |
   | Mix Modeler Marketing TouchPoint | Verwijderen | Toestaan of Weigeren |
   | Mix Modeler-conversie | Maken | Toestaan of Weigeren |
   | Mix Modeler-conversie | Bijwerken | Toestaan of Weigeren |
   | Mix Modeler-conversie | Verwijderen | Toestaan of Weigeren |
   | Mix Modeler-model | Maken | Toestaan of Weigeren |
   | Mix Modeler-model | Bijwerken | Toestaan of Weigeren |
   | Mix Modeler-model | Verwijderen | Toestaan of Weigeren |
   | Mix Modeler-model | Rescore | Toestaan of Weigeren |
   | Mix Modeler-model | Klonen | Toestaan of Weigeren |
   | Mix Modeler-model | Trein/Retrein | Toestaan of Weigeren |
   | Mix Modeler-model | Metagegevens downloaden/opslaan | Toestaan of Weigeren |
   | Mix Modeler-abonnement | Maken | Toestaan of Weigeren |
   | Mix Modeler-abonnement | Bijwerken | Toestaan of Weigeren |
   | Mix Modeler-abonnement | Gekoppeld model wijzigen | Toestaan of Weigeren |
   | Mix Modeler Data Harmonization | Synchronisatie activeren | Toestaan of Weigeren |


1. Selecteer een item in het activiteitenlog om een deelvenster voor meer informatie te openen.

   ![ de Controle van Mix Modeler ](/help/assets/mix-modeler-audit.png)

1. Om op **[!UICONTROL Category]**, **[!UICONTROL Action]**, **[!UICONTROL Request ID]**, **[!UICONTROL User]**, **[!UICONTROL Status]** of **[!UICONTROL Date]** waaier te filtreren, selecteer ![ Filter ](/help/assets/icons/Filter.svg).

1. Om de kolommen te wijzigen die in het logboek van de Activiteit worden getoond, selecteer ![ Kolommen ](/help/assets/icons/ColumnSetting.svg) en in de **[!UICONTROL Customize table]** dialoog selecteer de kolommen om te tonen. Selecteer **[!UICONTROL Apply]** om de selectie toe te passen, **[!UICONTROL Cancel]** om de selectie te annuleren.

1. Om het controlelogboek te downloaden, uitgezochte ![ Download ](/help/assets/icons/Download.svg) **[!UICONTROL Download log]**. Selecteer in het dialoogvenster **[!UICONTROL Download log]** de indeling **[!UICONTROL CSV]** of **[!UICONTROL JSON]** en selecteer **[!UICONTROL Download]** .

## Toegang tot auditlogboeken

Wanneer de eigenschap voor uw organisatie wordt toegelaten, worden de controlelogboeken automatisch verzameld aangezien de activiteit voorkomt. U te hoeven niet om de inzameling van het controlelogboek manueel toe te laten.

Om controlelogboeken te bekijken en uit te voeren, moet u de de toegangsbeheertoestemming van de Toegang van Logboeken van de Controle hebben gekregen. Leren hoe te om individuele toestemmingen voor de eigenschappen van Mix Modeler te beheren, zie de [ documentatie van de toegangscontrole ](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home).
