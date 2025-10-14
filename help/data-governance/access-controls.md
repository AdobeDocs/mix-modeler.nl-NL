---
title: Toegangsbesturingselementen
description: Leer hoe te om toegangscontroles in Mix Modeler te vormen.
feature: Administration
exl-id: c9ec97d9-b9a2-41f5-8626-1cf967d5d7fe
source-git-commit: 9a6c1f1c12ab29da80a1997cfd31ca07b38eaa22
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Toegangsbesturingselementen

De controle van de toegang voor Mix Modeler wordt verstrekt door Experience Platform in [&#x200B; Adobe Admin Console &#x200B;](https://adminconsole.adobe.com/) en door [&#x200B; Toestemmingen &#x200B;](https://experienceleague.adobe.com/nl/docs/experience-platform/access-control/home#platform-permissions) in Experience Platform. Deze functionaliteit gebruikt productprofielen in de Admin Console, die gebruikers met toestemmingen en zandbakken verbinden.

Voor meer informatie over toegangsbeheer, zie [&#x200B; het overzicht van de Toegangscontrole &#x200B;](https://experienceleague.adobe.com/nl/docs/experience-platform/access-control/home).

## Op rollen gebaseerd toegangsbeheer

Zie [&#x200B; Beleid &#x200B;](../main-guide/administration.md) op hoe te om op rol-gebaseerde toegangstoestemmingen voor Mix Modeler gebruikers en gebruikersgroepen in Experience Platform te vormen.

## Toegangsbeheer op basis van kenmerken

[&#x200B; op attributen-Gebaseerd toegangsbeheer &#x200B;](https://experienceleague.adobe.com/nl/docs/experience-platform/access-control/abac/overview) is een vermogen van Experience Platform dat beheerders toelaat om toegang tot specifieke voorwerpen en/of mogelijkheden te controleren die op attributen worden gebaseerd. Kenmerken kunnen metagegevens zijn die aan een object worden toegevoegd, zoals een label dat aan een schemaveld of -segment wordt toegevoegd. Een beheerder bepaalt toegangsbeleid dat attributen omvat om de toestemmingen van de gebruikerstoegang te beheren.

Met deze functionaliteit kunt u XDM-schemavelden (Experience Data Model) labelen met labels die bereik voor organisatie of gegevensgebruik definiëren. Parallel hieraan kunnen beheerders de gebruikers- en rolinebeheerinterface gebruiken om het toegangsbeleid voor XDM-schemavelden te definiëren. En beheer beter de toegang die aan gebruikers of groepen gebruikers (interne, externe, of derdegebruikers) wordt gegeven. Bovendien, op attribuut-gebaseerde toegangsbeheer staat beheerders toe om toegang tot specifieke segmenten te beheren.

Via op kenmerken gebaseerde toegangscontrole kunnen beheerders de toegang van gebruikers tot zowel gevoelige persoonlijke gegevens (SPD) als persoonlijk identificeerbare informatie (PII) in alle workflows en bronnen van het Platform beheren. Beheerders kunnen gebruikersrollen definiëren die alleen toegang hebben tot specifieke velden en gegevens die overeenkomen met die velden.

Wanneer het vormen van datasetregels voor geharmoniseerde datasets, wordt de attributen van het Experience Platform [&#x200B; gebaseerd toegangsbeheer &#x200B;](https://experienceleague.adobe.com/nl/docs/experience-platform/access-control/abac/overview) afgedwongen op een gebied-niveau. Een veld is beperkt wanneer een label is gekoppeld aan een schemaveld. En een actief beleid wordt toegelaten dat toegang voor u tot dat gebied ontkent. Dientengevolge:

* u ziet niet de schemagebieden die voor u beperkt zijn wanneer u een datasetregel creeert,
* u kunt de afbeelding van een of meer schemavelden die voor u zijn beperkt, niet weergeven of bewerken. Wanneer u een datasetregel uitgeeft of bekijkt die dergelijke beperkte gebieden bevat, ziet u het volgende scherm.
  ![&#x200B; Actie niet toegestaan &#x200B;](/help/assets/action-not-permitted.png)
