---
title: Begrense tilgang en sharepoint eller onedrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692774"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begrense tilgang en sharepoint eller onedrive

Det er mange måter å begrense tilgangen til SharePoint Online/OneDrive-tjenester på. Disse ulike tilgangsbegrensningsmetodene er skissert nedenfor. 

**Begrensning av tillatelser**

I SharePoint Online og OneDrive for Business begrenser vi tilgangen til elementer som områder, filer og mapper ved å bare gi tilgang til de gruppene/personene som skal ha tilgang.

- [Tilpasse tillatelser for en SharePoint-liste eller et SharePoint-bibliotek](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Tilpasse tillatelser for SharePoint-området](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Endre tillatelsene for en undermappe](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Kontrollere tilgang fra ikke-administrerte enheter](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Som SharePoint eller global administrator kan du blokkere eller begrense tilgangen til SharePoint- og OneDrive-innhold fra uadministrerte enheter (de som ikke er hybrid-AD som er koblet til eller kompatibel i Intune).

**Begrensning av nettverksplassering**

Som IT-administrator kan du kontrollere tilgangen til SharePoint- og OneDrive-ressurser basert på definerte nettverksplasseringer du stoler på. Dette kalles også stedsbasert policy. Hvis du vil ha mer informasjon, kan du se [Kontrollere tilgang til SharePoint Online- og OneDrive-data basert på nettverksplassering](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Begrensning av områdelås** 

I SharePoint Online har du muligheten til å låse en områdesamling, slik at ingen har tilgang. Dette er angitt via PowerShell og [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjelp av egenskapen [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState .

**Begrense brukere fra å opprette områder eller sekundære områder**

Som SharePoint-administrator eller Global administrator kan du la brukerne opprette og administrere sine egne SharePoint-områder, finne ut hva slags områder de kan opprette, og angi plasseringen av områdene. Hvis du vil ha mer informasjon, kan du se [Administrere oppretting av område i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

