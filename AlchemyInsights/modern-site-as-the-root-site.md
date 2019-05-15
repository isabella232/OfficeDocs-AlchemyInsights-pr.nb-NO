---
title: Moderne området som det primære området
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057747"
---
# <a name="modern-site-as-root-site"></a>Moderne område som rotområde

[Utgivelsen av mål](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) kunder kan nå aktivere moderne kommunikasjon området opplevelse på klassisk rotområdet for sine SharePoint leier.

Denne funksjonen kan aktiveres ved å kjøre en enkel PowerShell-cmdleten. For vellykket kjøring av PowerShell-kommandoer må det primære området en ny kommunikasjon-hjemmesiden. Detaljer om kravene til PowerShell-cmdlet og funksjonen er tilgjengelig i artikkelen [Aktivere SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps). 

Vi vil bli gradvis rullende dette ut, av som standard til angitt versjon kunder i tidlig mai 2019, og Rull ut vil være tilgjengelig over hele verden på slutten av juni 2019. Fortsette å referere til [Meldingssentral](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for andre nye funksjoner med moderne. 

**Viktig**: ikke Slett klassisk rotområdet for å opprette et område for moderne kommunikasjon. Dette støttes ikke av Microsoft. Sletter det primære området, blir alle SharePoint-områder i organisasjonen utilgjengelig for alle brukere, før du kan gjenopprette området eller opprette et nytt område på den samme URL-adressen. 
 
 