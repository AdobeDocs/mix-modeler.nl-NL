---
title: Schema's
description: Leer hoe te om de schema's te beheren die worden vereist om gegevens in Mix Modeler in te voeren.
feature: Schemas
exl-id: 08289581-5af9-4422-b049-8c24105e2a8e
source-git-commit: 9a6c1f1c12ab29da80a1997cfd31ca07b38eaa22
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 2%

---

# Schema&#39;s

Om schema&#39;s te beheren, ondersteunend de gegevens u in Experience Platform en gebruik in Mix Modeler wilt opnemen:

1. Ga naar de interface van de Mix Modeler.

1. Selecteer ![ Schema&#39;s ](/help/assets/icons/Schemas.svg) **[!UICONTROL Schemas]**, onder **[!UICONTROL SETUP]**.

Zie het [ overzicht van Schema&#39;s UI ](https://experienceleague.adobe.com/docs/experience-platform/xdm/ui/overview.html?lang=en) voor meer informatie.

## Samengevoegde of samenvattingsgegevens

Het wordt ten zeerste aanbevolen de klasse XDM Summary Metrics als basis van het schema te gebruiken dat ten grondslag ligt aan geaggregeerde of samenvattingsgegevens die u in Experience Platform wilt opnemen en in Mix Modeler wilt gebruiken.

Gebruik de klasse XDM Summary Metrics voor:

- tuingegevens, bijvoorbeeld gegevens uit Facebook of YouTube.

- gegevens over externe factoren, zoals gegevens uit SPX (S&amp;P 500 aandelenindexen), weergegevens;

- gegevens over interne factoren, bijvoorbeeld prijswijzigingen, een vakantiekalender.

>[!IMPORTANT]
>
>De schemadefinitie moet minstens één numeriek gebied (het gebruiken van Geheel, Dubbel, Van Boole, of ander numeriek type) bevatten om de vereiste metriek voor de opgenomen gegevens te steunen.

Een schema met de basisklasse **[!DNL XDM Summary Metrics]** kan eenvoudig zijn, zoals in **[!DNL ExternalFactorSummarySchema]** hieronder wordt getoond.

![ Extern het Schema van Factoren ](/help/assets/external-factors-schema.png)

Dit eenvoudige schema kan worden gebruikt om datasets in te voeren die gegevens bevatten, bijvoorbeeld:

- Concurrentie-indexgegevens

  | tijdstempel | date_type | factor | value |
  |---|---|---|--:|
  | 2020-11-28T00 :00: 00.000Z | week | concurrent_index | 289,8 |
  | 2020-12-05T00 :00: 00.000Z | week | concurrent_index | 291,2 |
  | 2020-12-12T00 :00: 00.000Z | week | concurrent_index | 280,07 |
  | ... | ... | ... | ... |

- Publieke vakantiegegevens

  | tijdstempel | date_type | factor | value |
  |---|---|---|--:|
  | 2020-11-28T00 :00: 00.000Z | week | all_Feays_flag | 0,0 |
  | 2020-12-05T00 :00: 00.000Z | week | all_Feays_flag | 0,0 |
  | 2020-12-12T00 :00: 00.000Z | week | all_Feays_flag | 0,0 |
  | 2020-12-19T00 :00: 00.000Z | week | all_Feays_flag | 0,0 |
  | 2020-12-26T00 :00: 00.000Z | week | all_Feays_flag | 1,0 |
  | ... | ... | ... | ... |


Zie hieronder voor een uitgebreider voorbeeld van een instructie **[!DNL LumaPaidMarketingSchema]** waarbij **[!DNL XDM Summary Metrics]** als basisklasse wordt gebruikt. Het schema gebruikt specifieke gebiedsgroepen (die met kleuren worden geannoteerd) voor metriek (**[!DNL AMMMetrics]**), dimensies (**[!DNL AMMDimensions]**), en andere klant-specifieke informatie (**[!DNL CustomerSpecific]**).

![ Samenvattingsschema ](/help/assets/summary-schema.png)

Gezien de asynchrone aard van profielopname, wanneer het verzamelen van geaggregeerde of summiere gegevens uit externe bronnen, wordt het aangemoedigd om de Externe het gebiedsgroep van de Details van de Controle van het Systeem van Source als deel van een schema te gebruiken. Deze veldgroep definieert een set auditeigenschappen voor externe bronnen.


## Ondersteunde gegevenstypen

Mix Modeler ondersteunt momenteel geen subset van gegevenstypen voor Experience Platforms. De volgende basisgegevenstypes (gebieden), die in [ Grondbeginselen van schemacompositie ](https://experienceleague.adobe.com/docs/experience-platform/xdm/schema/composition.html?lang=en#data-type) worden vermeld, worden gesteund:

- String
- Geheel
- Dubbel
- Boolean
- Lang
- Kort
- Byte
- Datum
- Datum/tijd
