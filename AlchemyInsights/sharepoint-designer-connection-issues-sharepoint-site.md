---
title: Tillatelsesnivåer for SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760701"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer-tilkoblingsproblemer 

Hvis SharePoint Designer er problemer med tilkoblingen til SharePoint-områder, prøv følgende vanlige løsninger.

Trinn 1: Kontroller SharePoint Designer er oppdatert.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Oppdatering for SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Trinn 2: Fjerne lokal hurtigbuffer-filer

- Lukk SharePoint Designer 2013.

- Gå til følgende mapper til å fjerne bufrede filer på den lokale datamaskinen.

- Klikk Start, Kjør, og Slett alle filer som er funnet under hver av de under steder.

%APPDATA%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Åpne SharePoint Designer 2013, og Skriv inn kontoen på nytt for å se om det fungerer.

Trinn 3: [Aktiver moderne godkjenning for 2013 Office på Windows-enheter](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Trinn 4: Administratorer må tillate egendefinert skript til å tillate SharePoint Designer-tilkobling.

For en detaljert fremgangsmåte, eksempler og vurderinger for å se [Tillat eller forby egendefinert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

