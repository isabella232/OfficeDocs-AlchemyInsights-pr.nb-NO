---
title: Manglende e-postmeldinger i karantene
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831743"
---
# <a name="missing-emails-in-quarantine"></a>Manglende e-postmeldinger i karantene"

Administratorer kan [vise, frigi eller slette disse meldingene.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Hvis du vil åpne sikkerhetssenteret & samsvarssenteret, går du til [https://protection.office.com](https://protection.office.com/) . Hvis du vil åpne Karantenesiden direkte, går du til [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Du kan søke etter følgende verdier:  

- **Meldings-ID:** Den globalt unike identifikatoren for meldingen. Hvis du velger en melding i listen, vises  **Meldings-ID-verdien**  i  **detaljer-undermenyen**  som vises. Administratorer kan bruke [meldingssporing til](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) å finne meldinger og tilhørende meldings-ID-verdier.
- **Avsenderens e-postadresse:** En enkelt avsenders e-postadresse.
- **E-postadresse for** mottaker: Én enkelt mottakers e-postadresse.
- **Emne:** Bruk hele emnet i meldingen. Søket skiller ikke mellom store og små bokstaver.

Når du har angitt søkekriteriene, klikker du ![ Oppdater-knappen ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Oppdater for** å filtrere resultatene.  

Cmdletene du bruker til å vise og behandle meldinger og filer i karantene, er:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Vær oppmerksom på at denne cmdleten bare er for meldinger, ikke skadelig programvarefiler fra ATP for SharePoint Online, OneDrive for Business eller Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)