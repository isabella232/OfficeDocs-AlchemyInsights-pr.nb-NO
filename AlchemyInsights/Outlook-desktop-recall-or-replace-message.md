---
title: Tilbakekalling eller erstatte en e-postmelding i Outlook Desktop
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502328"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Hente tilbake eller erstatte en Outlook-e-postmelding

- Som administrator kan du **hente meldinger på vegne av brukere som bruker PowerShell**. Du kan ikke hente meldinger fra administrasjonssenteret.
- Du kan **bare hente meldinger som sendes til personer i organisasjonen**. Hvis e-posten ble sendt til en Gmail-adresse, kan du for eksempel ikke huske den.
- Du kan **bare hente meldinger som sendes fra Outlook-2016 på PCen**. Hvis en bruker sender en melding ved hjelp av Outlook for Mac eller Outlook på nettet, kan du ikke huske den.

Slik tilbakekaller eller erstatter du en e-postmelding:

1. Velg mappen Sendte elementer i mapperuten til venstre i Outlook-vinduet.
1. Dobbeltklikk meldingen du vil tilbakekalle for å åpne den.
1. Velg **kategorien Melding,** og velg deretter **Handlinger**  >  **Tilbakekall denne meldingen**.
1. Velg **Slett uleste kopier av denne meldingen** eller Slett **uleste kopier og erstatt med en ny melding**, og velg deretter **OK**.
1. Hvis du sender en ny melding, skriver du meldingen og velger deretter **Send**.
1. Vellykket eller mislykket meldingsoppbakkalling avhenger av mottakerens innstillinger i Outlook. Hvis du vil ha fremgangsmåte for å sjekke tilbakekallingen, kan du se [denne artikkelen](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Søke etter og slette e-postmeldinger i organisasjonen

- Hvis du ikke er global administrator, må kontoen din legges til rollen eDiscovery Manager eller compliance search management-rollen for å søke etter meldinger. Hvis du vil slette meldinger, må du bli med i rollegruppen Organisasjonsstyring eller rollen Administrasjon av søk og tømming. Tillatelser for disse rollene tilordnes i [sikkerhets- og samsvarssenteret](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Opprett et innholdssøk](https://docs.microsoft.com/microsoft-365/compliance/content-search) for å finne meldingen du vil slette.
- [Koble til Sikkerhets- og samsvarssenter PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Hvis du bruker godkjenning med flere faktorer, kan du se [Koble til Microsoft 365-sikkerhets- og samsvarssenter PowerShell ved hjelp av godkjenning med flere faktorer](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).