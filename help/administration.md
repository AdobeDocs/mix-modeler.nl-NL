---
title: Beheer
description: Leer hoe u Mix Modeler kunt beheren.
feature: Administration
source-git-commit: c145754ecd6a6d8f5aab333ced739c4053aeaae5
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 7%

---


# Beheer

Gebruik de [Adobe Admin Console](https://helpx.adobe.com/nl/enterprise/using/admin-console.html) het beheer van producten en gebruikers van Mixxen Modeler.

Mix Modeler werkt alleen correct als u de juiste machtigingen instelt.

In de gebruikersinterface van Adobe Experience Cloud:

1. Selecteren **[!UICONTROL Permissions]** van de linkerspoorstaaf, onder **[!UICONTROL ADMINISTRATION]**.

1. Selecteren ![Persoon](assets/icons/User.svg) **[!UICONTROL Roles]** in het linkerdeelvenster.

1. Selecteer een bestaande rol of maak een rol met **[!UICONTROL Create role]**. Als u een bestaande rol selecteert, selecteert u ![Bewerken](assets/icons/Edit.svg) **[!UICONTROL Edit]** om de machtigingen voor de rol te bewerken. Zie [Rollen beheren](https://helpx.adobe.com/nl/enterprise/using/admin-console.html) voor meer informatie .

1. Zorg ervoor dat u de volgende machtigingen voor de rol selecteert:

   * **[!UICONTROL Sandboxes]**: Selecteer ten minste één sandbox.

   * **[!UICONTROL Data Management]**: zorg dat u de opties selecteert **[!UICONTROL View Datasets]** en **[!UICONTROL Manage Datasets]**.

   * **[!UICONTROL Data Modeling]**: zorg dat u de opties selecteert **[!UICONTROL Manage Schemas]** en **[!UICONTROL View Schemas]**.

   * **[!UICONTROL Destinations]**: zorg dat u **[!UICONTROL Manage and Activate Dataset Destination]**, **[!UICONTROL Destination Authoring]**, **[!UICONTROL Activate Destinations]** en **[!UICONTROL View Destinations]**.

   * **[!UICONTROL Data Ingestion]**: zorg dat u **[!UICONTROL View Sources]** en **[!UICONTROL Manage Sources]**.

   <!--
    * **[!UICONTROL Data Governance]**: ensure you select **[!UICONTROL View User Activity Log]** and **[!UICONTROL View Data Usage Policies]**.
    -->

   De machtigingen die voor de rol zijn ingesteld, moeten er als volgt uitzien:

   ![Machtigingen](assets/permissions.png)

   <!--![Permissions](assets/permissions-including-privacy.png)-->

   Selecteren **[!UICONTROL Save]** om de machtigingen op te slaan.

1. In **[!UICONTROL Details]** binnen **[!UICONTROL Role]** de passende **[!UICONTROL Users]** en/of **[!UICONTROL User groups]** om gebruikers toegang tot Mix Modeler te verlenen.
