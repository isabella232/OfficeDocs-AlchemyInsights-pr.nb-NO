---
title: SharePoint Tilkoblingsproblemer med designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942034"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Tilkoblingsproblemer med designer 

Hvis SharePoint Designer har tilkoblingsproblemer SharePoint nettsteder, kan du prøve følgende vanlige løsninger.

Trinn 1: Kontroller at SharePoint Designer 2013 er oppdatert med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) og oppdateringen for 2. august [2016 for SharePoint Designer 2013.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



Trinn 2: Fjern de lokale bufferfilene:

1. Lukk SharePoint Designer 2013.

2. Fjern alle filene i hver av følgende mapper på den lokale datamaskinen.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Åpne SharePoint Designer 2013, og skriv inn kontoen på nytt for å se om den fungerer.

Trinn 3: [Aktiver moderne godkjenning for Office 2013 på Windows enheter](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Trinn 4: Administratorer må  tillate egendefinert skript i innstillingene SharePoint for å tillate SharePoint Designer-tilkoblingen. Se [Tillate eller forhindre egendefinert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) hvis du vil ha mer informasjon.


