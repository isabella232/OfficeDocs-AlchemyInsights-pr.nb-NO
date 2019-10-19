---
title: Bytt ut ditt klassiske rotområde med et moderne nettsted
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36749269"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Bytt ut ditt klassiske rotområde med et moderne nettsted

Hvis miljøet ble konfigurert før april 2019, kan du endre det primære området til et moderne område ved hjelp av Microsoft PowerShell:

- Hvis du har et annet område som du vil bruke som ditt primære webområde, kan du erstatte [(bytte) det primære området](https://docs.microsoft.com/sharepoint/modern-root-site) med det. 
    - Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et område med et annet område under arkivering av det opprinnelige området. Tilgjengelig for begge gruppeområder (ikke koblet til en gruppe) og kommunikasjons område. 

- Flere funksjoner vil bli innført snart som gjør at du kan fortsette å bruke innholdet på området, men konvertere det eksisterende området til et område for kommunikasjon. 
>[!Important]
>Disse evnene vil bli rullet ut gradvis. Fortsett å sjekke Office 365 Message Center for oppdateringer. 

## <a name="known-issues-with-swapping-sites"></a>Kjente problemer ved bytte av områder

- Målområdet kan returnere en feilmelding av typen "ikke funnet" (HTTP 404) for en kort tidsperiode.
- Innhold må være recrawled for å oppdatere søkeindeksen. Det er ingen manuelle trinn som kreves-dette vil bli gjort automatisk.
- Alt som er avhengig av "statiske" koblinger (for eksempel File Sync og OneNote-filer) må rettes manuelt.
- Hvis kildeområdet var et organisatorisk nyhetsområde, oppdaterer du URL-adressen.Få en liste over alle organisatoriske nyhetsnettsteder.
- Project Server-områder må kanskje valideres for å sikre at de fortsatt er riktig tilknyttet.





