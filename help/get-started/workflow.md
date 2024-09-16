---
title: Workflow voor Mixxen Modeler
description: Begrijp het typische werkschema voor Mix Modeler.
feature: Ingest Data, Plans, Harmonized Data, Models
exl-id: 200ff846-5d78-4b25-a425-bfd558b88c88
source-git-commit: 9a6c1f1c12ab29da80a1997cfd31ca07b38eaa22
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Workflow voor Mixxen Modeler

Bekijk deze video voor een inleiding aan het gebruikerswerkschema in Mix Modeler.

>[!VIDEO](https://video.tv.adobe.com/v/3424854/?learn=on)


Een typisch werkschema in Mix Modeler bestaat uit de volgende activiteiten:

![ de tekst van Alt ](/help/assets/ApplicationWorkflow.svg)

|  | Activiteit | Beschrijving |
|---|---|---|
| ![ Gegevens ](/help/assets/icons/Data.svg){width="100"} | [**Ingest gegevens**](../ingest-data/overview.md) | Gegevens over gebeurtenissen uit Experience Platform (bijvoorbeeld Adobe Analytics, Web SDK, andere bronnen), samengevoegde gegevens uit marketingkanalen (bijvoorbeeld tv, tuinen, e-mail, eigendom en activiteiten), gegevens over externe factoren van klanten (bijvoorbeeld prijswijzigingen in abonnementsdiensten) en gegevens over interne factoren (bijvoorbeeld vakantiepatronen). |
| ![ DataCheck ](/help/assets/icons/DataCheck.svg){width="100"} | [**harmoniseer gegevens**](../harmonize-data/overview.md) | Vorm toewijzingsregels en de regels van de conflictoplossing om de diverse marketing datasets te verenigen nodig om campagneprestaties in Mix Modeler te meten en te plannen. |
| ![ FileConfig ](/help/assets/icons/FileGear.svg){width="100"} | [**vorm modellen**](../models/create.md) | Configureer modelinstanties met marketingaanraakpunten (bijvoorbeeld kanalen), conversiedefinities en interne en externe factoren. |
| ![ FileData ](/help/assets/icons/FileData.svg){width="100"} | [**Lijn en scoremodellen**](../models/overview.md) | Samengevoegde scores en scores op gebeurtenisniveau maken met behulp van training en scoring in computers. |
| ![ FileChart ](/help/assets/icons/FileChart.svg){width="100"} | [**creeer plannen**](../plans/overview.md) | Bepaal de beste toewijzing van marketingfondsen om een bedrijfsdoelstelling te bereiken aan de hand van de resultaten van de modellen van de Mix Modeler. |
| ![ Dashboard ](/help/assets/icons/Dashboard.svg){width="100"} | [**het dashboard van het Overzicht**](../dashboard/overview.md) | Krijg inzicht in geharmoniseerde gegevens, modellen, en plannen, gebruikend diverse configureerbare visualisaties. |

{style="table-layout:auto"}

Het gedetailleerde gegevensgeoriënteerde stroomschema hieronder illustreert hoe:

* geharmoniseerde gegevens zijn gebaseerd op:

   * ervaringsgegevens (afkomstig van de bronconnector van Analytics, verzameld via Experience Platform-SDK&#39;s en API&#39;s, opgenomen via bronconnectors of via streaming opname);
   * samengevoegde of samenvattingsgegevens van tuinen (zoals Facebook, YouTube), verkeersbronnen of gegevens over offlinereclame, en
   * definities van geharmoniseerde velden en gegevenssetregels.

* een model is gebaseerd op :

   * de conversie- en marketingdefinities van aanspreekpunten die voortvloeien uit de geharmoniseerde gegevens en
   * niet-marketingaggregaat of samenvattende gegevens die interne of externe factoren bevatten.

* Mut-touch attributie-gebeurtenisscores kunnen mogelijk worden teruggeplaatst in het Experience Platform data Lake voor gebruik in volgende modelconfiguratie, training en scoring.

![ Uitgebreide werkschema ](/help/assets/comprehensive-workflow.svg)
