---
title: Schema's
description: Leer hoe u de schema's beheert die nodig zijn om gegevens in Mix Modeler in te voeren.
feature: Schemas
exl-id: 08289581-5af9-4422-b049-8c24105e2a8e
source-git-commit: 7524c2ffc0408b04e6bef5bd5deedc1feea0b682
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 1%

---

# Schema&#39;s

Om schema&#39;s te beheren, ondersteunend de gegevens u in Experience Platform en gebruik in Mix Modeler wilt opnemen:

1. Ga naar de Mix Modeler interface.

1. Selecteer ![&#x200B; Schema&#39;s &#x200B;](/help/assets/icons/Schemas.svg) **[!UICONTROL Schemas]**, onder **[!UICONTROL SETUP]**.

Zie het [&#x200B; overzicht van Schema&#39;s UI &#x200B;](https://experienceleague.adobe.com/docs/experience-platform/xdm/ui/overview.html?lang=nl-NL) voor meer informatie.

## Samengevoegde of samenvattingsgegevens

Het wordt ten zeerste aanbevolen de klasse XDM Summary Metrics als basis van het schema te gebruiken dat ten grondslag ligt aan geaggregeerde of samenvattingsgegevens die u in Experience Platform wilt opnemen en die u in Mix Modeler wilt gebruiken.

Gebruik de klasse XDM Summary Metrics voor:

- tuingegevens, bijvoorbeeld gegevens van Facebook of YouTube.

- gegevens over externe factoren, zoals gegevens uit SPX (S&amp;P 500 aandelenindexen), weergegevens;

- gegevens over interne factoren, bijvoorbeeld prijswijzigingen, een vakantiekalender.

>[!IMPORTANT]
>
>De schemadefinitie moet minstens één numeriek gebied (het gebruiken van Geheel, Dubbel, Van Boole, of ander numeriek type) bevatten om de vereiste metriek voor de opgenomen gegevens te steunen.

Een schema met de basisklasse **[!DNL XDM Summary Metrics]** kan eenvoudig zijn, zoals in **[!DNL ExternalFactorSummarySchema]** hieronder wordt getoond.

![&#x200B; Extern het Schema van Factoren &#x200B;](/help/assets/external-factors-schema.png)

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

![&#x200B; Samenvattingsschema &#x200B;](/help/assets/summary-schema.png)

Gezien de asynchrone aard van profielopname, wanneer het verzamelen van geaggregeerde of summiere gegevens uit externe bronnen, wordt het aangemoedigd om de Externe het gebiedsgroep van de Details van de Controle van het Systeem van Source als deel van een schema te gebruiken. Deze veldgroep definieert een set auditeigenschappen voor externe bronnen.

## Factor Standaard velden, veldgroep

Voor het gemak, steunt Experience Platform een specifieke het gebiedsgroep van de Gebieden van de Factor Standaard voor interne en externe factoren gegevens vaak deel van samenvatting, interne factor, of externe factorgegevens. Deze veldgroep definieert de volgende velden:

| Weergavenaam veld | Veldnaam | Veldtype | Gegevenstype | Vereist | Beschrijving |
|---|---|---|---|:-:|---|
| Naam factor | factorName | Dimension | String | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | De naam van de factor |
| Waarde factor | factorValue | Metrisch | Dubbel | ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) | De waarde van de factor |
| Type factor | factorType | Dimension | String (Enum) | | Het type factor.<br/> Mogelijke waarden zijn: <ul><li>Intern (interne factor)</li><li>Extern (externe factor)</li></ul> |
| Type waarde | valueType | Dimension | String (Enum) | | Mogelijke waarden zijn:<ul><li>Werkelijk (werkelijke waarde)</li><li>Voorspeld (voorspelde waarde)</li></ul>Als er geen waarde is, is Actueel de standaardwaarde. |
| Korreligheid | granulariteit | Dimension | String (Enum) | | Mogelijke waarden zijn:<ul><li>Dagelijks</li><li>Wekelijks</li><li>Maandelijks</li></ul> |

Een samenvatting, interne factor, of externe factordataset kan op:

- Een schema dat **&#x200B;**&#x200B;de Groep van de Gebieden van de Factor Standaard gebruikt. Deze dataset wordt getoond als **[!UICONTROL Factors]** dataset wanneer u datasetregels vormt. En de geharmoniseerde gebieden u, als deel van de datasetregels voor de dataset bepaalt, zijn beschikbaar als factoren wanneer u een model creeert.
- Een schema dat **niet** de Groep van de Gebieden van de Factor Standaard gebruikt. Deze dataset wordt getoond als **[!UICONTROL Summary]** dataset wanneer u datasetregels vormt. De dataset wordt gevormd als summiere gegevens en beïnvloedt geharmoniseerde gegevens niet.

## Ondersteunde gegevenstypen

Mix Modeler biedt momenteel geen ondersteuning voor een subset van Experience Platform-gegevenstypen. De volgende basisgegevenstypes (gebieden), die in [&#x200B; Grondbeginselen van schemacompositie &#x200B;](https://experienceleague.adobe.com/docs/experience-platform/xdm/schema/composition.html?lang=nl-NL#data-type) worden vermeld, worden gesteund:

- String
- Geheel
- Dubbel
- Boolean
- Lang
- Kort
- Byte
- Datum
- Datum/tijd


>[!MORELIKETHIS]
>
>- [&#x200B; Schemas &#x200B;](schemas.md)
