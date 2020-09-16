---
title: Legge til en gruppe på et SharePoint-område
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771217"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemer når du oppretter et tilkoblet nettsted i SharePoint

1. Noen vanlige problemer som oppstår når du oppretter eller gjen opprettet et gruppe tilkoblet nettsted.
Hvis du har slettet en gruppe og det tilkoblede nettstedet og vil opprette et annet nettsted med samme URL-adresse, må du fjerne det forrige nettstedet for godt.

   - Last ned [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Hvis du vil ha mer informasjon om hvordan du kommer i gang med PowerShell, kan du se [komme i gang med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Fjern nettstedet fra Slettede nett steder ved hjelp av PowerShell-cmdleten [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) . PowerShell kreves for å slette gruppe nett steder permanent.

1. Hvis du oppretter et gruppe tilkoblet nettsted og mottar en advarsel: **en annen gruppe med samme alias finnes allerede**, kan du kontrollere de eksisterende gruppene fra [administrasjons senteret for Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Hvis du vil løse problemet, sletter du den eksisterende gruppen hvis den ikke lenger er nødvendig, eller oppretter nettstedet med et annet alias tilordnet.

1. Det finnes ulike metoder for å opprette og bruke moderne grupper med SharePoint.

   - Du kan koble eksisterende områder til en Microsoft 365-gruppe. Hvis du vil ha mer informasjon, kan du se [Koble til en Microsoft 365-gruppe ved å bruke SharePoint-brukergrensesnittet](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Hvis du vil opprette et område i en Microsoft 365-gruppe som er tilkoblet, må du opprette et [gruppe område](https://admin.microsoft.com/sharepoint).
