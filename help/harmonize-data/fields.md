---
title: Geharmoniseerde velden
description: Leer hoe u velden definieert die u kunt gebruiken als onderdeel van het harmoniseren van uw gegevens in de Mix Modeler.
feature: Harmonized Data, Harmonized Fields
exl-id: f051279a-1ae9-49bd-a946-abfc34c90413
source-git-commit: fecb122f6e2e8ae532babd0e2964ad200174a032
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 0%

---

# Geharmoniseerde velden

Met geharmoniseerde velden kunt u velden definiëren voor conceptueel dezelfde gegevens, die afkomstig zijn van verschillende bronnen, elk met een eigen definitie van die gegevens. Een klikmeting kan bijvoorbeeld anders worden gedefinieerd en benoemd, afhankelijk van de gegevensbron. Als u op een geharmoniseerd veld klikt, kunt u een algemene nomenclatuur definiëren voor klikmetrische gegevens op basis van deze verschillende bronnen van klikgegevens.

Met geharmoniseerde velden kunt u de velden definiëren die u wilt gebruiken als onderdeel van de workflow voor het harmoniseren van gegevens. De gebieden u bepaalt kunnen in het bepalen van datasetregels, marketing worden gebruikt aanraakpunten en omzettingen.

## Globale harmonisatievelden

De standaard beschikbare globale harmonisatievelden in Mix Modeler zijn:


| Veldnaam | Weergavenaam | Categorie | Gegevenstype | Opmerking |
| ---------------------- | ---------------------- | --------- | --------- | --------- |
| merk | Merk | Dimension | String |           |
| campagne | Campaign | Dimension | String |           |
| kanaal | Kanaal | Dimension | String |           |
| channel_id | Kanaal-id | Dimension | String |           |
| channel_type_at_source | Kanaaltype bij bron | Dimension | String |           |
| kanaal | Kanaal | Dimension | String |           |
| klikken | Klikken | Metrisch | Getal |           |
| conversietype | Conversietype | Dimension | String |           |
| kosten | Kosten | Metrisch | Valuta |           |
| gegevensset | Gegevensset | Dimension | String |           |
| date_type | Datumtype | Dimension | String | dag, week |
| e-mail | Verzonden e-mails | Metrisch | Getal |           |
| event_date | Datum | Dimension | Datum en tijd |           |
| bruto_demand | Bruto-vraag | Metrisch | Valuta |           |
| indrukken | Impessies | Metrisch | Getal |           |
| last_updated_date | Laatst bijgewerkt op | Dimension | Datum en tijd |           |
| koppelbezoeken | Bezoekingen koppelen | Metrisch | Getal |           |
| mediatype | Mediatype | Dimension | String |           |
| net_sales | Nettoverkoop | Metrisch | Valuta |           |
| orders | Orders | Metrisch | Getal |           |
| sourceType | Brontype | Dimension | String |           |
| besteden | Draaien | Metrisch | Valuta |           |
| verkeersbron | verkeersbron | Dimension | String |           |

{style="table-layout:auto"}

U kunt uw eigen geharmoniseerde velden toevoegen, bewerken of verwijderen boven op deze geharmoniseerde velden.

## Geharmoniseerde velden beheren

Een lijst van de beschikbare geharmoniseerde gebieden, in de interface van de Mix Modeler zien:

1. Selecteren ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** van de linkerspoorstaaf.

1. Selecteren **[!UICONTROL Fields]** in de bovenste balk. U ziet een tabel met de geharmoniseerde velden. Als er meer pagina&#39;s beschikbaar zijn, gebruikt u ![Pijl-links](../assets/icons/ChevronLeft.svg) of ![Pijl-rechts](../assets/icons/ChevronRight.svg) om **[!UICONTROL Page _x _van_x_]** om tussen pagina&#39;s van de lijst te bewegen.

   De tabelkolommen geven details over de geharmoniseerde velden

   | Kolomnaam | Details |
   | ---------------------- | ----------|
   | Veldnaam | De naam van het geharmoniseerde veld. |
   | Weergavenaam | De weergavenaam van het geharmoniseerde veld. Deze vertoningsnaam wordt gebruikt wanneer het bepalen van datasetregels, marketing touchpoint, en omzettingsdefinities. |
   | Categorie | Hiermee wordt opgegeven of een geharmoniseerd gegevensveld een [!UICONTROL Dimension], [!UICONTROL Metric] of [!UICONTROL Derived]. Een afgeleide categorie is een geharmoniseerd veld met behulp van een op cijfers gebaseerde definitie van formule. |
   | Gegevenstype | Hiermee wordt het gegevenstype ([!UICONTROL Number], [!UICONTROL String], [!UICONTROL Currency], [!UICONTROL Date time]). |
   | Aanmaakdatum | Datum en tijdstip waarop het geharmoniseerde veld wordt gecreëerd. |
   | Eigenaar | Geeft aan of een geharmoniseerd veld een standaardveld is ([!UICONTROL Global]), of wordt door u gedefinieerd ([!UICONTROL Client]). |
   | Laatst gewijzigd | Gegevens en tijdstip van de laatste wijziging van het geharmoniseerde veld. |
   | Formule | Geeft de formule aan voor een geharmoniseerd veld op basis van een afgeleide categorie. |

   {style="table-layout:auto"}

1. Om naar een specifiek geharmoniseerd gebied te zoeken, gebruik ![Zoeken](../assets/icons/Search.svg) **[!UICONTROL *Geharmoniseerd veld zoeken *]**.


### Een geharmoniseerd veld toevoegen

Om een geharmoniseerd veld toe te voegen, ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Fields]** interface in de Mix Modeler:

1. Selecteren ![Toevoegen](../assets/icons/AddCircle.svg) **[!UICONTROL Add field]**.

1. In de **[!UICONTROL Create]** dialoogvenster:

   1. Voer een **[!UICONTROL Field name]** bijvoorbeeld `region`.
   1. Voer een **[!UICONTROL Display name]** bijvoorbeeld `Region`.
   1. Selecteer een **[!UICONTROL Category]**: **[!UICONTROL Dimension]**, **[!UICONTROL Metric]** of **[!UICONTROL Derived]**.

      Wanneer u **[!UICONTROL Derived]** een **[!UICONTROL Formula]**. Om een geldige rekenkundige uitdrukking te bouwen, combineer één of meerdere metriek van **[!UICONTROL Insert Metric]** met een of meer operatoren **[!UICONTROL + - * / ( )]** . Bijvoorbeeld: `[orders]/[impressions]`

   1. Selecteer een **[!UICONTROL Data type]**.

      - **[!UICONTROL String]** of **[!UICONTROL Date time]**, als de geselecteerde categorie Dimension is.
      - **[!UICONTROL Number]** of **[!UICONTROL Currency]** als de geselecteerde categorie Metrisch of Afgeleid is.

   1. Selecteren **[!UICONTROL Submit]** het geharmoniseerde veld toe te voegen. Selecteren **[!UICONTROL Close]** het dialoogvenster sluiten zonder het geharmoniseerde veld toe te voegen.

      ![Een veld maken](../assets/create-field.png)


### Een geharmoniseerd veld bewerken

U kunt alleen geharmoniseerde velden bewerken die u eerder hebt gemaakt (eigenaar is client). U kunt een geharmoniseerd veld niet bewerken.

Als u een geharmoniseerd veld wilt bewerken, gaat u naar ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Fields]** interface in de Mix Modeler:

1. Selecteer het geharmoniseerde veld dat u wilt bewerken. Bijvoorbeeld: **[!UICONTROL Region]**.

1. In de **[!UICONTROL Edit harmonization values]** deelvenster, waarden wijzigen voor **[!UICONTROL Display name]**, **[!UICONTROL Category]**, en **[!UICONTROL Data type]**. Zie [Een geharmoniseerd veld toevoegen](#add-a-harmonized-field) voor meer informatie .

1. Selecteren **[!UICONTROL Submit]** de wijzigingen op het geharmoniseerde veld toe te passen.

   ![Een veld bewerken](../assets/edit-field.png)

### Een geharmoniseerd veld verwijderen

U kunt alleen geharmoniseerde velden verwijderen die u eerder hebt gemaakt (eigenaar is client). U kunt een geharmoniseerd veld niet verwijderen.

Als u een geharmoniseerd veld wilt verwijderen, gaat u naar ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Fields]** interface in de Mix Modeler:

1. Selecteer bijvoorbeeld het geharmoniseerde veld dat u wilt verwijderen **[!UICONTROL Region]**.

1. Selecteren ![Verwijderen](../assets/icons/Delete.svg) **[!UICONTROL Delete]** van de **[!UICONTROL Edit harmonization values]** linkerdeelvenster.

   >[!WARNING]
   >
   >   Het veld wordt onmiddellijk verwijderd.

