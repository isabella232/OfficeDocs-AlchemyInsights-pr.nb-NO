---
title: Tilbakekalle eller erstatte en e-postmelding
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e541620a499b02a7206579ffcc505ceb4e632a4c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742764"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Hente eller erstatte en e-postmelding i Microsoft 365

- Du kan **bare hente meldinger som sendes til personer i organisasjonen**. Hvis meldingen ble sendt til en Gmail-adresse, kan du for eksempel ikke huske den.
- Du kan **bare hente meldinger som sendes fra Outlook 2016 for PCen**. Hvis en bruker sender en melding ved hjelp av Outlook for Mac eller Outlook på nettet, kan du ikke huske den.
- Hvis du er administrator, kan du **hente meldinger på vegne av brukere ved hjelp av PowerShell**. Du kan ikke hente meldinger fra administrasjonssenteret. Rull ned til "Søk etter og slett e-postmeldinger i organisasjonen" for mer informasjon.

**Tilbakekall eller erstatt en e-postmelding du sendte**

1. Velg Mappen Sendte elementer i mapperuten til venstre i Outlook-vinduet.
2. Åpne meldingen du vil huske. Du må dobbeltklikke for å åpne meldingen. Hvis du velger meldingen slik at den vises i leseruten, kan du ikke hente meldingen.
3. Velg **Handlinger tilbakekall** > **denne meldingen**i kategorien Melding .
4. Velg **Slett uleste kopier av denne meldingen** eller Slett **uleste kopier og erstatt med en ny melding**, og velg deretter **OK**.
5. Hvis du sender en erstatningsmelding, skriver du meldingen og velger **deretter Send**.
6. Vellykket eller mislykket tilbakekalling av meldinger avhenger av mottakernes innstillinger i Outlook.

Hvis du vil ha mer informasjon, inkludert hvordan du sjekker tilbakekallingen, kan du se [Tilbakekall eller erstatte en e-postmelding du sendte](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Søke etter og slette e-postmeldinger i organisasjonen*** Hvis du vil søke etter og slette e-postmeldinger i organisasjonen, er det enklest hvis du er global administrator. Hvis du ikke er global administrator, må kontoen din legges til i rollegruppen eDiscovery Manager eller i rollen administrasjon av samsvarssøk. Hvis du vil slette meldinger, må du bli med i rollegruppen Organisasjonsstyring eller rollen Administrasjon for søk og tømming. Tillatelser til disse rollene tilordnes i [samsvarssenter for sikkerhet &](https://protection.office.com/).

1. [Opprett et innholdssøk](https://docs.microsoft.com/office365/securitycompliance/content-search) for å finne meldingen som skal slettes.
2. [Koble til Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Hvis du bruker MFA, kan du se [Koble til Microsoft 365-sikkerhet & Compliance Center PowerShell ved hjelp av godkjenning med flere faktorer](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
