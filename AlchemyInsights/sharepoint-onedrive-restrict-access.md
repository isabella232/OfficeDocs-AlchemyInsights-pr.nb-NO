---
title: Begrense tilgang i SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700464"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begrense tilgang i SharePoint eller OneDrive

Det er mange måter å begrense tilgang til SharePoint Online/OneDrive-tjenester på. Disse forskjellige Begrensnings metodene for tilgang er angitt nedenfor. 

**Tillatelses begrensning**

I SharePoint Online og OneDrive for Business begrenser vi tilgang til elementer som nett steder, filer og mapper ved bare å gi tilgang til disse gruppene/enkelt personene som skal ha tilgang.

- [Tilpasse tillatelser for en SharePoint-liste eller et bibliotek](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Tilpasse tillatelser for SharePoint-område](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Endre tillatelsene for en under mappe](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Kontrollere tilgang fra ikke-administrerte enheter](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Som en SharePoint-eller global administrator kan du blokkere eller begrense tilgang til SharePoint og OneDrive-innhold fra ikke-administrerte enheter (som ikke er hybride AD-sammenføyd eller kompatible i Intune).

**Nettverks plasserings begrensning**

Som IT-administrator kan du kontrollere tilgang til SharePoint-og OneDrive-ressurser basert på definerte nettverks plasseringer du stoler på. Dette er også kjent som steds BAS ert policy. Hvis du vil ha mer informasjon, kan du se [kontrollere tilgang til SharePoint Online-og OneDrive-data basert på nettverks plassering](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Begrensninger for område lås** 

I SharePoint Online har du muligheten til å låse en nettsteds samling, så ingen har tilgang til den. Dette angis via PowerShell og [administrasjons grensesnittet for SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjelp av [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate-egenskapen.

**Begrense brukere fra å opprette områder eller sekundære områder**

Som en SharePoint-administrator eller global administrator kan du la brukerne opprette og administrere sine egne SharePoint-nettsteder, bestemme hvilke typer områder de kan opprette, og angi plasseringen av områdene. Hvis du vil ha mer informasjon, kan du se [Behandle område oppretting i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

