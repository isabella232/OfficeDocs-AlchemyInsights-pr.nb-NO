---
title: Begrens tilgang i SharePoint eller OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750673"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begrens tilgang i SharePoint eller OneDrive

Det er mange måter å begrense tilgangen til SharePoint Online/OneDrive tjenester. Disse ulike tilgangs Begrensnings metodene er beskrevet nedenfor. 

**Tillatelse begrensning**

I SharePoint Online og OneDrive for Business, begrenser vi tilgang til elementer som områder, filer og mapper ved bare å gi tilgang til disse gruppene/enkeltpersoner som skal ha tilgang.

- [Tilpasse tillatelser for SharePoint-lister eller-biblioteker](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Tilpasse tillatelser for SharePoint-område](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Endre tillatelsene for en undermappe](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Kontrollere tilgang fra ikke-administrerte enheter](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Som en SharePoint eller global administrator i Office 365, kan du blokkere eller begrense tilgangen til SharePoint-og OneDrive-innhold fra ikke-administrerte enheter (de som ikke er kombinert AD eller kompatibel i Intune).

**Begrensning av nettverksplassering**

Som IT-administrator kan du styre tilgangen til SharePoint-og OneDrive-ressurser basert på definerte nettverksplasseringer du stoler på. Dette er også kjent som stedsbasert policy. Hvis du vil ha mer informasjon, kan du se [kontrollere tilgangen til SharePoint Online og OneDrive-data basert på nettverksplassering](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Begrensning av område lås** 

I SharePoint Online har du muligheten til å låse en områdesamling, slik at ingen har tilgang til dem. Dette angis via PowerShell og [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjelp av [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate-egenskapen.

**Hindre brukere i å opprette områder eller sekundære områder**

Som en SharePoint-administrator eller en global administrator for Office 365 kan du la brukerne opprette og administrere sine egne SharePoint-områder, bestemme hva slags områder de kan opprette og angi plasseringen av områdene. Hvis du vil ha mer informasjon, kan du se [Behandle områdeoppretting i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

