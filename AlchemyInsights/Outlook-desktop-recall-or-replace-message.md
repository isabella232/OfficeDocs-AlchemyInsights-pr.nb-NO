---
title: Outlook stasjonære tilbakekalle eller erstatte en e-postmelding
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496120"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Tilbakekalle eller erstatte en e-postmelding i Outlook

- Som administrator kan du **tilbakekalling av meldinger på vegne av brukere ved hjelp av PowerShell**. Du kan ikke tilbakekalle meldinger fra administrasjonssenteret.
- Du kan **bare tilbakekalling av meldinger som sendes til personer i organisasjonen**. Hvis meldingen ble sendt til en Gmail-adresse, for eksempel du kan ikke kalle tilbake den.
- Du kan **bare tilbakekalling av meldinger sendt fra Outlook-2016 på PCen**. Hvis en bruker sender en melding ved hjelp av Outlook for Mac eller Outlook på World Wide web, kan du ikke kan huske den.

Tilbakekalle eller erstatte en e-postmelding:

1. Velg mappen Sendte elementer i mapper-ruten til venstre i Outlook-vinduet.
1. Dobbeltklikk meldingen du vil kalle tilbake for å åpne den.
1. Velg kategorien **melding** , og velg deretter **Handlinger** > **Kall tilbake denne meldingen**.
1. Velg **Slette uleste kopier av denne meldingen** , eller **Slette uleste kopier og erstatte dem med en ny melding**, og velg deretter **OK**.
1. Hvis du sender en ny melding, meldingen, og deretter velger du **Send**.
1. Vellykket eller mislykket tilbakekalling av en melding, avhengig av mottakerens innstillinger i Outlook. Fremgangsmåte å kontrollere tilbakekalling i [denne artikkelen](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Søke etter og slette e-postmeldinger i organisasjonen

- Hvis du ikke er en global admin, må kontoen legges til eDiscovery lederrolle eller overholdelse Søk management rollen til å søke etter meldinger. Hvis du vil slette meldinger, må du koble til rollegruppen organisasjon Management eller rollen Søk og Tøm management. Tillatelser for disse rollene tilordnes i [midten av sikkerhet og overholdelse](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Opprett en innhold Søk](https://docs.microsoft.com/office365/securitycompliance/content-search) til å finne meldingen for å slette.
- [Koble til sikkerhet og overholdelse Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Hvis du bruker multifaktorautentisering, kan du se [koble til Office 365-sikkerhet og overholdelse Center PowerShell ved hjelp av multifaktorautentisering](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).