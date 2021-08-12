---
title: Bytte det klassiske rotnettstedet med et moderne nettsted
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
ms.openlocfilehash: 7209595f5cda9b31e53241d9d5696fa584ff5e5ab3d237aae28542bf7aec9398
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940828"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Bytte det klassiske rotnettstedet med et moderne nettsted

Hvis miljøet ble konfigurert før april 2019, kan du endre rotnettstedet til et moderne nettsted ved hjelp av Microsoft PowerShell:

- Hvis du har et annet nettsted som du vil bruke som rotnettsted, kan du [erstatte (bytte) rotnettstedet](https://docs.microsoft.com/sharepoint/modern-root-site) med det. 
    - Bruk [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et nettsted med et annet nettsted mens du arkiverer det opprinnelige nettstedet. Tilgjengelig for både gruppenettsted (ikke koblet til en gruppe) og kommunikasjonsnettstedet. 

- Flere funksjoner innføres snart, slik at du kan fortsette å bruke innholdet på nettstedet, men konvertere det eksisterende nettstedet til et kommunikasjonsnettsted. 
>[!Important]
>Disse funksjonene rulles ut gradvis. Fortsett å se etter oppdateringer i meldingssenteret. 

## <a name="known-issues-with-swapping-sites"></a>Kjente problemer med å bytte nettsteder

- Målnettstedet kan returnere feilmeldingen «Finner ikke» (HTTP 404) i en kort tidsperiode.
- Innhold må på nytt for å oppdatere søkeindeksen. Det kreves ingen manuelle trinn – dette gjøres automatisk.
- Alt som er avhengig av statiske koblinger (for eksempel filsynkronisering OneNote filer), må korrigeres manuelt.
- Hvis kildenettstedet var et nyhetsnettsted for organisasjonen, oppdaterer du nettadressen. Få en liste over alle nyhetsnettsteder for organisasjonen.
- Project Servernettsteder må kanskje valideres for å sikre at de fortsatt er tilknyttet riktig.
