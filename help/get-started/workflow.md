---
title: Workflow voor Mixxen Modeler
description: Begrijp het typische werkschema voor Mix Modeler.
feature: Ingest Data, Plans, Harmonized Data, Models
exl-id: 200ff846-5d78-4b25-a425-bfd558b88c88
source-git-commit: 33883626d8e7aca2eecc3571593be53ef41ac458
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Workflow voor Mixxen Modeler

Een typisch werkschema in Mix Modeler kijkt als:

![Alt-tekst](../assets/ApplicationWorkflow.svg)

|  | Activiteit | Beschrijving |
|---|---|---|
| ![Gegevens](../assets/icons/Data.svg){width="100"} | [**Samenvattingsgegevens**](../ingest-data/overview.md) | Gegevens over gebeurtenissen uit Experience Platform (bijvoorbeeld Adobe Analytics, Web SDK, andere bronnen), samengevoegde gegevens uit marketingkanalen (bijvoorbeeld tv, tuinen, e-mail, eigendom en activiteiten), gegevens over externe factoren van klanten (bijvoorbeeld prijswijzigingen in abonnementsdiensten) en gegevens over interne factoren (bijvoorbeeld vakantiepatronen). |
| ![DataCheck](../assets/icons/DataCheck.svg){width="100"} | [**Gegevens harmoniseren**](../harmonize-data/overview.md) | Vorm toewijzingsregels en de regels van de conflictoplossing om de diverse marketing datasets te verenigen nodig om campagneprestaties in Mix Modeler te meten en te plannen. |
| ![FileConfig](../assets/icons/FileGear.svg){width="100"} | [**Modellen configureren**](../models/create.md) | Vorm modelinstanties met marketing touchpoints (bijvoorbeeld kanalen) en omzettingsdefinities. |
| ![FileData](../assets/icons/FileData.svg){width="100"} | [**Train- en scoremodellen**](../models/overview.md) | Samengevoegde scores en scores op gebeurtenisniveau maken met behulp van training en scoring in computers. |
| ![FileChart](../assets/icons/FileChart.svg){width="100"} | [**Abonnementen maken**](../plans/overview.md) | Bepaal de beste toewijzing van marketingfondsen om een bedrijfsdoelstelling te bereiken aan de hand van de resultaten van de modellen van de Mix Modeler. |
| ![Dashboard](../assets/icons/Dashboard.svg){width="100"} | [**Overzichtdashboard**](../dashboard/overview.md) | Bekijk de geharmoniseerde gegevens, modellen en plannen met behulp van verschillende configureerbare widgets. |

{style="table-layout:auto"}
