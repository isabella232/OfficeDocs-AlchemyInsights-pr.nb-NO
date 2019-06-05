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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719490"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Opprette gruppe tilkoblede område i SharePoint Online

<p><strong>Det er noen vanlige problemer som kan oppstå når koblet område å opprette eller opprette en gruppe på nytt.&nbsp;</strong></p>  <p>1.Hvis du har slettet en gruppe, og det tilknyttede området og ønsker å opprette et annet område med samme URL-adresse, må du slette det forrige området.</p>  <ul>  <li>Last ned <a title="SPO administrasjonskonsoll" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO Management Shell</a> - For mer informasjon om å komme i gang med powershell, kan du se <a title="komme i gang med SharePoint Online Management Shell" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Komme i gang med SharePoint Online Management Shell</a>. <br /><br /></li>  <li>Fjerne webområdet fra slettet områder ved hjelp av den <a title="Fjern SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Fjern SPODeletedSite</a> powershell-cmdleten.</li>  </ul>  <p>Hvis du oppretter en gruppe sammenkoblede området og få en advarsel om <strong>en annen gruppe med samme aliaset allerede finnes</strong>, kan du se de eksisterende gruppene fra den <a title="Office 365 fra administrasjonssenteret" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 fra administrasjonssenteret</a>. Tilordnet til å løse problemet, sletter den eksisterende gruppen hvis det ikke lenger er nødvendig eller opprette området med et annet aliasnavn.&nbsp;</p>  <p><strong>Det finnes ulike måter å opprette og bruke moderne grupper med SharePoint.&nbsp;</strong></p>  <ol>  <li>Du kan koble eksisterende områder til en gruppe for Office 365. For mer informasjon, kan du se <a title="koble til en Office 365-gruppe ved hjelp av SharePoint bruker ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Koble en Office 365-gruppe ved hjelp av SharePoint bruker ineterface</a>.</li>  <li>Hvis du vil opprette en Office 365-gruppen koblet område, må du opprette et gruppeområde. For mer informasjon, kan du se <a title="oppretter et gruppeområde i SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Opprette et teamområde i SharePoint.</a></li>  </ol>

