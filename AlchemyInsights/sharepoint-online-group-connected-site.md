---
title: Legge til en gruppe på et SharePoint-område
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: b54457427ffa563b6a6323d85e1c8800191eca11
ms.sourcegitcommit: a98b25fa3cac9ebba983f4932881d774880aca93
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/13/2020
ms.locfileid: "44064402"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemer når du oppretter et gruppetilkoblet område i SharePoint

1. Det oppstod vanlige problemer når du oppretter eller oppretter et gruppetilkoblet område på nytt.
Hvis du har slettet en gruppe og det tilkoblede området og ønsker å opprette et annet nettsted med samme NETTADRESSE, må du fjerne det forrige nettstedet permanent.

   - Last ned [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Hvis du vil ha mer informasjon om hvordan du kommer i gang med Powershell, kan du se [Komme i gang med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Fjern området fra slettede områder ved hjelp av cmdleten [Fjern SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell . Powershell er nødvendig for å slette gruppeområder permanent.

1. Hvis du oppretter et gruppetilkoblet område og mottar en advarsel: **En annen gruppe med samme alias finnes allerede**, kan du kontrollere de eksisterende gruppene fra [administrasjonssenteret for Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Hvis du vil løse problemet ved å slette den eksisterende gruppen hvis den ikke lenger er nødvendig eller opprette området med et annet alias tilordnet.

1. Det finnes forskjellige måter å opprette og bruke moderne grupper på med SharePoint.

   - Du kan koble eksisterende områder til en Microsoft 365-gruppe. Hvis du vil ha mer informasjon, kan du se [Koble til en Microsoft 365-gruppe ved hjelp av SharePoint-brukergrensesnittet](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Hvis du vil opprette et tilkoblet Microsoft 365-gruppeområde, må du opprette et [gruppeområde](https://admin.microsoft.com/sharepoint).
