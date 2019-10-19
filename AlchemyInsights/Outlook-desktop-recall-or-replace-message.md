---
title: Outlook desktop tilbakekalle eller erstatte en e-postmelding
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36496120"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Tilbakekalle eller erstatte en Outlook-e-postmelding

- Som administrator kan du **tilbakekalle meldinger på vegne av brukere som bruker PowerShell**. Du kan ikke tilbakekalle meldinger fra administrasjonssenteret.
- Du kan **bare tilbakekalle meldinger som er sendt til personer i organisasjonen**. Hvis meldingen for eksempel ble sendt til en Gmail-adresse, kan du ikke huske den.
- Du kan **bare tilbakekalle meldinger som er sendt fra Outlook 2016 på PC**-en. Hvis en bruker sender en melding ved hjelp av Outlook for Mac eller Outlook på weben, kan du ikke tilbakekalle den.

Slik tilbakekaller eller erstatter du en e-postmelding:

1. I mapperuten til venstre i Outlook-vinduet velger du sendte elementer-mappen.
1. Dobbeltklikk meldingen du vil tilbakekalle, for å åpne den.
1. Velg kategorien **melding** , og velg deretter **handlinger** > **tilbakekall denne meldingen**.
1. Velg **Slett uleste kopier av denne meldingen** eller **Slett uleste kopier og Erstatt med en ny melding**, og velg deretter **OK**.
1. Hvis du skal sende en ny melding, skriver du meldingen og velger **Send**.
1. Mottakerens innstillinger i Outlook er vellykket eller mislykket av en tilbakekalling av melding. Hvis du vil ha trinn for hvordan du ser tilbakekallingen, kan du se [denne artikkelen](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Søke etter og slette e-postmeldinger i organisasjonen

- Hvis du ikke er en global administrator, må kontoen din legges til rollen eDiscovery Manager eller kontroll av Samsvars søk for å søke etter meldinger. Hvis du vil slette meldinger, må du bli med i rollegruppen for organisasjonsadministrasjon eller administrasjons rollen for søk og fjerning. Tillatelser for disse rollene er tilordnet i [sikkerhets-og samsvarssenteret](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Opprett et innholdssøk](https://docs.microsoft.com/office365/securitycompliance/content-search) for å finne meldingen som skal slettes.
- [Koble til PowerShell for sikkerhets-og samsvarssenter](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Hvis du bruker multifaktorautentisering, kan du se [Koble til Office 365 sikkerhet og kompatibilitet Center PowerShell ved hjelp av multi-faktor-godkjenning](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).