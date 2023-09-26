---
title: Schema's
description: Leer hoe te om de schema's te beheren die worden vereist om gegevens in te voeren in de Modelleur van de Adobe.
feature: Datasets
source-git-commit: abbfc78e9fa774a240d000131f35d3dc257c15ea
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 1%

---


# Schema&#39;s

Om schema&#39;s te beheren, ondersteunend de gegevens u in Adobe Experience Platform en gebruik in de Modelleur van de Adobe wilt opnemen:

1. Ga naar de interface van de Modelleur van de Adobe Mix.

1. Selecteren ![Schemas](../assets/icons/Schemas.svg) **[!UICONTROL Schemas]**, onder **[!UICONTROL DATA MANAGEMENT]**.

Zie de [Overzicht van de interface Schemas](https://experienceleague.adobe.com/docs/experience-platform/xdm/ui/overview.html?lang=en) voor meer informatie .

## Samengevoegde of samenvattingsgegevens

Het wordt hoogst geadviseerd om de klasse van Metriek van de Samenvatting XDM als basis van het schema te gebruiken onderliggende om het even welk aggregaat of samenvattingsgegevens u in Experience Platform en gebruik in de Modelleur van de Mengeling van de Adobe wilt opnemen.

Zie hieronder voor een voorbeeld van een **[!DNL LumaPaidMarketingSchema]** de XDM Summary Metrics gebruiken als de basisklasse en speciale veldgroepen (met kleuren aangeduid) voor metrisch (**[!DNL AMMMetrics]**), afmetingen (**[!DNL AMMDimensions]**) en andere klantspecifieke informatie (**[!DNL CustomerSpecific]**).

![Samenvattingsschema](../assets/summary-schema.png)

Om een reeks controle eigenschappen te bepalen, wordt het sterk aangemoedigd om de Externe het gebiedsgroep van de Details van de Controle van het Bronsysteem te gebruiken, als deel van een schema dat voor het verzamelen van geaggregeerde of samenvattende gegevens uit externe bronnen wordt gebruikt.
