---
title: Overzicht van gegevensbeheer
description: Leer hoe u de services en tools van Experience Platform gebruikt waarmee u uw verzamelde ervaringsgegevens kunt beheren. Zo, volgt u uw bedrijfspraktijken, wettelijke verplichtingen, en ontwikkelingsproces.
feature: Administration
exl-id: 87407c29-e158-48bf-bde9-b3c16a16107e
source-git-commit: bdde574b150bda2b0c82a9f5a20160fed26cb69d
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Overzicht van gegevensbeheer

De integratie tussen Mix Modeler en Experience Platform biedt Mix Modeler de mogelijkheden om de intrinsieke functies voor gegevensbeheer van Experience Platform te benutten. In dit gedeelte van de documentatie worden de specifieke kenmerken van de functies voor gegevensbeheer in Mix Modeler beschreven.

Met Experience Platform Data Governance hebt u de mogelijkheid om uw gegevens te beheren en te begrijpen tijdens de reis die de gegevens door Experience Platform maken. Deze reis impliceert het handhaven van gegevenskwaliteit, gegevensverbinding, gegevenscatalogisering, en veel meer.

De etiketten en het beleid van het gegevensgebruik die op datasets worden gecreeerd die door het oppervlak van Experience Platform in Mix Modeler waar nodig worden verbruikt. Bijvoorbeeld, stoppen deze etiketten of waarschuwen gebruikers wanneer het schrappen van datasets die deel van een datasetregel in de geharmoniseerde gegevens uitmaken. Of verberg schemagebieden die voor gebruikers wanneer het creëren van een datasetregel worden beperkt.

Dankzij de integratie van gegevensbeheer kunt u de naleving efficiënter beheren. Gegevensstewards in uw organisatie kunnen beleid plaatsen om gebruik te beperken. Dientengevolge, kunt u gegevens gebruiken die met beleid in plaats van gegevens worden bepaald in overeenstemming zijn. Lees de documentatie over [&#x200B; Etiketten en Beleid &#x200B;](https://experienceleague.adobe.com/nl/docs/analytics-platform/using/cja-dataviews/data-governance) om meer te leren.

De volgende functies voor gegevensbeheer zijn beschikbaar:

| Functie | Details |
|---|---|
| Toegangsbesturingselementen | Op rollen gebaseerd toegangsbeheer en op attribuut-gebaseerd (gebied-niveau) toegangsbeheer worden gesteund. Zie [&#x200B; controles van de Toegang &#x200B;](access-controls.md) voor meer informatie. |
| Controlelogboeken | Wanneer gebruikers specifieke categorieën van Mix Modeler maken, bijwerken of verwijderen, registreert de functie van de Controle van Experience Platform de activiteit in de controlelogboeken. Zie [&#x200B; Logboeken van de Controle &#x200B;](audit-logs.md) voor meer informatie. |
| Beleid | In het kader van de geharmoniseerde gegevensworkflow worden door Experience Platform gedefinieerde beleidsregels afgedwongen. Elke schending van labels voor gegevensgebruik wordt gemeld en aan de gebruiker weergegeven. Zie [&#x200B; Beleid &#x200B;](policies.md) voor meer informatie. |
| Versleuteling | Alle gegevenssets die worden gebruikt voor de invoer en uitvoer van modellen, voldoen aan de Experience Platform-richtlijnen. Experience Platform-gegevenscodering is van toepassing op gegevens in rust en in doorvoer. |
| Gegevenshygiëne | Alle gegevenssets die voor invoer en uitvoer van modellen worden gebruikt, voldoen aan de Experience Platform-richtlijnen. Experience Platform biedt een reeks tools voor het beheer van de levenscyclus van klantgegevens, waaronder de ondersteuning voor verschillende soorten gegevensvervaldatums. Wanneer u een brondataset van Experience Platform schrapt, die als deel van uw geharmoniseerde gegevens wordt gebruikt, wordt u op de hoogte gebracht. Zie [&#x200B; regels van de Dataset &#x200B;](/help/harmonize-data/dataset-rules.md) voor meer informatie. |
| Door de klant beheerde toetsen | Als u Mix Modeler een licentie hebt verleend met de Add-on Privacy Security Shield, kunt u de mogelijkheid van Keys voor door klanten beheerde sleutels gebruiken om Azure Key Vault te gebruiken om uw eigen sleutels via API&#39;s te plaatsen. U hebt een volledig beheer van de gegevens die in Mix Modeler worden verwerkt. |
