---
title: Manglende e-postmeldinger i karantene
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673723"
---
# <a name="missing-emails-in-quarantine"></a>Manglende e-postmeldinger i karantene

Administratorer kan [vise, frigi eller slette disse meldingene.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Hvis du vil åpne sikkerhets & Samsvars senteret, går du til [https://protection.office.com](https://protection.office.com/) . Hvis du vil åpne karantene siden direkte, går du til [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Du kan søke etter følgende verdier:  

- **Meldings-ID**: den globalt unike identifikatoren for meldingen. Hvis du velger en melding i listen, vises  **meldings-ID**  -verdien i ruten  **detaljer**  under meny som vises. Administratorer kan bruke [meldings sporing](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) til å finne meldinger og tilsvarende meldings-ID-verdier.
- **Avsender-e**-postadresse: en enkelt avsenderens e-postadresse.
- **Mottakerens e-postadresse**: en enkelt mottakers e-postadresse.
- **Emne**: Bruk hele emnet i meldingen. Søket skiller ikke mellom store og små bokstaver.

Når du har skrevet inn søke kriteriene, klikker du Oppdater ![ knappe ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **oppdatering** for å filtrere resultatene.  

Cmdletene du bruker til å vise og administrere meldinger og filer i karantene, er:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Eksporter-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Vær oppmerksom på at denne cmdleten bare er for meldinger, ikke filer med skadelig program vare fra ATP for SharePoint Online, OneDrive for Business eller Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)