---
title: Legge til en gruppe på et SharePoint-område
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507856"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Problemer når du oppretter eller en gruppe koblet områder i SharePoint Online

Det er noen vanlige problemer som kan oppstå når koblet område å opprette eller opprette en gruppe på nytt.

 Hvis du har slettet en gruppe, og det tilknyttede området og ønsker å opprette et annet område med samme URL-adresse, må du slette det forrige området.

Last ned [SPO administrasjonskonsoll](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 For mer informasjon om å komme i gang med powershell, kan du se [Komme i gang med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Fjerne webområdet fra slettet områder ved hjelp av [Fjern SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell-cmdleten.

Hvis du oppretter en gruppe sammenkoblede området og få en advarsel om det finnes allerede en annen gruppe med samme alias, må du kontrollere eksisterende grupper fra [Office 365 fra administrasjonssenteret](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Tilordnet til å løse problemet, sletter den eksisterende gruppen hvis det ikke lenger er nødvendig eller opprette området med et annet aliasnavn.

Det finnes ulike måter å opprette og bruke moderne grupper med SharePoint.

Du kan koble eksisterende områder til en gruppe for Office 365. For mer informasjon, se [koble til en Office 365-gruppe ved hjelp av SharePoint bruker ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Hvis du vil opprette en Office 365-gruppen koblet område, må du opprette et gruppeområde. For mer informasjon, kan du se [opprette et teamområde i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

