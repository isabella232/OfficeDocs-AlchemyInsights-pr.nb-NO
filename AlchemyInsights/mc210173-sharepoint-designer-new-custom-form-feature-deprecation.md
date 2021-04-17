---
title: MC210173 – utforming av nytt egendefinert skjema for SharePoint Designer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831815"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 – utforming av nytt egendefinert skjema for SharePoint Designer

Vi har identifisert et problem som berører SharePoint Designer-funksjonalitet for [oppretting av egendefinerte skjemaer](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) i SharePoint Online. Etter nøye gjennomgang har vi kommet frem til at det ikke finnes noen kjent løsning for dette problemet og har valgt å deaktivere funksjonen for tilpasset skjema-opprettelse fra og med kl. 03.00 UTC på lørdag 25. april 2020. Denne endringen påvirker ikke muligheten til å redigere tidligere opprettede skjemaer eller andre eksisterende funksjoner i SharePoint Online Designer.

Etter denne endringen var utført kan brukere ha mottatt feilen: «Kunne ikke lagre listeendringene på serveren», ved oppretting av nye skjemaer.

Brukere som tidligere har brukt SharePoint Designer til å opprette egendefinerte skjemaer, kan i stedet bruke [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) til dette formålet.

PowerApps er et enkelt og kraftig verktøy som gjør det mulig for brukere som bruker SharePoint Online Modern-opplevelsen, å opprette og redigere tilpassede skjemaer for SharePoint-lister og dokumentbiblioteker rett fra et nettleservindu. PowerApps krever ikke kunnskap om tradisjonell koding eller andre appnedlastinger som for eksempel InfoPath.

**Obs**: Brukere av SharePoint Online Classic må midlertidig bytte til den moderne opplevelsen for tilgang til og for å bruke PowerApps, men alle tilpassede skjemaer opprettet i PowerApps, er tilgjengelige for brukere av SharePoint Online Class-opplevelsen.
