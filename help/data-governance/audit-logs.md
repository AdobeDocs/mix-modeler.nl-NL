---
title: Controlelogboeken
description: Leer hoe te om tot controlelogboeken van Mix Modeler toegang te hebben.
feature: Administration
exl-id: aa65aac5-bea4-43ff-b0d0-9e8a6a97d3ca
source-git-commit: 77a338ae568c854b99069b849a18661d413c501c
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---

# Controlelogboeken

Om de transparantie en de zichtbaarheid van activiteiten die in het systeem worden uitgevoerd te vergroten, wordt gebruikersactiviteit binnen de workflow van de Mix Modeler vastgelegd in de auditlogboeken van het Experience Platform om te begrijpen welke gebruikersgestuurde wijzigingen in de categorieën Mixxen Modeler worden doorgevoerd. Deze logboeken vormen een auditspoor dat met het oplossen van problemenkwesties kan helpen, en uw zaken kan helpen effectief aan het beleid van het collectieve gegevensbeheer en regelgevende vereisten voldoen.

<!-- DO WE HAVE TO ADD THIS
If you are subject to the Health Insurance Portability and Accountability Act (HIPAA) and create, receive, maintain, or transmit permitted sensitive personal data through Mix Modeler, you are responsible for executing a BAA with Adobe and licensing Healthcare Shield.
-->

Een controlelogboek deelt wie welke actie, en wanneer uitvoerde. Elke actie die in een logboek wordt geregistreerd bevat meta-gegevens die op het actietype, datum en tijd, e-mailidentiteitskaart van de gebruiker die de actie, en extra attributen relevant voor het actietype uitvoerde. Hiermee worden handelingen bijgehouden die gebruikers in de Mix Modeler hebben gemaakt, bijgewerkt en verwijderd.

Om het controlelogboek, in de interface van de Mix Modeler te inspecteren:

1. Selecteer ![ Lijst van de Taak ](/help/assets/icons/TaskList.svg) **[!UICONTROL Audits]** van **[!UICONTROL PRIVACY]**.

1. In **[!UICONTROL Audits]** vindt u de **[!UICONTROL Activity log]** . In het activiteitenlogboek worden vermeldingen weergegeven voor de volgende categorieën, handelingen en status van Mixxen Modeler.

   | Categorie | Handeling | Status |
   |---|---|---|
   | Gegevensregel Mix Modeler | Maken | Toestaan of Weigeren |
   | Gegevensregel Mix Modeler | Bijwerken | Toestaan of Weigeren |
   | Gegevensregel Mix Modeler | Verwijderen | Toestaan of Weigeren |
   | Veld Mix Modeler | Maken | Toestaan of Weigeren |
   | Veld Mix Modeler | Bijwerken | Toestaan of Weigeren |
   | Veld Mix Modeler | Verwijderen | Toestaan of Weigeren |
   | Aanraakpunt voor marketingMix Modeler | Maken | Toestaan of Weigeren |
   | Aanraakpunt voor marketingMix Modeler | Bijwerken | Toestaan of Weigeren |
   | Aanraakpunt voor marketingMix Modeler | Verwijderen | Toestaan of Weigeren |
   | Mix Modeler converteren | Maken | Toestaan of Weigeren |
   | Mix Modeler converteren | Bijwerken | Toestaan of Weigeren |
   | Mix Modeler converteren | Verwijderen | Toestaan of Weigeren |
   | Model Mix Modeler | Maken | Toestaan of Weigeren |
   | Model Mix Modeler | Bijwerken | Toestaan of Weigeren |
   | Model Mix Modeler | Verwijderen | Toestaan of Weigeren |
   | Model Mix Modeler | Opnieuw score | Toestaan of Weigeren |
   | Model Mix Modeler | Klonen | Toestaan of Weigeren |
   | Model Mix Modeler | Trein/herinrichting | Toestaan of Weigeren |
   | Model Mix Modeler | Metagegevens downloaden/opslaan | Toestaan of Weigeren |
   | Mix Modeler Plan | Maken | Toestaan of Weigeren |
   | Mix Modeler Plan | Bijwerken | Toestaan of Weigeren |
   | Mix Modeler Plan | Gekoppeld model wijzigen | Toestaan of Weigeren |
   | Harmonisatie van gegevens Mix Modeler | Synchronisatie activeren | Toestaan of Weigeren |


1. Selecteer een item in het activiteitenlog om een deelvenster voor meer informatie te openen.

   ![ Controle van de Mix Modeler ](/help/assets/mix-modeler-audit.png)

1. Om op **[!UICONTROL Category]**, **[!UICONTROL Action]**, **[!UICONTROL Request ID]**, **[!UICONTROL User]**, **[!UICONTROL Status]** of **[!UICONTROL Date]** waaier te filtreren, selecteer ![ Filter ](/help/assets/icons/Filter.svg).

1. Om de kolommen te wijzigen die in het logboek van de Activiteit worden getoond, selecteer ![ Kolommen ](/help/assets/icons/ColumnSetting.svg) en in de **[!UICONTROL Customize table]** dialoog selecteer de kolommen om te tonen. Selecteer **[!UICONTROL Apply]** om de selectie toe te passen, **[!UICONTROL Cancel]** om de selectie te annuleren.

1. Om het controlelogboek te downloaden, uitgezochte ![ Download ](/help/assets/icons/Download.svg) **[!UICONTROL Download log]**. Selecteer in het dialoogvenster **[!UICONTROL Download log]** de indeling **[!UICONTROL CSV]** of **[!UICONTROL JSON]** en selecteer **[!UICONTROL Download]** .

## Toegang tot auditlogboeken

Wanneer de eigenschap voor uw organisatie wordt toegelaten, worden de controlelogboeken automatisch verzameld aangezien de activiteit voorkomt. U te hoeven niet om de inzameling van het controlelogboek manueel toe te laten.

Om controlelogboeken te bekijken en uit te voeren, moet u de de toegangsbeheertoestemming van de Toegang van Logboeken van de Controle hebben gekregen. Leren hoe te om individuele toestemmingen voor de eigenschappen van de Mix Modeler te beheren, zie de [ documentatie van de toegangscontrole ](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home).
