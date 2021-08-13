---
title: Outlook Tilbakekalle eller erstatte en e-postmelding på skrivebordet
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918404"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Kalle tilbake eller erstatte en Outlook e-postmelding

- Som administrator kan du kalle **tilbake meldinger på vegne av brukere som bruker PowerShell.** Du kan ikke kalle tilbake meldinger fra administrasjonssenteret.
- Du kan **bare tilbakekalle meldinger som sendes til personer i organisasjonen.** Hvis meldingen ble sendt til en Gmail-adresse, kan du for eksempel ikke kalle den tilbake.
- Du kan **bare tilbakekalle meldinger som sendes fra Outlook 2016 på PC-en.** Hvis en bruker sender en melding ved hjelp av Outlook for Mac eller Outlook på nettet, kan du ikke kalle den tilbake.

Slik tilbakekaller eller erstatter du en e-postmelding:

1. Velg Sendte elementer-mappen i mapperuten til venstre Outlook vinduet.
1. Dobbeltklikk meldingen du vil kalle tilbake for å åpne den.
1. Velg **Melding-fanen,** og velg deretter **Handlinger**  >  **tilbakekall denne meldingen**.
1. Velg **Slett uleste kopier av denne** meldingen eller Slett uleste kopier og erstatt med en **ny** melding , og velg deretter **OK**.
1. Hvis du sender en erstatningsmelding, skriver du meldingen og velger deretter **Send**.
1. Hvor vellykket eller mislykket tilbakekallingen av en melding er avhengig av mottakerens innstillinger i Outlook. Hvis du vil ha informasjon om hvordan du kontrollerer tilbakekallingen, kan [du se denne artikkelen](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Søke etter og slette e-postmeldinger i organisasjonen

- Hvis du ikke er global administrator, må kontoen din legges til i rollen eDiscovery Manager eller administrasjonsrollen for samsvarssøk for å søke etter meldinger. Hvis du vil slette meldinger, må du bli med i rollegruppen organisasjonsbehandling eller rollen søk og tøm behandling. Tillatelser for disse rollene tilordnes i [sikkerhets- og samsvarssenteret.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Opprett et innholdssøk for](https://docs.microsoft.com/microsoft-365/compliance/content-search) å finne meldingen du vil slette.
- [Koble til sikkerhets- og samsvarssenteret PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Hvis du bruker godkjenning med flere faktorer, kan du [Koble til for Microsoft 365 powershell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)for sikkerhet og samsvarssenter ved hjelp av godkjenning med flere faktorer.