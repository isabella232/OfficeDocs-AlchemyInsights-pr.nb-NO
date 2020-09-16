---
title: Tilkoblings problemer i SharePoint Designer
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727180"
---
# <a name="sharepoint-designer-connection-issues"></a>Tilkoblings problemer i SharePoint Designer 

Hvis SharePoint Designer har tilkoblings problemer til SharePoint-nettsteder, kan du prøve følgende vanlige løsninger.

Trinn 1: Kontroller at SharePoint Designer 2013 er oppdatert med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) og [oppdateringen fra August 2, 2016 for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Trinn 2: Fjern de lokale hurtig buffer filene:

1. Lukk SharePoint Designer 2013.

2. På den lokale data maskinen fjerner du alle filene som ble funnet i hver av følgende mapper.

    - %APPDATA%\Microsoft\Web server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Åpne SharePoint Designer 2013, og skriv inn kontoen på nytt for å se om det fungerer.

Trinn 3: [Aktiver moderne godkjenning for Office 2013 på Windows-enheter](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Trinn 4: administratorer må **tillate egen definert skript** i innstillingene for administrasjons senteret for SharePoint for å tillate SharePoint Designer-tilkoblingen. Se [tillate eller hindre egen definert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for mer informasjon.


