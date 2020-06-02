---
title: Hente tilbake eller erstatte en e-postmelding
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
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509465"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Hente tilbake eller erstatte en e-postmelding i Microsoft 365

- Du kan **bare hente meldinger som sendes til personer i organisasjonen**. Hvis e-posten ble sendt til en Gmail-adresse, kan du for eksempel ikke huske den.
- Du kan **bare hente meldinger som sendes fra Outlook-2016 for PCen**. Hvis en bruker sender en melding ved hjelp av Outlook for Mac eller Outlook på nettet, kan du ikke huske den.
- Hvis du er administrator, kan du **hente meldinger på vegne av brukere ved hjelp av PowerShell**. Du kan ikke hente meldinger fra administrasjonssenteret. Rull ned til «Søk etter og slett e-postmeldinger i organisasjonen» hvis du vil ha mer informasjon.

**Hente tilbake eller erstatte en e-postmelding du har sendt**

1. Velg Mappen Sendte elementer i mapperuten til venstre i Outlook-vinduet.
2. Åpne meldingen du vil huske. Du må dobbeltklikke for å åpne meldingen. Hvis du velger meldingen slik at den vises i leseruten, kan du ikke hente frem meldingen.
3. Velg **Handlinger**  >  **Tilbakekall denne meldingen på Melding-fanen**.
4. Velg **Slett uleste kopier av denne meldingen** eller Slett **uleste kopier og erstatt med en ny melding**, og velg deretter **OK**.
5. Hvis du sender en ny melding, skriver du meldingen og velger deretter **Send**.
6. Vellykket eller mislykket meldingsoppkalling avhenger av mottakernes innstillinger i Outlook.

Hvis du vil ha mer informasjon, inkludert hvordan du sjekker tilbakekallingen, kan du se [Tilbakekalle eller erstatte en e-postmelding du har sendt](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Søke etter og slette e-postmeldinger i organisasjonen*** Hvis du vil søke etter og slette e-postmeldinger i organisasjonen, er det enklest hvis du er global administrator. Hvis du ikke er global administrator, må kontoen din legges til rollegruppen for eDiscovery Manager eller rollen Administrasjon av samsvarssøk. Hvis du vil slette meldinger, må du bli med i rollegruppen Organisasjonsstyring eller rollen Administrasjon av søk og tømming. Tillatelser til disse rollene tilordnes i [& samsvarssenter for sikkerhet.](https://protection.office.com/)

1. [Opprett et innholdssøk](https://docs.microsoft.com/microsoft-365/compliance/content-search) for å finne meldingen du vil slette.
2. [Koble til sikkerhets & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Hvis du bruker MFA, kan du se [Koble til Microsoft 365-sikkerhet & Compliance Center PowerShell ved hjelp av godkjenning med flere faktorer](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
