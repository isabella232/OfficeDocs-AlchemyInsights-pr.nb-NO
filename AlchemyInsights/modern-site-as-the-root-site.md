---
title: Moderne område som roten området
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
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753913"
---
# <a name="modern-site-as-root-site"></a>Moderne nettsted som root nettsted

Vi har begynt å utrulling en ny funksjon som vil tillate deg å [bytte din klassiske nettstedet root nettsted med et moderne nettsted](https://docs.microsoft.com/sharepoint/modern-root-site). Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et område med et annet område under arkivering av det opprinnelige området. Tilgjengelig for begge gruppeområder (ikke koblet til en gruppe) og kommunikasjons område.

>[!Important]
> Ikke slett det klassiske rotområdet for å opprette et moderne kommunikasjons nettsted. Dette støttes ikke av Microsoft. Hvis du sletter rotområdet, vil alle SharePoint-områder i organisasjonen være utilgjengelige for alle brukere, helt til du gjenoppretter området eller oppretter et nytt område på samme URL-adresse. Vi kommuniserer denne funksjonen via meldingssentralen. Du bør forvente at funksjonen skal være slått på i leietaker kort tid.

## <a name="known-issues-with-swapping-sites"></a>Kjente problemer ved bytte av områder
- Målområdet kan returnere en feilmelding av typen "ikke funnet" (HTTP 404) for en kort tidsperiode.
- Innhold må være recrawled for å oppdatere søkeindeksen. Det er ingen manuelle trinn som kreves her, dette vil bli gjort automatisk.
- Alt som er avhengig av "statiske" koblinger (for eksempel File Sync og OneNote-filer) må rettes manuelt.
- Project Server-områder må kanskje valideres for å sikre at de fortsatt er riktig tilknyttet. 
