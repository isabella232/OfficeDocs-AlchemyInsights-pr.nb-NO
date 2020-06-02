---
title: Tilkoblingsproblemer for SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511553"
---
# <a name="sharepoint-designer-connection-issues"></a>Tilkoblingsproblemer for SharePoint Designer 

Hvis SharePoint Designer har tilkoblingsproblemer til SharePoint-områder, kan du prøve følgende vanlige løsninger.

Trinn 1: Kontroller at SharePoint Designer 2013 er oppdatert med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) og [2 August 2016 oppdatering for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Trinn 2: Tøm de lokale bufferfilene:

1. Lukk SharePoint Designer 2013.

2. Fjern alle filene i hver av følgende mapper på den lokale datamaskinen.

    - %APPDATA%\Microsoft\Web-servertillegg\hurtigbuffer
    - %APPDATA%Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Åpne SharePoint Designer 2013, og skriv inn kontoen på nytt for å se om den fungerer.

Trinn 3: [Aktiver moderne godkjenning for Office-2013 på Windows-enheter](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Trinn 4: Administratorer må **tillate egendefinert skript** i administrasjonssenteret for SharePoint for å tillate SharePoint Designer-tilkoblingen. Se [Tillate eller forhindre egendefinert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) hvis du vil ha mer informasjon.


