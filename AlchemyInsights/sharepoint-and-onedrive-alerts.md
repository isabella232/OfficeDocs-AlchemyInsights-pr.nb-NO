---
title: Forsinkelser i mottak av SharePoint-og OneDrive-varsler
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727252"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Forsinkelser i mottak av SharePoint-og OneDrive-varsler

- Kontroller først mappen søppel post eller søppel post i e-posten.
- Hvis **alle varsler fra flere filer eller biblioteker er forsinket**, kan du gå til [instrument bordet for tjeneste tilstand](https://portal.office.com/adminportal/home?ref=/servicehealth) for å se etter rådgivere/hendelser som kan oppstå med SharePoint eller Exchange. Problemet kan være med Varsels funksjonen for SharePoint og forsinkelser i e-postmeldinger gjennom Exchange. Vær også oppmerksom på om andre e-postmeldinger leveres – hvis ikke, er problemet sannsynligvis i Exchange-forsinkelser.
- Hvis **et enkelt varsel fra en bestemt fil eller bibliotek ikke leveres**, kan du prøve å slette og opprette det på nytt. Se [Behandle, vise eller slette SharePoint-varsler](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) for å opprette varselet på nytt.

> [!NOTE]
> - Varsler kan ikke sendes til en distribusjons gruppe. Bare sikkerhets-og O365-grupper støttes.
> - Du kan ikke tilpasse e-postmaler for varsler. Du må bruke arbeids flyten i Microsoft flyt eller SharePoint Designer for å få dem.
