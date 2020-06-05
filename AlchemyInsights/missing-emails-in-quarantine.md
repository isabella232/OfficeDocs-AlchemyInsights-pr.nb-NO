---
title: Manglende e-post i karantene
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569554"
---
# <a name="missing-emails-in-quarantine"></a>Manglende e-post i karantene"

Administratorer kan [vise, frigi eller slette disse meldingene.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Hvis du vil åpne & for &, går du til [https://protection.office.com](https://protection.office.com/) . Hvis du vil åpne Karantene-siden direkte, går du til [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Du kan søke etter følgende verdier:  

- **Meldings-ID**: Den globalt unike identifikatoren for meldingen. Hvis du velger en melding i listen, vises **Details** **meldings-ID-verdien** i detalj-undermenyen som vises. Administratorer kan bruke [meldingssporing](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) til å finne meldinger og de tilsvarende meldings-ID-verdiene.
- **Avsenderens e-postadresse**: En enkelt avsenders e-postadresse.
- **Mottaker-e-postadresse:** En enkelt mottakers e-postadresse.
- **Emne**: Bruk hele emnet i meldingen. Søket skiller ikke mellom store og små bokstaver.

Når du har angitt søkekriteriene, klikker du ![ Oppdater-knappen Oppdater for ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** å filtrere resultatene.  

Cmdletene du bruker til å vise og administrere meldinger og filer i karantene, er:
- [Slett karanteneMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Eksport-karanteneMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Få karanteneMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Forhåndsvisning-KaranteneMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Vær oppmerksom på at denne cmdleten er bare for meldinger, ikke malware-filer fra ATP for SharePoint Online, OneDrive for Bedrifter eller Teams.
- [Slipp karanteneMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)