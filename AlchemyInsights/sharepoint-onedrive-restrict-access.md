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
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093844"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begrense tilgang i SharePoint eller OneDrive

Det finnes mange måter å begrense tilgang til SharePoint Online/OneDrive tjenester på. Disse ulike tilgangsbegrensningsmetodene er beskrevet nedenfor. 

**Tillatelsesbegrensning**

I SharePoint Online og OneDrive for Business begrenser vi tilgangen til elementer som nettsteder, filer og mapper ved bare å gi tilgang til disse gruppene/personene som skal ha tilgang.

- [Tilpasse tillatelser for en SharePoint eller et bibliotek](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Tilpasse SharePoint områdetillatelser](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Endre tillatelsene for en undermappe](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Kontrollere tilgang fra ikke-administrerte enheter](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Som SharePoint eller global administrator kan du blokkere eller begrense tilgangen til SharePoint og OneDrive innhold fra uadministrerte enheter (de som ikke er hybrid AD sammenføyd eller kompatibel i Intune).

**Begrensninger for nettverksplassering**

Som IT-administrator kan du kontrollere tilgang til SharePoint og OneDrive ressurser basert på definerte nettverksplasseringer som du stoler på. Dette kalles også plasseringsbasert policy. Hvis du vil ha mer informasjon, kan du se Kontrollere tilgang til SharePoint Online og [OneDrive data basert på nettverksplassering](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Begrensning av nettstedslås** 

I SharePoint Online har du muligheten til å låse en nettstedssamling, slik at ingen har tilgang. Dette angis via PowerShell og SharePoint [Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjelp av egenskapen [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Begrense brukere fra å opprette områder eller sekundære nettsteder**

Som SharePoint administrator eller global administrator kan du la brukerne opprette og administrere sine egne SharePoint nettsteder, bestemme hva slags nettsteder de kan opprette, og angi plasseringen til nettstedene. Hvis du vil ha mer informasjon, kan du [se Administrere opprettelse](https://docs.microsoft.com/sharepoint/manage-site-creation) av nettsted i SharePoint Online

