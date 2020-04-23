---
title: Forsinkelser i mottak av SharePoint- og OneDrive-varsler
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: fb7ab6e8139c46d89b1cae1ee0ab9b9a601c8b64
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742010"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Forsinkelser i mottak av SharePoint- og OneDrive-varsler

- Sjekk først søppelpost- eller søppelpostmappen i e-posten din.
- Hvis **alle varsler fra flere filer eller biblioteker er forsinket**, kan du gå til [instrumentbordet for tjenestetilstand](https://portal.office.com/adminportal/home?ref=/servicehealth) for å se etter eventuelle råd/hendelser som kan forekomme med SharePoint eller Exchange. Problemet kan være med SharePoint-varslingsfunksjonen eller forsinkelser i e-postmeldinger via Exchange. Vær også oppmerksom på om annen e-post blir levert – hvis ikke, er problemet sannsynligvis med Exchange-forsinkelser.
- Hvis **et individuelt varsel fra en bestemt fil eller et bestemt bibliotek ikke leveres**, prøver du å slette og opprette det på nytt. Se [Administrere, vise eller slette SharePoint-varsler](https://support.microsoft.com/office/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) for å opprette varselet på nytt.

> [!NOTE]
> - Varsler kan ikke sendes til en distribusjonsgruppe. Bare Sikkerhets- og O365-grupper støttes.
> - Du kan ikke tilpasse e-postmaler for varsel. Du må bruke Microsoft Flow eller SharePoint Designer Workflow for å oppnå disse.
