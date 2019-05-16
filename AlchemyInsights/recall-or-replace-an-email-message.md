---
title: Tilbakekalle eller erstatte en e-postmelding
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1860
ms.assetid: ''
ms.openlocfilehash: 6e66b5d60fe9ac66c2f2f8f7e99e753652c3a59e
ms.sourcegitcommit: bcb2612ab8ba2aee5165e3912dca95cc1bdd09f4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/16/2019
ms.locfileid: "34096574"
---
# <a name="recall-or-replace-an-email-message"></a>Tilbakekalle eller erstatte en e-postmelding

- Du kan **bare tilbakekalling av meldinger som sendes til personer i organisasjonen**. Hvis meldingen ble sendt til en Gmail-adresse, for eksempel du kan ikke kalle tilbake den.
- Du kan **bare tilbakekalling av meldinger sendt fra Outlook-2016 for PC**. Hvis en bruker sender en melding ved hjelp av Outlook for Mac eller Outlook på World Wide web, kan du ikke kan huske den.
- Hvis du er en administrator, kan du **tilbakekalling av meldinger på vegne av brukere ved hjelp av PowerShell**. Du kan ikke tilbakekalle meldinger fra administrasjonssenteret. Bla ned til "Søk etter og Slett e-postmeldinger i organisasjonen" for mer informasjon.

***Tilbakekalle eller erstatte en e-postmelding du har sendt***
1. Velg mappen Sendte elementer i mapper-ruten til venstre i Outlook-vinduet.
2. Åpne meldingen du vil kalle tilbake. Du må dobbeltklikke for å åpne meldingen. Å merke meldingen slik den vises i leseruten mulig ikke å kalle tilbake meldingen.
3. Velg **Handlinger**i kategorien melding > **Kall tilbake denne meldingen**.
4. Velg **Slette uleste kopier av denne meldingen** , eller **Slette uleste kopier og erstatte dem med en ny melding**, og velg deretter **OK**.
5. Hvis du sender en ny melding, meldingen, og deretter velger du **Send**.
6. Vellykket eller mislykket tilbakekalling av en melding, avhengig av mottakerens innstillinger i Outlook. 

Hvis du vil ha mer informasjon, inkludert hvordan du kontrollerer tilbakekallingen, kan du se [tilbakekalle eller erstatte en e-postmelding som er sendt](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Søk etter og Slett e-postmeldinger i organisasjonen*** Hvis du vil søke etter og slette e-postmeldinger i organisasjonen, er det enklest Hvis du er en global administrator. Hvis du ikke er en global admin, må kontoen legges til rollegruppen eDiscovery Manager eller overholdelse Søk management-rollen. Hvis du vil slette meldinger, må du koble til rollegruppen organisasjon Management eller rollen Søk og Tøm management. Tillatelser til disse rollene tilordnes i [samsvar for Sikkerhetssenter &](https://protection.office.com/).

1. [Opprett en innhold Søk](https://docs.microsoft.com/en-us/office365/securitycompliance/content-search) til å finne meldingen for å slette.
2. [Koble til sikkerhet & overholdelsessenteret PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Hvis du bruker MFA, kan du se [koble til Office 365-sikkerhet & kompatibilitet Center PowerShell ved hjelp av multifaktorautentisering](https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 