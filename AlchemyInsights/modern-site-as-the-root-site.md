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
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000401"
---
# <a name="modern-site-as-root-site"></a>Moderne nettsted som rotnettsted

Vi har begynt å rulle ut en ny funksjon som lar deg bytte det klassiske nettstedets [rotområde med et moderne nettsted.](https://docs.microsoft.com/sharepoint/modern-root-site) Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et nettsted med et annet nettsted mens du arkiverer det opprinnelige nettstedet. Tilgjengelig for både gruppenettsted (ikke koblet til en gruppe) og kommunikasjonsnettstedet.

>[!Important]
> Ikke slett det klassiske rotnettstedet for å opprette et moderne kommunikasjonsnettsted. Dette støttes ikke av Microsoft. Hvis du sletter rotnettstedet, blir alle SharePoint i organisasjonen utilgjengelige for alle brukere, helt til du gjenoppretter nettstedet eller oppretter et nytt nettsted på samme nettadresse. Vi kommuniserer denne funksjonen via meldingssenteret. Du bør forvente at funksjonen blir slått på i leieren om kort tid.

## <a name="known-issues-with-swapping-sites"></a>Kjente problemer med å bytte nettsteder
- Målnettstedet kan returnere feilmeldingen «Finner ikke» (HTTP 404) i en kort tidsperiode.
- Innhold må på nytt for å oppdatere søkeindeksen. Det er ingen manuelle trinn som kreves her. Dette gjøres automatisk.
- Alt som er avhengig av statiske koblinger (for eksempel filsynkronisering OneNote filer), må korrigeres manuelt.
- Project Servernettsteder må kanskje valideres for å sikre at de fortsatt er tilknyttet riktig. 
