---
title: Beheer
description: Leer hoe u Mix Modeler kunt beheren.
feature: Administration
exl-id: 76d6d15d-a838-4ee2-9929-e55ea8946b80
source-git-commit: 51a4bc6557422a281fa03d49877cb378d14314e2
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 2%

---

# Beheer

Gebruik de [Adobe Admin Console](https://helpx.adobe.com/nl/enterprise/using/admin-console.html) het beheer van producten en gebruikers van Mixxen Modeler.

Mix Modeler werkt alleen correct als u de juiste machtigingen instelt.

In de gebruikersinterface van Adobe Experience Cloud:

1. Selecteren **[!UICONTROL Permissions]** van de linkerspoorstaaf, onder **[!UICONTROL ADMINISTRATION]**.

1. Selecteren ![Persoon](assets/icons/User.svg) **[!UICONTROL Roles]** in het linkerdeelvenster.

1. Selecteer een bestaande rol of maak een rol met **[!UICONTROL Create role]** (bijvoorbeeld **Mix Modeler**). Als u een bestaande rol selecteert, selecteert u ![Bewerken](assets/icons/Edit.svg) **[!UICONTROL Edit]** om de machtigingen voor de rol te bewerken. Zie [Rollen beheren](https://helpx.adobe.com/nl/enterprise/using/admin-console.html) voor meer informatie .

1. Controleer of u een of meer sandboxen voor de rol hebt geselecteerd.

1. Voeg de **Adobe Mix Modeler** bron aan de lijst van middelen voor de rol.

1. Zorg ervoor dat u de juiste **[!UICONTROL Adobe Mix Modeler]** machtigingen voor de rol die u configureert. U kunt een of meer van de volgende rollen selecteren:

   - **[!UICONTROL View Adobe Mix Modeler Harmonized Data]**
   - **[!UICONTROL Manage Adobe Mix Modeler Harmonized Data]**
   - **[!UICONTROL View Adobe Mix Modeler Models Configuration]**
   - **[!UICONTROL Manage Adobe Mix Modeler Models Configuration]**
   - **[!UICONTROL View Adobe Mix Modeler Plans Configuration]**
   - **[!UICONTROL Manage Adobe Mix Modeler Plans Configuration]**

     ![Mix Modeler RBAC](assets/mix-modeler-rbac.png)


1. Zorg ervoor dat u aanvullende machtigingen voor de rol selecteert. Als u bijvoorbeeld gegevenssets en schema&#39;s wilt weergeven of beheren, selecteert u:

   - **[!UICONTROL Data Management]**: selecteer de relevante opties: **[!UICONTROL View Datasets]** of **[!UICONTROL Manage Datasets]**.

   - **[!UICONTROL Data Modeling]**: selecteer de relevante opties: **[!UICONTROL Manage Schemas]** of **[!UICONTROL View Schemas]**.

   <!--
    * **[!UICONTROL Data Governance]**: ensure you select **[!UICONTROL View User Activity Log]** and **[!UICONTROL View Data Usage Policies]**.
    -->

   <!--![Permissions](assets/permissions-including-privacy.png)-->

   Selecteren **[!UICONTROL Save]** om de machtigingen op te slaan.

1. In **[!UICONTROL Details]** binnen **[!UICONTROL Role]** de passende **[!UICONTROL Users]** of **[!UICONTROL User groups]** om gebruikers toegang tot Mix Modeler te verlenen.
