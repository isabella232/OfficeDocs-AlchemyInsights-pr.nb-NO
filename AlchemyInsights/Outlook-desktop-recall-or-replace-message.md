---
title: Tilbakekalling av Outlook-skrivebord eller erstatt en e-postmelding
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687519"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Tilbakekalle eller erstatte en Outlook-e-postmelding

- Som administrator kan du **tilbakekalle meldinger på vegne av brukere som bruker PowerShell**. Du kan ikke hente meldinger fra administrasjonssenteret.
- Du kan **bare hente meldinger som sendes til personer i organisasjonen**. Hvis meldingen ble sendt til en Gmail-adresse, kan du for eksempel ikke huske den.
- Du kan **bare hente meldinger som sendes fra Outlook-2016 på PCen**. Hvis en bruker sender en melding ved hjelp av Outlook for Mac eller Outlook på nettet, kan du ikke huske den.

Slik tilbakekaller eller erstatter du en e-postmelding:

1. Velg Mappen Sendte elementer i mapperuten til venstre i Outlook-vinduet.
1. Dobbeltklikk meldingen du vil huske for å åpne den.
1. Velg **kategorien Melding,** og velg deretter **Handlinger** > **tilbakekall denne meldingen**.
1. Velg **Slett uleste kopier av denne meldingen** eller Slett **uleste kopier, og erstatt med en ny melding**, og velg deretter **OK**.
1. Hvis du sender en erstatningsmelding, skriver du meldingen, og deretter velger du **Send**.
1. Vellykket eller mislykket tilbakekalling av en melding avhenger av mottakerens innstillinger i Outlook. Hvis du vil ha trinn for å se om tilbakekallingen, kan du se [denne artikkelen](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Søke etter og slette e-postmeldinger i organisasjonen

- Hvis du ikke er global administrator, må kontoen din legges til i rollen eDiscovery Manager eller rollen for administrasjon av samsvarsøk for å søke etter meldinger. Hvis du vil slette meldinger, må du bli med i rollegruppen Organisasjonsstyring eller rollen Administrasjon for søk og tømming. Tillatelser for disse rollene tilordnes i [sikkerhets- og samsvarssenteret](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Opprett et innholdssøk](https://docs.microsoft.com/office365/securitycompliance/content-search) for å finne meldingen som skal slettes.
- [Koble til Sikkerhets- og samsvarssenter PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Hvis du bruker godkjenning med flere faktorer, kan du se [Koble til Microsoft 365-sikkerhet og samsvarssenter PowerShell ved hjelp av godkjenning med flere faktorer](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).