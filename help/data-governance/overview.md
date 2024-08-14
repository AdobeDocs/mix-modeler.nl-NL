---
title: Gegevensbeheer
description: Leer hoe u de services en tools van Experience Platform gebruikt waarmee u de verzamelde ervaringsgegevens kunt beheren. Zo, volgt u uw bedrijfspraktijken, wettelijke verplichtingen, en ontwikkelingsproces.
feature: Administration
source-git-commit: 6776a91563f120db1341adef923aab4b0f582c9d
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Gegevensbeheer

De integratie tussen Mix Modeler en Experience Platform biedt Mix Modeler de mogelijkheden om de intrinsieke functies voor gegevensbeheer van Experience Platform te benutten. In dit gedeelte van de documentatie worden de specifieke kenmerken van de functies voor gegevensbeheer in de Mix Modeler beschreven.

Het Beheer van Gegevens van het Experience Platform geeft u de capaciteit om uw gegevens door de reis te controleren en te begrijpen die de gegevens door Experience Platform nemen. Deze reis impliceert het handhaven van gegevenskwaliteit, gegevensverbinding, gegevenscatalogisering, en veel meer.

De etiketten en het beleid van het gegevensgebruik die op datasets worden gecreeerd die door de oppervlakte van de Experience Platform in de Mix Modeler waar nodig worden verbruikt. Bijvoorbeeld, stoppen deze etiketten of waarschuwen gebruikers wanneer het schrappen van datasets die deel van een datasetregel in de geharmoniseerde gegevens uitmaken. Of verberg schemagebieden die voor gebruikers wanneer het creëren van een datasetregel worden beperkt.

Dankzij de integratie van gegevensbeheer kunt u de naleving efficiënter beheren. Gegevensstewards in uw organisatie kunnen beleid plaatsen om gebruik te beperken. Dientengevolge, kunt u gegevens gebruiken die met beleid in plaats van gegevens worden bepaald in overeenstemming zijn. Lees de documentatie over [ Etiketten en Beleid ](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-dataviews/data-governance) om meer te leren.

De volgende functies voor gegevensbeheer zijn beschikbaar:

| Functie | Details |
|---|---|
| Toegangsbesturingselementen | Op rollen gebaseerd toegangsbeheer en op attribuut-gebaseerd (gebied-niveau) toegangsbeheer worden gesteund. Zie [ controles van de Toegang ](access-controls.md) voor meer informatie. |
| Controlelogboeken | Wanneer de gebruikers creëren, bijwerken of schrappen specifieke categorieën van de Mix Modeler, registreert de functionaliteit van de Controle van het Experience Platform de activiteit in de controlelogboeken. Zie [ Logboeken van de Controle ](audit-logs.md) voor meer informatie. |
| Beleid | In het kader van de geharmoniseerde gegevenswerkstroom worden door Experience Platforms gedefinieerde beleidsregels afgedwongen. Elke schending van labels voor gegevensgebruik wordt gemeld en aan de gebruiker weergegeven. Zie [ Beleid ](policies.md) voor meer informatie. |
| Versleuteling | Alle datasets die voor input en output van modellen worden gebruikt volgen de richtlijnen van het Experience Platform. De gegevensencryptie van het Experience Platform is van toepassing op gegevens in rust en in-transit. |
| Gegevenshygiëne | Alle datasets die voor input en uit modellen worden gebruikt volgen de richtlijnen van het Experience Platform. Experience Platform biedt een reeks hulpmiddelen om de levenscyclus van klantgegevens te beheren, met inbegrip van de steun van verschillende types van gegevensvervalsing. Wanneer u een brondataset van Experience Platform schrapt, die als deel van uw geharmoniseerde gegevens wordt gebruikt, wordt u op de hoogte gebracht. Zie [ regels van de Dataset ](/help/harmonize-data/dataset-rules.md) voor meer informatie. |
| Door de klant beheerde toetsen | Wanneer u een licentie hebt verkregen voor Mix Modeler met het privacybeveiligingsschild of de invoegtoepassing voor het privacyschild, kunt u de mogelijkheid voor door de klant beheerde sleutels gebruiken om Azure Key Vault te gebruiken om uw eigen sleutels via API&#39;s in te voeren. U hebt volledig beheer van gegevens die binnen modellen in Mix Modeler worden verwerkt. |
