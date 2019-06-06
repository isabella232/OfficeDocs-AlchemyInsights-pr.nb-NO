---
title: Begrense tilgang i SharePoint eller OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735151"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begrense tilgang i SharePoint eller OneDrive

Det er mange måter å begrense tilgang til SharePoint Online/OneDrive tjenester. Disse ulike metoder for begrensningen beskrives nedenfor. 

Begrensning av tilgang

I SharePoint Online og OneDrive for bedrifter begrense vi tilgang til elementer, for eksempel områder, filer og mapper ved å bare gi tilgang til de grupper/personene som skal ha tilgang.

[Tilpasse tillatelser for en SharePoint-liste eller et bibliotek](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[Tilpasse SharePoint-områdetillatelser](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[Endre tillatelsene for en undermappe](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[Kontrollere tilgang fra ikke-administrerte enheter](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

SharePoint eller global admin i Office 365, kan du sperre eller begrense tilgang til innhold i SharePoint og OneDrive fra ikke-administrerte enheter (de ikke hybrid Annonse sammenføyde eller kompatibel i Intune).

Nettverk plasseringen begrensning

Som en IT-administrator, kan du styre tilgang til SharePoint- og OneDrive ressurser basert på definerte nettverksplasseringer som du stoler på. Dette er også kjent som sted-basert policy. Hvis du vil ha mer informasjon, se [kontrollere tilgang til SharePoint Online og OneDrive data basert på nettverksplasseringen](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)

Lås områdebegrensningen 

Du har muligheten til å låse en områdesamling, slik at ingen har tilgang til i SharePoint Online. Dette angis via PowerShell og [SharePoint Online Management Shell](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjelp av [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState-egenskapen.

Hindre brukere i å opprette områder eller sekundære områder

Du kan la brukerne opprette og administrere sine egne SharePoint-områder, finne ut hvilke områder de kan opprette, som en SharePoint-administrator eller en global administrator for Office 365 og angi plasseringen av områdene. Hvis du vil ha mer informasjon, kan du se [Behandle områdeoppretting i SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)

