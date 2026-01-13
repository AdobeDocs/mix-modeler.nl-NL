---
title: Overzicht van plannen
description: Leer hoe u plannen in Mix Modeler kunt weergeven, selecteren en uitvoeren.
feature: Plans
exl-id: 45a8dc30-3259-493d-8ea5-1899903733a6
source-git-commit: 0d11168b71319e6c854482f89dbb1bb68962a880
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

# Overzicht van plannen

Met de plannen in Mix Modeler kunt u budgetten toewijzen per bedrijfseenheid en kanaal. De planningsfunctionaliteit is geïntegreerd met de resultaten van de getrainde modellen op basis van uw geharmoniseerde gegevens.

In een plan worden de discretionaire investeringen (bijvoorbeeld budgetten) beschreven die een bedrijf in de loop van een bepaald tijdsbestek aan marketinggerelateerde projecten wil besteden. Deze investeringen zijn in dienst van gemeenschappelijke KPI&#39;s (bijvoorbeeld orders, inkomsten). De plannen kunnen uitgaven van kanalen zoals betaalde reclame, gesponsorde Web-inhoud, gebeurtenissen omvatten.

Een plan vereist:

- een model,
- een gegevensbereik,
- een begroting.

Een plan kan eventueel omvatten:

- een geconfigureerd herkenningsvenster,
- meerdere vluchtdata met elk een doelbudget;
- minimum- en maximumbegrotingsbeperkingen per kanaal en vluchtdatum.

Als een model dat u voor uw plan hebt gebruikt op nieuwe gegevens wordt gescoord, moet u een nieuw plan tot stand brengen om rekening met de opnieuw geschetste gegevens te houden.


## Abonnementen maken

Als u een plan wilt maken, gebruikt u de wizard voor het maken van een Mix Modeler-abonnement. Zie [&#x200B; bouwt plannen &#x200B;](build.md) voor meer details.


## Abonnementen beheren

Als u een tabel met uw huidige plannen wilt weergeven, gaat u naar de interface van Mix Modeler:

1. Selecteer ![](/help/assets/icons2/FileChart.svg) **[!UICONTROL Plans]** in het linkerspoor.

1. U ziet een tabel met de huidige plannen en hun status.

   De tabelkolommen geven details over de plannen op.

   | Kolomnaam | Details |
   |---|---|
   | Naam | Naam van het plan |
   | Model | Het model dat als basis voor het plan wordt gebruikt. |
   | Datumbereik | Het volledige datumbereik voor een abonnement. |
   | Begroting | De totale begroting voor een plan. |
   | Plan-doel | Het doel metrisch bepaalde voor een doel gebaseerd plan. |
   | Voorspelde terugkeer | De [&#x200B; voorspelde terugkeer &#x200B;](/help/main-guide/glossary.md) voor een plan |
   | voorspelde ROI | Het [&#x200B; voorspelde ROI &#x200B;](/help/main-guide/glossary.md) voor een plan. |
   | Voorspelde conversie | De [&#x200B; voorspelde omzetting &#x200B;](/help/main-guide/glossary.md) voor een plan |
   | Voorspelde CPA | [&#x200B; voorspelde CPA &#x200B;](/help/main-guide/glossary.md) voor een plan |
   | Status | De status van een plan: <p><span style="color:red">●</span> Mislukt, <p><span style="color:blue">●</span> Verwerken, of <p><span style="color:green">●</span> Voltooid. |

   {style="table-layout:auto"}

   U kunt ![&#x200B; gebruiken ColumnSetting &#x200B;](/help/assets/icons/ColumnSetting.svg) om ![&#x200B; Vinkje &#x200B;](/help/assets/icons/Checkmark.svg) te selecteren de kolommen in de lijst te tonen.

   Om de lijst op om het even welke kolom in het stijgen ![&#x200B; te sorteren ArrowMoveUp &#x200B;](/help/assets/icons2/ArrowMoveUp.svg) of dalende ![&#x200B; ArrowMoveDown &#x200B;](/help/assets/icons2/ArrowMoveDown.svg) orde, selecteer de titel van de kolom.

   Om te sorteren of resize **[!UICONTROL Name]**, **[!UICONTROL Model]** of **[!UICONTROL Date range]** kolom, uitgezochte **[!UICONTROL Name]** ![&#x200B; ChevronDown &#x200B;](/help/assets/icons/ChevronDown.svg), **[!UICONTROL Model]** ![&#x200B; ChevronDown &#x200B;](/help/assets/icons/ChevronDown.svg) of **[!UICONTROL Date range]** ![&#x200B; ChevronDown &#x200B;](/help/assets/icons/ChevronDown.svg). Selecteer **[!UICONTROL Sort ascending]**, **[!UICONTROL Sort descending]** of **[!UICONTROL Resize column]** in het contextmenu. U kunt de muisaanwijzer ook boven het kolomscheidingsteken voor deze kolommen plaatsen om het formaat van een kolom te wijzigen.

1. Het gebruik ![&#x200B; Onderzoek &#x200B;](/help/assets/icons/Search.svg) om de lijst voor één of meerdere specifieke plannen te zoeken en te filtreren.

### Abonnementen

Om de inzichten van een plan te bekijken en een plan uit te geven:

1. Selecteer ![&#x200B; PLan &#x200B;](/help/assets/icons/FileChart.svg) **[!UICONTROL Plans]** van het linkerspoor.

1. Selecteer de naam van het abonnement.

U wordt opnieuw gericht aan [&#x200B; Inzichten van het Plan &#x200B;](insights.md).


### Een abonnement dupliceren

Een abonnement dupliceren:

- Selecteer ![&#x200B; Meer &#x200B;](/help/assets/icons/More.svg) voor een plan. Selecteer **[!UICONTROL Duplicate]** in het contextmenu.
- Alternatief, selecteer een plan in de lijst ![&#x200B; SelectBox &#x200B;](/help/assets/icons/SelectBox.svg) en selecteer ![&#x200B; Exemplaar &#x200B;](/help/assets/icons/Copy.svg) **[!UICONTROL Duplicate]** van de blauwe actiebar.

Een nieuw plan, met een naam die uit de originele die naam van het plan wordt samengesteld met **[!UICONTROL (Copy)]wordt toegevoegd (_n_)**, wordt gecreeerd. U wordt automatisch opnieuw gericht aan [&#x200B; de verwezenlijking van het Plan &#x200B;](build.md) om bijgewerkte details voor het gekopieerde plan te verstrekken.

- De details (zoals Beschrijving, Begroting, en meer) van het originele plan worden gekopieerd over.
- Begrotingsbeperkingen van het oorspronkelijke plan worden naar het nieuwe gemaakte plan gekopieerd.
- U hebt de optie om een ander model als basis voor het gekopieerde plan te selecteren.
   - Voor aanraakpunten of kanalen die wel in het gekopieerde plan bestaan, maar niet in het nieuw geselecteerde model bestaan, worden eventuele beperkingen voor deze aanraakpunten of kanalen uit het plan verwijderd.
   - Voor aanraakpunten of kanalen die niet in het gekopieerde plan bestaan, maar wel in het nieuw geselecteerde model, worden de beperkingen ingesteld op:
      - een minimumwaarde van `0`,
      - een maximumwaarde die in overeenstemming is met de begroting voor het vliegbereik van het plan.



### Abonnementen vergelijken

Plannen vergelijken:

1. Selecteer twee plannen in de tabel.
1. Selecteer ![&#x200B; vergelijken &#x200B;](/help/assets/icons/Compare.svg) **[!UICONTROL Compare]** van de blauwe actiebar. U ziet de gebruikersinterface van **[!UICONTROL Compare plans]** .


### Abonnementen verwijderen

Een abonnement verwijderen:

1. Selecteer ![&#x200B; Meer &#x200B;](/help/assets/icons/More.svg) voor een plan. Selecteer **[!UICONTROL Delete]** in het contextmenu. <br/> Alternatief, selecteer een plan in de lijst ![&#x200B; SelectBox &#x200B;](/help/assets/icons/SelectBox.svg) en selecteer ![&#x200B; Schrapping &#x200B;](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** van de blauwe actiebar.
1. Selecteer **[!UICONTROL Delete]** in het bevestigingsdialoogvenster van **[!UICONTROL Delete plan]** om het abonnement te verwijderen. Selecteer **[!UICONTROL Cancel]** om te annuleren.

Meerdere plannen verwijderen:

1. Selecteer meerdere plannen.
1. Van de blauwe actiebar, uitgezochte ![&#x200B; Schrapping &#x200B;](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** om de plannen te schrappen.
1. Selecteer **[!UICONTROL Delete]** in de **[!UICONTROL Delete *x *plannen]**&#x200B;bevestigingsdialoog om de plannen te schrappen. Selecteer **[!UICONTROL Cancel]**&#x200B;om te annuleren.


