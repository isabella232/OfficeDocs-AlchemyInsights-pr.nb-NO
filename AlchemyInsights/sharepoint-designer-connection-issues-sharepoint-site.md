---
title: SharePoint Designer-tilkoblingsproblemer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508432"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer-tilkoblingsproblemer 

Hvis SharePoint Designer er problemer med tilkoblingen til SharePoint-områder, kan du prøve følgende vanlige løsninger.

Trinn 1: Kontroller at SharePoint Designer 2013 er oppdatert med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) og [2. August 2016 oppdatering for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Trinn 2: Fjerne lokal hurtigbuffer-filer:

1. Lukk SharePoint Designer 2013.

2. Fjerne alle filer som finnes i hver av følgende mapper på den lokale datamaskinen.

    - %APPDATA%\Microsoft\Web server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Åpne SharePoint Designer 2013, og Skriv inn kontoen på nytt for å se om det fungerer.

Trinn 3: [Aktiver moderne godkjenning for 2013 Office på Windows-enheter](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Trinn 4: Administratorer må **Tillate egendefinert skript** i administrasjonssenteret for SharePoint-innstillingene til å tillate SharePoint Designer-tilkobling. Se [Tillat eller forby egendefinert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for mer informasjon.


