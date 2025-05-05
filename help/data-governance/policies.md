---
title: Beleid
description: Leer hoe u het beleid kunt benaderen vanuit de Mix Modeler.
feature: Administration
exl-id: 4dba7c30-ad1e-4213-a2b0-afc55f2448a3
source-git-commit: 132dc18b84723358a7d65e2aaadd49cf1deb2dd8
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 1%

---

# Beleid

Zodra u door het werkschema gaat om een model tot stand te brengen en de configuratie van het model voor te leggen, [ beleidshandhaving ](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/enforcement/overview#automatic-enforcement) controles om te zien of zijn er om het even welke schendingen. Als een beleidsovertreding optreedt, wordt een pop-up weergegeven die aangeeft dat een of meer beleidsregels zijn overtreden. Deze controle moet ervoor zorgen dat uw gegevensverrichtingen en marketing acties binnen Experience Platform met het beleid van het gegevensgebruik verenigbaar zijn.

Standaard controleert de Mix Modeler op overtredingen van door de Adobe gedefinieerd beleid die zijn gekoppeld aan de volgende labels en marketingacties:

| Beleidsnaam | Gekoppeld label | Bijbehorende marketingactie |
|---|---|---|
| Gebruiksanalyses en gebruikersgebaseerde metingen beperken | C8 | Analytics |
| Gegevenswetenschap beperken | C9 | Gegevenswetenschap |
| Gegevens beperken bij exporteren | 12 | Gegevens exporteren |

Overtredingen worden ook gecontroleerd op het beleid dat u zelf hebt gedefinieerd en dat marketingacties bevat die in de bovenstaande tabel worden vermeld.

Wanneer het overtreden van een beleid terwijl het bouwen van een datasetregel, ziet u popover die informatie over de beleidsschending toont.

Bijvoorbeeld:

- u hebt het [!UICONTROL Restrict data science] beleid met het bijbehorende label [!UICONTROL C9] en de bijbehorende marketingactie [!UICONTROL Data Science] ingeschakeld,
- u hebt het label [!UICONTROL C9] - [!UICONTROL No data science] toegepast op het veld `totalCost` in het schema Conversiegegevens,
- U wilt een gegevenssetregel instellen die, onder andere, het `totalCost` -veld van het Conversiegegevensschema toewijst aan het geharmoniseerde veld met de naam `spend` (en de weergavenaam `Spend` ).

Wanneer u de datasetregel wilt bewaren, ziet u **[!UICONTROL Data governance policy violation detected]** popup, tonend een lijst van geschonden beleid. Wanneer u de naam van het beleid selecteert, wordt in [!UICONTROL Violation summary] een lijst weergegeven met de tags [!UICONTROL Active data governance labels] , [!UICONTROL Entity] , [!UICONTROL Type] , [!UICONTROL Field] en [!UICONTROL Government labels] toegepast.

<!-- pending screenshot -->

Wanneer het toepassen van een etiket van het gegevensgebruik op een schemagebied dat reeds in geharmoniseerde gegevens wordt gebruikt, ziet u een popover die informatie over de beleidsschending toont.

Bijvoorbeeld:

- u hebt een gegevenssetregel ingesteld die, onder andere, het `totalCost` -veld van uw Conversiegegevensschema koppelt aan het geharmoniseerde veld met de naam `spend` (en weergavenaam `Spend` ).
- u hebt met succes de geharmoniseerde gegevens met succes minstens eens gesynchroniseerd (zie [ regels Dataset - de gegevens van de Synchronisatie ](/help/harmonize-data/dataset-rules.md#sync-data)).
- u schakelt het [!UICONTROL Restrict data science] beleid met het bijbehorende label [!UICONTROL C9] en de bijbehorende marketingactie [!UICONTROL Data Science] in.
- u wilt het label [!UICONTROL C9] - [!UICONTROL No data science] toepassen op het veld `totalCost` in het schema Conversiegegevens.

Wanneer u de schema-update wilt opslaan, ziet u een **[!UICONTROL Data governance policy violation detected]** pop-up met een lijst met overtreden beleidsregels. Selecteer de naam van het beleid in de [!UICONTROL Violation summary] om meer details in de [!UICONTROL Data Lineage] lijst te vinden.

<!-- pending screenshot -->

## Overtredingen gedetecteerd

De geconstateerde overtreding van het gegevensbeheerbeleid geeft specifieke informatie over de schending. U kunt deze schendingen door beleidsmontages en andere maatregelen oplossen die niet direct met het configuratiewerkschema verwant zijn. U kunt bijvoorbeeld de labels wijzigen, zodat bepaalde velden mogen worden gebruikt voor wetenschappelijke doeleinden. Alternatief, kon u de modelconfiguratie zelf ook wijzigen, zodat het model geen voorwerp met een etiket van het gegevensgebruik gebruikt.

De ![ 2&rbrace; selectie van de Privacy ](/help/assets/icons/Privacy.svg) &lbrace;in het linkerspoor verleent toegang tot de [!UICONTROL Policies] interface van Experience Platform, die uw beleid, etiketten en marketing acties toestaat te beheren.**[!UICONTROL Policies]**

<!--
Currently,  Mix Modeler does not support all of the data governance functionality offered by Experience Platform. Field level access control is supported. See [Field level access control](../harmonize-data/dataset-rules.md#field-level-access-control)
-->

>[!MORELIKETHIS]
>
>[ Overzicht van het het gebruiksbeleid van Gegevens ](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/policies/overview)
>
>

