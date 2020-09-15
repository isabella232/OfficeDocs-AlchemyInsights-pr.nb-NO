---
title: Bytte ut det klassiske rot området med et moderne nettsted
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691188"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Bytte ut det klassiske rot området med et moderne nettsted

Hvis miljøet ble konfigurert før 2019, kan du endre rot nettstedet til et moderne nettsted ved hjelp av Microsoft PowerShell:

- Hvis du har et annet nettsted du vil bruke som rot område, kan du erstatte [(bytte) det primære nettstedet](https://docs.microsoft.com/sharepoint/modern-root-site) med det. 
    - Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen til et nettsted med et annet område mens du arkiverer det opprinnelige nettstedet. Tilgjengelig for både gruppe nettsted (ikke koblet til en gruppe) og kommunikasjons område. 

- Flere funksjoner kommer snart til at du kan fortsette å bruke innholdet på området, men konvertere det eksisterende nettstedet til et kommunikasjons område. 
>[!Important]
>Disse funksjonene blir rullet ut gradvis. Fortsett å kontrollere meldings senteret for oppdateringer. 

## <a name="known-issues-with-swapping-sites"></a>Kjente problemer med å bytte nett steder

- Mål området kan returnere en feil melding om at det ikke ble funnet (HTTP 404) i løpet av en kort tids periode.
- Innhold må kravlesøkes for å oppdatere søke indeksen. Det er ikke nødvendig med et manuelt trinn – dette skjer automatisk.
- Alt som er avhengig av «statisk»-koblinger (for eksempel fil synkroniserings-og OneNote-filer), må korrigeres manuelt.
- Hvis kilde området var et organisasjons nyhets nettsted, oppdaterer du URL-adressen.Få en liste over alle organisasjonens nyhets områder.
- Project Server-områder må kanskje Valide res for å sikre at de fortsatt er riktige.
