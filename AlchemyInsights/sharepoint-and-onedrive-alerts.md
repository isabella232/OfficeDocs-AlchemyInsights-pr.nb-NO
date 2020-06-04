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
ms.openlocfilehash: 7f1033cec3abec782d1eee3b32128c4c60778913
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563519"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Forsinkelser i mottak av SharePoint- og OneDrive-varsler

- Først sjekk søppelpost- eller søppelpostmappen i e-posten din.
- Hvis **alle varsler fra flere filer eller biblioteker er forsinket,** kan du gå til instrumentbordet for [tjenestetilstand](https://portal.office.com/adminportal/home?ref=/servicehealth) for å se etter råd/hendelser som kan oppstå med SharePoint eller Exchange. Problemet kan være med SharePoint-varslingsfunksjonen eller forsinkelser i e-postmeldinger via Exchange. Vær også oppmerksom på om andre e-postmeldinger leveres – hvis ikke, er problemet sannsynligvis med Exchange-forsinkelser.
- Hvis **et enkeltvarsel fra en bestemt fil eller et bestemt bibliotek ikke leveres,** kan du prøve å slette og opprette det på nytt. Se [Behandle, vise eller slette SharePoint-varsler](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) for å opprette varselet på nytt.

> [!NOTE]
> - Varsler kan ikke sendes til en distribusjonsgruppe. Bare sikkerhet- og O365-grupper støttes.
> - Du kan ikke tilpasse e-postmaler for varsel. Du må bruke Microsoft Flow eller SharePoint Designer Workflow for å oppnå disse.
