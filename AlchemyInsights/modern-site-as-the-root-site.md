---
title: Moderne nettsted som rotnettsted
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327611"
---
# <a name="modern-site-as-root-site"></a>Moderne nettsted som rotnettsted

Vi har begynt å rulle ut en ny funksjon som lar deg bytte det klassiske nettstedets [rotområde med et moderne nettsted.](https://docs.microsoft.com/sharepoint/modern-root-site) Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et nettsted med et annet nettsted mens du arkiverer det opprinnelige nettstedet. Tilgjengelig for både gruppenettsted (ikke koblet til en gruppe) og kommunikasjonsnettstedet.

**Viktig:** Ikke slett det klassiske rotnettstedet for å opprette et moderne kommunikasjonsnettsted. Dette støttes ikke av Microsoft. Hvis du sletter rotnettstedet, blir alle SharePoint i organisasjonen utilgjengelige for alle brukere, helt til du gjenoppretter nettstedet eller oppretter et nytt nettsted på samme nettadresse. Vi kommuniserer denne funksjonen via meldingssenteret. Du bør forvente at funksjonen blir slått på i leieren om kort tid.

## <a name="known-issues-with-swapping-sites"></a>Kjente problemer med å bytte nettsteder
- Målnettstedet kan returnere feilmeldingen «Finner ikke» (HTTP 404) i en kort tidsperiode.
- Innhold må på nytt for å oppdatere søkeindeksen. Det er ingen manuelle trinn som kreves her. Dette gjøres automatisk.
- Alt som er avhengig av statiske koblinger (for eksempel filsynkronisering OneNote filer), må korrigeres manuelt.
- Project Servernettsteder må kanskje valideres for å sikre at de fortsatt er tilknyttet riktig. 
