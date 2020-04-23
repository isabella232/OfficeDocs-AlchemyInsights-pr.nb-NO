---
title: Bytt ditt klassiske rotnettsted med et moderne nettsted
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741553"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Bytt ditt klassiske rotnettsted med et moderne nettsted

Hvis miljøet ble konfigurert før april 2019, kan du endre rotområdet til et moderne område ved hjelp av Microsoft PowerShell:

- Hvis du har et annet nettsted som du vil bruke som rotområde, kan du erstatte [(bytte) rotområdet](https://docs.microsoft.com/sharepoint/modern-root-site) med det. 
    - Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et område med et annet område mens du arkiverer det opprinnelige området. Tilgjengelig for både gruppeområde (ikke koblet til en gruppe) og kommunikasjonsområde. 

- Ytterligere funksjoner vil bli introdusert snart som vil tillate deg å fortsette å bruke innholdet på nettstedet, men konvertere det eksisterende området til et kommunikasjonsområde. 
>[!Important]
>Disse egenskapene vil bli rullet ut gradvis. Fortsett å se etter oppdateringer i meldingssenteret. 

## <a name="known-issues-with-swapping-sites"></a>Kjente problemer med bytte nettsteder

- Målområdet kan returnere en "ikke funnet" (HTTP 404) feil i en kort periode.
- Innholdet må søkes på nytt for å oppdatere søkeindeksen. Det er ikke nødvendig med manuelt trinn - dette vil bli gjort automatisk.
- Alt som er avhengig av "statiske" koblinger (for eksempel Filsynkronisering og OneNote-filer), må korrigeres manuelt.
- Hvis kildeområdet var et organisasjonsnyhetsnettsted, oppdaterer du URL-adressen.Få en liste over alle organisatoriske nyhetssider.
- Project Server-områder må kanskje valideres for å sikre at de fortsatt er tilknyttet på riktig måte.
