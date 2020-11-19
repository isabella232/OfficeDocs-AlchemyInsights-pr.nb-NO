---
title: Kalle tilbake eller erstatte en e-postmelding
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353515"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Kalle tilbake eller erstatte en e-postmelding i Microsoft 365

- Du kan **bare tilbakekalle meldinger som sendes til personer i organisasjonen**. Hvis meldingen for eksempel ble sendt til en Gmail-adresse, kan du ikke tilbakekalle den.
- Du kan **bare tilbakekalle meldinger som er sendt fra Outlook for PC-en**. Hvis en bruker sender en melding ved hjelp av Outlook for Mac eller Outlook på nettet, kan du ikke tilbakekalle den.
- Som leier administrator kan du **tilbakekalle meldinger på vegne av brukere ved hjelp av PowerShell** (Hvis du vil ha mer informasjon, se: [søke etter og slette e-postmeldinger](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Du kan ikke tilbakekalle meldinger fra administrasjons senteret. Rull ned til søk etter og slett e-postmeldinger i organisasjonen for mer informasjon.

**Tilbakekalle eller erstatte en e-postmelding du har sendt**

1. I mappe ruten til venstre i Outlook-vinduet velger du sendte elementer-mappen.
2. Åpne meldingen du vil kalle tilbake. Du må dobbeltklikke for å åpne meldingen. Hvis du velger meldingen slik at den vises i lese ruten, kan du ikke kalle tilbake meldingen.
3. På melding-fanen velger du **handlinger** for å  >  **tilbakekalle denne meldingen**.
4. Velg **Slett uleste kopier av denne meldingen** , eller **Slett uleste kopier og Erstatt med en ny melding**, og velg deretter **OK**.
5. Hvis du sender en erstatnings melding, skriver du meldingen og velger **Send**.
6. Mottakerens innstillinger i Outlook er vellykket eller mislykket tilbake kalling av meldingen.

Hvis du vil ha mer informasjon, inkludert hvordan du sjekker tilbake kallingen, kan [du se kalle tilbake eller erstatte en e-postmelding du har sendt](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Hvis du **_vil søke etter og slette e-postmeldinger i organisasjonen_**, er det enklest hvis du er en global administrator. Hvis du ikke er global administrator, må kontoen legges til i rolle gruppen eDiscovery Manager, eller i rollen som søke behandling for samsvar. Hvis du vil slette meldinger, må du bli med i rolle gruppen organisasjons behandling eller søke og fjerne administrasjons rollen. Tillatelser til disse rollene er tilordnet i [sikkerhets & samsvars senteret](https://protection.office.com/).

1. [Opprett et innholds søk](https://docs.microsoft.com/microsoft-365/compliance/content-search) for å finne meldingen som skal slettes.
2. [Koble til sikkerhets & samsvars senteret PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Hvis du bruker MFA (godkjenning med flere faktorer), kan du se [Koble til Microsoft 365 sikkerhets & samsvars senteret PowerShell ved hjelp av godkjenning med flere faktorer](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
