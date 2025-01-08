---
title: Workflow voor Mixxen Modeler
description: Begrijp het typische werkschema voor Mix Modeler.
feature: Ingest Data, Plans, Harmonized Data, Models
exl-id: 200ff846-5d78-4b25-a425-bfd558b88c88
source-git-commit: da92298bbd5b2fc14b54121f0c43dc3763f9a0a3
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# Workflow voor Mixxen Modeler

Bekijk deze video voor een inleiding aan het gebruikerswerkschema in Mix Modeler.

>[!VIDEO](https://video.tv.adobe.com/v/3424854/?learn=on)


Een typisch werkschema in Mix Modeler bestaat uit de volgende activiteiten:

![ de tekst van Alt ](/help/assets/ApplicationWorkflow.svg)

|  | Activiteit | Beschrijving |
|---|---|---|
| ![ Gegevens ](/help/assets/icons/Data.svg){width="100"} | [**Ingest gegevens**](../ingest-data/overview.md) | Gegevens over gebeurtenissen uit Experience Platform (bijvoorbeeld Adobe Analytics, Web SDK, andere bronnen), samengevoegde gegevens uit marketingkanalen (bijvoorbeeld tv, tuinen, e-mail, eigendom en activiteiten), gegevens over externe factoren van klanten (bijvoorbeeld prijswijzigingen in abonnementsdiensten) en gegevens over interne factoren (bijvoorbeeld vakantieplannen). |
| ![ DataCheck ](/help/assets/icons/DataCheck.svg){width="100"} | [**harmoniseer gegevens**](../harmonize-data/overview.md) | Vorm toewijzingsregels en de regels van de conflictoplossing om de diverse marketing datasets te verenigen nodig om campagneprestaties in Mix Modeler te meten en te plannen. |
| ![ FileConfig ](/help/assets/icons/FileGear.svg){width="100"} | [**vorm modellen**](../models/create.md) | Configureer modelinstanties met marketingaanraakpunten (bijvoorbeeld kanalen), conversiedefinities en interne en externe factoren. |
| ![ FileData ](/help/assets/icons/FileData.svg){width="100"} | [**Lijn en scoremodellen**](../models/overview.md) | Samengevoegde scores en scores op gebeurtenisniveau maken met behulp van training en scoring in computers. |
| ![ FileChart ](/help/assets/icons/FileChart.svg){width="100"} | [**creeer plannen**](../plans/overview.md) | Bepaal de beste toewijzing van marketingfondsen om een bedrijfsdoelstelling te bereiken aan de hand van de resultaten van de modellen van de Mix Modeler. |
| ![ Dashboard ](/help/assets/icons/Dashboard.svg){width="100"} | [**het dashboard van het Overzicht**](../dashboard/overview.md) | Krijg inzicht in geharmoniseerde gegevens, modellen, en plannen, gebruikend diverse configureerbare visualisaties. |

{style="table-layout:auto"}

<!---
The detailed data-oriented flowchart below illustrates how:

* harmonized data is based on:

  * experience event data (originating from Analytics source connector, collected through Experience Platform SDKs and APIs, ingested through source connectors, or using streaming ingestion),
  * aggregate or summary data from walled gardens (like Facebook, YouTube), traffic sources, or offline advertising data, and 
  * definitions of harmonized fields and dataset rules.

* a model is based on:

  * the conversion and marketing touchpoint definitions resulting from the harmonized data and 
  * non-marketing aggregate or summary data containing internal or external factors.

* mult-touch attribution event scores can potentially be fed back into Experience Platform data lake for use in subsequent model configuration, training and scoring.

![Comprehensive workflow](/help/assets/comprehensive-workflow.svg)

-->
