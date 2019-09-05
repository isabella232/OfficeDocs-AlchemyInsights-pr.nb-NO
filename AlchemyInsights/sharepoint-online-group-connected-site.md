---
title: Legge til en gruppe på et SharePoint-område
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750529"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Problemer når du oppretter eller grupperer tilkoblede områder i SharePoint Online

Det er et par vanlige problemer som oppstår når du oppretter eller gjenoppretter en gruppe koblet området.

 Hvis du har slettet en gruppe og det tilkoblede området og ønsker å opprette et annet område med samme NETTADRESSE, må du fjerne det forrige området permanent.

Last ned [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Hvis du vil ha mer informasjon om hvordan du kommer i gang med PowerShell, se [komme i gang med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Fjern området fra Slettede områder ved hjelp av [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell-cmdleten.

Hvis du oppretter et tilkoblet Gruppeområde og mottar en advarsel en annen gruppe med samme alias finnes allerede, kan du kontrollere de eksisterende gruppene fra [Office 365 fra administrasjonssenteret](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Du kan løse problemet ved å slette den eksisterende gruppen hvis den ikke lenger er nødvendig, eller opprette området med et annet alias tilordnet.

Det finnes ulike måter å opprette og bruke moderne grupper med SharePoint.

Du kan koble eksisterende områder til en Office 365-gruppe. Hvis du vil ha mer informasjon, kan [du se koble en Office 365-gruppe ved hjelp av SharePoint-ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Hvis du vil opprette et tilkoblet område for Office 365-gruppen, må du opprette et gruppeområde. Hvis du vil ha mer informasjon, kan du se [opprette et gruppeområde i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

