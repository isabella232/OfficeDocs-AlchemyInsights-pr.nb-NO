---
title: Legge til en gruppe på et SharePoint nettsted
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 52f3bca7e92e9523838b5ad691f8accf0e7d0d03df79bb575f93b024e32cf3c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093719"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Vanlige problemer når du oppretter et gruppe tilkoblet nettsted i SharePoint

1. Hvis du har slettet en gruppe og det tilkoblede nettstedet og ønsker å opprette et annet nettsted med samme nettadresse, må du fjerne det forrige nettstedet permanent.

   - Last [ned skallet for SPO-administrasjon](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Hvis du vil ha mer informasjon om hvordan du kommer i gang med Powershell, kan du se Komme i gang med SharePoint [Online Management Shell](/powershell/module/sharepoint-online/remove-sposite).
   - Fjern nettstedet fra Slettede nettsteder ved hjelp [av Remove-SPODeletedSite](/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell-cmdleten. Powershell er nødvendig for å slette gruppenettsteder permanent.

1. Hvis du oppretter et gruppe tilkoblet nettsted og mottar en [advarsel:](https://admin.microsoft.com/AdminPortal/Home#/groups)En annen gruppe med samme **alias** finnes allerede, kontrollerer du de eksisterende gruppene fra Administrasjonssenter for Microsoft 365 . Hvis du vil løse problemet, sletter du den eksisterende gruppen hvis den ikke lenger er nødvendig eller oppretter nettstedet med et annet alias tilordnet.

1. Det finnes ulike måter å opprette og bruke moderne grupper på med SharePoint.

   - Du kan koble eksisterende nettsteder til en Microsoft 365 gruppe. Hvis du vil ha mer [informasjon, Koble til en Microsoft 365 brukergruppe ved hjelp av SharePoint brukergrensesnittet](/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Hvis du vil opprette Microsoft 365 et gruppe tilkoblet område, må du opprette et [gruppeområde](https://admin.microsoft.com/sharepoint).
