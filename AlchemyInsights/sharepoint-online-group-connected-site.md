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
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582820"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemer når du oppretter et tilknyttet gruppeområde i SharePoint

1. Noen vanlige problemer oppstod når du oppretter eller oppretter et tilknyttet gruppeområde på nytt.
Hvis du har slettet en gruppe og det tilkoblede området og ønsker å opprette et annet nettsted med samme URL-adresse, må du fjerne det forrige nettstedet permanent.

   - Last ned [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Hvis du vil ha mer informasjon om hvordan du kommer i gang med Powershell, kan du se [Komme i gang med Administrasjonsskall for SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Fjern området fra slettede områder ved hjelp av cmdleten [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell . Powershell er nødvendig for å slette gruppeområder permanent.

1. Hvis du oppretter et tilknyttet gruppeområde og får en advarsel: **Det finnes allerede en annen gruppe med samme alias**, kontrollerer du de eksisterende gruppene fra administrasjonssenteret for Microsoft [365](https://admin.microsoft.com/AdminPortal/Home#/groups). Hvis du vil løse problemet, sletter du den eksisterende gruppen hvis den ikke lenger er nødvendig eller oppretter området med et annet alias som er tilordnet.

1. Det finnes forskjellige måter å opprette og bruke moderne grupper med SharePoint på.

   - Du kan koble eksisterende områder til en Microsoft 365-gruppe. Hvis du vil ha mer informasjon, kan du se [Koble til en Microsoft 365-gruppe ved hjelp av SharePoint-brukergrensesnittet](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Hvis du vil opprette et tilkoblet microsoft 365-gruppeområde, må du opprette et [gruppeområde](https://admin.microsoft.com/sharepoint).
