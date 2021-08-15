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
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024395"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Kalle tilbake eller erstatte en e-postmelding i Microsoft 365

- Du kan **bare tilbakekalle meldinger som sendes til personer i organisasjonen.** Hvis meldingen for eksempel ble sendt til en Gmail-adresse, kan du ikke kalle den tilbake.
- Du kan **bare tilbakekalle meldinger som sendes fra Outlook for PC-en.** Hvis en bruker sender en melding ved hjelp av Outlook for Mac eller Outlook på nettet, kan du ikke kalle den tilbake.
- Som leieradministrator kan du kalle tilbake meldinger på vegne av brukere ved hjelp av **PowerShell** (Hvis du vil ha mer informasjon, kan du se: Søke etter [og slette e-postmeldinger](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Du kan ikke kalle tilbake meldinger fra administrasjonssenteret. Rull ned til «Søk etter og slett e-postmeldinger i organisasjonen» for mer informasjon.

**Kalle tilbake eller erstatte en e-postmelding du har sendt**

1. Velg Sendte elementer-mappen i mapperuten til venstre Outlook vinduet.
2. Åpne meldingen du vil kalle tilbake. Du må dobbeltklikke for å åpne meldingen. Hvis du velger meldingen slik at den vises i leseruten, kan du ikke kalle tilbake meldingen.
3. Velg Handlinger som **tilbakekaller** denne meldingen på  >  **Melding-fanen.**
4. Velg **Slett uleste kopier av denne** meldingen eller Slett uleste kopier og erstatt med en **ny** melding, og velg deretter **OK**.
5. Hvis du sender en erstatningsmelding, skriver du meldingen og velger **Deretter Send**.
6. Hvor vellykket eller mislykket en tilbakekalling av meldinger avhenger av mottakernes innstillinger i Outlook.

Hvis du vil ha mer informasjon, inkludert hvordan du kontrollerer tilbakekallingen, kan du se Kalle tilbake [eller erstatte en e-postmelding du har sendt.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Hvis du vil søke etter og slette e-postmeldinger i organisasjonen,*** er det enklest hvis du er global administrator. Hvis du ikke er global administrator, må kontoen din legges til i rollegruppen for eDiscovery Manager eller i rollen for behandling av samsvarssøk. Hvis du vil slette meldinger, må du bli med i rollegruppen organisasjonsbehandling eller rollen søk og tøm behandling. Tillatelser til disse rollene tilordnes i [sikkerhetssenteret & samsvarssenteret](https://protection.office.com/).

1. [Opprett et innholdssøk for](https://docs.microsoft.com/microsoft-365/compliance/content-search) å finne meldingen du vil slette.
2. [Koble til sikkerhets- & Samsvarssenter PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Hvis du bruker MFA (godkjenning med flere faktorer), kan du se Koble til Microsoft 365 [Sikkerhets-& Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)ved hjelp av godkjenning med flere faktorer .
