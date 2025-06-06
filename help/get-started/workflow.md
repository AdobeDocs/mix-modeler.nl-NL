---
title: Mix Modeler-workflow
description: Begrijp de standaardworkflow voor Mix Modeler.
feature: Ingest Data, Plans, Harmonized Data, Models
exl-id: 200ff846-5d78-4b25-a425-bfd558b88c88
source-git-commit: bdb5992ba1e6a4e5aa546b6ffb8e9673ed69be22
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Mix Modeler-workflow

Bekijk deze video voor een inleiding op de gebruikersworkflow in Mix Modeler.

>[!VIDEO](https://video.tv.adobe.com/v/3424854/?learn=on)


Een typische workflow in Mix Modeler bestaat uit de volgende activiteiten:

![ de tekst van Alt ](/help/assets/ApplicationWorkflow.svg)

|  | Activiteit | Beschrijving |
|---|---|---|
| ![ Gegevens ](/help/assets/icons/Data.svg){width="100"} | [**Ingest gegevens**](../ingest-data/overview.md) | Gegevens over evenementen uit Experience Platform (bijvoorbeeld Adobe Analytics, Web SDK, andere bronnen), samengevoegde gegevens uit marketingkanalen (bijvoorbeeld tv, tuinen, e-mail, eigendom en activiteiten), gegevens over externe factoren van klanten (bijvoorbeeld prijswijzigingen in abonnementsdiensten) en gegevens over interne factoren (bijvoorbeeld vakantieplannen). |
| ![ DataCheck ](/help/assets/icons/DataCheck.svg){width="100"} | [**harmoniseer gegevens**](../harmonize-data/overview.md) | Configureer toewijzingsregels en conflictoplossingsregels om de verschillende marketingdatasets samen te voegen die nodig zijn om de campagneresultaten in Mix Modeler te meten en te plannen. |
| ![ FileConfig ](/help/assets/icons/FileGear.svg){width="100"} | [**bouwt modellen**](../models/overview.md) | Buid-modelexemplaren met marketingaanraakpunten (bijvoorbeeld kanalen), conversiedefinities en interne en externe factoren. |
| ![ FileData ](/help/assets/icons/FileData.svg){width="100"} | [**Lijn en scoremodellen**](../models/overview.md) | Samengevoegde scores en scores op gebeurtenisniveau maken met behulp van training en scoring in computers. |
| ![ FileChart ](/help/assets/icons/FileChart.svg){width="100"} | [**bouwt plannen**](../plans/overview.md) | Maak en maak plannen. Bepaal de beste toewijzing van marketingfondsen om een bedrijfsdoelstelling te bereiken door gebruik te maken van de productie van Mix Modeler-modellen. |
| ![ Dashboard ](/help/assets/icons/Dashboard.svg){width="100"} | [**het dashboard van het Overzicht**](../dashboard/overview.md) | Krijg inzicht in geharmoniseerde gegevens, modellen, en plannen, gebruikend diverse configureerbare visualisaties. |

{style="table-layout:auto"}

Hieronder wordt een overzicht gegeven van hoe invoergegevens in Mix Modeler kunnen stromen en hoe Mix Modeler uitvoergegevens voor zijn eigen interface maar ook voor andere oplossingen, zoals Customer Journey Analytics, kan produceren.

![ de stroom van de inputoutputgegevens van Mix Modeler ](../assets/mm-input-output.png)
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
