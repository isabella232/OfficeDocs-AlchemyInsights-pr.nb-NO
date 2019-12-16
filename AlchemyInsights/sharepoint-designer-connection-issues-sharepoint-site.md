---
title: Problemer med tilkobling til SharePoint Designer
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
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051722"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemer med tilkobling til SharePoint Designer 

Hvis SharePoint Designer har tilkoblingsproblemer på SharePoint-områder, kan du prøve følgende vanlige løsninger.

Trinn 1: Kontroller at SharePoint Designer 2013 er oppdatert med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) og [August 2, 2016 oppdatering for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Trinn 2: Tøm de lokale hurtigbuffer filene:

1. Lukk SharePoint Designer-2013.

2. På den lokale datamaskinen, kan du fjerne alle filer som finnes i hver av følgende mapper.

    - %APPDATA%\Microsoft\Web server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Åpne SharePoint Designer 2013, og skriv inn kontoen på nytt for å se om den fungerer.

Trinn 3: [Aktiver moderne godkjenning for Office 2013 på Windows-enheter](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Trinn 4: administratorer må **tillate egendefinert skript** i innstillingene for SharePoint Administrasjonssenter for å tillate SharePoint Designer-tilkobling. Se [tillate eller forhindre egendefinert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for mer informasjon.


