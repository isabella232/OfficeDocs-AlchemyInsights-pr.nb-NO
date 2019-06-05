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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716900"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer-tilkoblingsproblemer 

<p>Hvis SharePoint Designer er problemer med tilkoblingen til SharePoint-områder, prøv følgende vanlige løsninger.</p> <p><strong>Trinn 1:</strong> <strong>Er oppdatert må du kontrollere SharePoint Designer&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Oppdatering for SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Trinn 2:</strong> <strong>Fjern merket for lokal hurtigbuffer-filer</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Lukk SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">Gå til følgende mapper til å fjerne bufrede filer på den lokale datamaskinen.&nbsp;</li> <li style="font-weight: 400;">Klikk <strong>Start -&gt; kjører</strong> og slette alle filene som er funnet under hver av de under steder.&nbsp;<br /><br />%APPDATA%\Microsoft\Web server Extensions\Cache<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Åpne SharePoint Designer 2013, og Skriv inn kontoen på nytt for å se om det fungerer.</li> </ol> <p><strong>Trinn 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Aktiverer moderne godkjenning for 2013 Office på Windows-enheter</strong></a>&nbsp;</p> <p><strong>Trinn 4:</strong> <strong>Administratorer må tillate egendefinert skript til å tillate SharePoint Designer-tilkobling</strong>.</p> <p>For en detaljert fremgangsmåte, eksempler og vurderinger for å se <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">Tillat eller forby egendefinert skript</a>.&nbsp;</p>


