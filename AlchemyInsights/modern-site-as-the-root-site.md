---
title: Moderne nettsted som rot område
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
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666879"
---
# <a name="modern-site-as-root-site"></a>Moderne nettsted som rot område

Vi har begynt å fremheve en ny funksjon som gjør at du kan [bytte til rot området for det klassiske nettstedet med et moderne nettsted](https://docs.microsoft.com/sharepoint/modern-root-site). Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen til et nettsted med et annet område mens du arkiverer det opprinnelige nettstedet. Tilgjengelig for både gruppe nettsted (ikke koblet til en gruppe) og kommunikasjons område.

>[!Important]
> Ikke slett det klassiske rot nettstedet for å opprette et moderne kommunikasjons område. Dette støttes ikke av Microsoft. Hvis du sletter rot området, blir alle SharePoint-nettsteder i organisasjonen utilgjengelig for alle brukere, til du gjenoppretter nettstedet eller oppretter et nytt nettsted på samme nett adresse. Vi vil kommunisere denne funksjonen via meldings senteret. Du bør også forvente at funksjonen skal slås på i leier snart.

## <a name="known-issues-with-swapping-sites"></a>Kjente problemer med å bytte nett steder
- Mål området kan returnere en feil melding om at det ikke ble funnet (HTTP 404) i løpet av en kort tids periode.
- Innhold må kravlesøkes for å oppdatere søke indeksen. Det er ikke nødvendig med manuelt trinn, dette gjøres automatisk.
- Alt som er avhengig av «statisk»-koblinger (for eksempel fil synkroniserings-og OneNote-filer), må korrigeres manuelt.
- Project Server-områder må kanskje Valide res for å sikre at de fortsatt er riktige. 
