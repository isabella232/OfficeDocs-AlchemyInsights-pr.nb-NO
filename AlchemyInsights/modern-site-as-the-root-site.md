---
title: Moderne området som det primære området
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: d5ea73c967013822854dbd408d4628d991c90378
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620768"
---
# <a name="modern-site-as-root-site"></a>Moderne område som rotområde

Vi har begynt å utrullingen en ny funksjon som lar deg bytte rotområdet klassisk område med et moderne område. Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et område med et annet område under arkivering av det opprinnelige området. Tilgjengelig for både Team (ikke koblet til en gruppe) og kommunikasjon-området. 

>[!Important]
> Ikke Slett klassisk rotområdet for å opprette et område for moderne kommunikasjon. Dette støttes ikke av Microsoft. Sletter det primære området, blir alle SharePoint-områder i organisasjonen utilgjengelig for alle brukere, før du kan gjenopprette området eller opprette et nytt område på den samme URL-adressen. Vi skal kommunisere denne funksjonen via Meldingssentret. Du bør forvente at funksjonen skal være aktivert i din leier kort tid.

## <a name="known-issues-with-swapping-sites"></a>Kjente problemer med bytte områder
- Målområdet kan returnere en "not found" (HTTP 404)-feil for en kort tidsperiode.
- Innhold må være kravlesøkt på nytt for å oppdatere søkeindeksen. Det er ingen manuelle trinn nødvendig her, dette vil bli gjort automatisk.
- Alt avhengig av "statisk" koblinger (for eksempel filsynkronisering og OneNote-filer) må korrigeres manuelt.
- Project Server-områder må kanskje valideres for å sikre at de er fortsatt tilknyttet på riktig måte. 
