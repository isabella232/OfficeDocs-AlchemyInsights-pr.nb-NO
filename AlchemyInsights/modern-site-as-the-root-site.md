---
title: Moderne området som det primære området
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232724"
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
