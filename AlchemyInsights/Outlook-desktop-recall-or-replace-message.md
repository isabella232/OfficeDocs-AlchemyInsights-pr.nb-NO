---
title: Skrive bords kall fra Outlook eller erstatte en e-postmelding
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
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663999"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Tilbakekalle eller erstatte en e-postmelding i Outlook

- Som administrator kan du **tilbakekalle meldinger på vegne av brukere som bruker PowerShell**. Du kan ikke tilbakekalle meldinger fra administrasjons senteret.
- Du kan **bare tilbakekalle meldinger som sendes til personer i organisasjonen**. Hvis meldingen for eksempel ble sendt til en Gmail-adresse, kan du ikke tilbakekalle den.
- Du kan **bare tilbakekalle meldinger som er sendt fra Outlook 2016 på PC-en**. Hvis en bruker sender en melding ved hjelp av Outlook for Mac eller Outlook på nettet, kan du ikke tilbakekalle den.

Slik tilbakekaller eller erstatter du en e-postmelding:

1. Velg sendte elementer-mappen i mappe ruten til venstre i Outlook-vinduet.
1. Dobbelt Klikk meldingen du vil kalle tilbake for å åpne den.
1. Velg **melding** -fanen, og velg deretter **handlinger**for å  >  **tilbakekalle denne meldingen**.
1. Velg **Slett uleste kopier av denne meldingen** , eller **Slett uleste kopier og Erstatt med en ny melding**, og velg deretter **OK**.
1. Hvis du sender en erstatnings melding, skriver du meldingen, og deretter velger du **Send**.
1. Om en tilbake melding er vellykket eller mislykket, avhenger av mottakerens innstillinger i Outlook. Hvis du vil ha informasjon om hvordan du sjekker tilbake kallingen, kan du se [denne artikkelen](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Søke etter og slette e-postmeldinger i organisasjonen

- Hvis du ikke er en global administrator, må kontoen legges til i rollen for administrasjon av eDiscovery-administrator og søke etter meldinger. Hvis du vil slette meldinger, må du bli med i rolle gruppen organisasjons behandling eller søke og fjerne administrasjons rollen. Tillatelser for disse rollene er tilordnet i [sikkerhets-og samsvars senteret](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Opprett et innholds søk](https://docs.microsoft.com/microsoft-365/compliance/content-search) for å finne meldingen som skal slettes.
- [Koble til sikkerhets-og samsvars senteret PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Hvis du bruker godkjenning med flere faktorer, kan du se [Koble til Microsoft 365 Security and revisjons senteret PowerShell ved hjelp av godkjenning med flere faktorer](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).