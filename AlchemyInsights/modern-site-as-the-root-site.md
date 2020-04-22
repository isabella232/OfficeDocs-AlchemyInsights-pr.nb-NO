---
title: Moderne nettsted som rotstedet
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713800"
---
# <a name="modern-site-as-root-site"></a>Moderne nettsted som rotnettsted

Vi har begynt å rulle ut en ny funksjon som lar deg [bytte ditt klassiske nettsted rotnettsted med et moderne nettsted](https://docs.microsoft.com/sharepoint/modern-root-site). Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et område med et annet område mens du arkiverer det opprinnelige området. Tilgjengelig for både gruppeområde (ikke koblet til en gruppe) og kommunikasjonsområde.

>[!Important]
> Ikke slett det klassiske rotområdet for å opprette et moderne kommunikasjonsområde. Dette støttes ikke av Microsoft. Hvis du sletter rotområdet, blir alle SharePoint-områder i organisasjonen utilgjengelige for alle brukere, til du gjenoppretter området eller oppretter et nytt område på samme URL-adresse. Vi kommuniserer denne funksjonen via meldingssenteret. Du bør forvente at funksjonen skal slås på i leieren om kort tid.

## <a name="known-issues-with-swapping-sites"></a>Kjente problemer med bytte nettsteder
- Målområdet kan returnere en "ikke funnet" (HTTP 404) feil i en kort periode.
- Innholdet må søkes på nytt for å oppdatere søkeindeksen. Det er ikke nødvendig med manuelt trinn her, dette vil bli gjort automatisk.
- Alt som er avhengig av "statiske" koblinger (for eksempel Filsynkronisering og OneNote-filer), må korrigeres manuelt.
- Project Server-områder må kanskje valideres for å sikre at de fortsatt er tilknyttet på riktig måte. 
