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
ms.openlocfilehash: 260048db6c439183da8e0bb0c2dfa3c7475fca79
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269385"
---
# <a name="modern-site-as-root-site"></a>Moderne område som rotområde

Vi har begynt å utrullingen en ny funksjon som lar deg bytte rotområdet klassisk område med et moderne område. Bruk [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et område med et annet område under arkivering av det opprinnelige området. Tilgjengelig for både Team (ikke koblet til en gruppe) og kommunikasjon-området. 

>[!Important]
> Ikke Slett klassisk rotområdet for å opprette et område for moderne kommunikasjon. Dette støttes ikke av Microsoft. Sletter det primære området, blir alle SharePoint-områder i organisasjonen utilgjengelig for alle brukere, før du kan gjenopprette området eller opprette et nytt område på den samme URL-adressen. Vi skal kommunisere denne funksjonen via Meldingssentret. Du bør forvente at funksjonen skal være aktivert i din leier kort tid.

## <a name="known-issues-with-swapping-sites"></a>Kjente problemer med bytte områder
- Målområdet kan returnere en "not found" (HTTP 404)-feil for en kort tidsperiode.
- Innhold må være kravlesøkt på nytt for å oppdatere søkeindeksen. Det er ingen manuelle trinn nødvendig her, dette vil bli gjort automatisk.
- Alt avhengig av "statisk" koblinger (for eksempel filsynkronisering og OneNote-filer) må korrigeres manuelt.
- Project Server-områder må kanskje valideres for å sikre at de er fortsatt tilknyttet på riktig måte. 
