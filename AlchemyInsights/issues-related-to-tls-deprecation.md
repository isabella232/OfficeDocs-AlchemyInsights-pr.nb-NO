---
title: Kan ikke sende/motta e-post til/fra Office 365 på grunn av TLS 1.0- og TLS 1.1-deaktiveringen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747122"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Kan ikke sende/motta e-post til/fra Office 365 på grunn av TLS 1.0- og TLS 1.1-deaktiveringen

Som bekreftet av meldingssenteret ble MC229914, TLS 1.0 og TLS 1.1-avviklingen startet å håndheve for Exchange Online-endepunkter for e-postflyt. Snart godtar ikke Office 365 TLS 1.0- og TLS 1.1-e-posttilkoblinger fra eksterne kilder. Exchange Online bruker heller aldri TLS 1.0 eller 1.1 til å sende utgående e-post. Hvis du har problemer på grunn av TLS 1.0- eller 1.1-deaktivering, kan du oppleve en av følgende feil:

- Avsenderen får NDR-retur - '421 4.4.2 Tilkobling ble brutt på grunn av SocketError'
- Feil i køvisningsprogrammet for lokal server som sender e-post til Officer 365- '421 4.4.2-tilkobling droppet på grunn av SocketError'
- Feil i Logg for Send [koblingsprotokoll](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) på serveren som sender e-post til Office 365– TLS-forhandling mislyktes med feilen SocketError
- Feil i protokollloggen for Send eller motta kobling – '451 5.7.3 Må utstede en STARTTLS-kommando først'

Hvis du opplever noen av feilene ovenfor, må du kontrollere at serveren som sender eller mottar e-post, har TLS 1.2 aktivert ved å kontrollere følgende registernøkler:

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:0000000 "Enabled"=dword:0000001**

Hvis du gjør endringer i registernøklene ovenfor for å aktivere TLS 1.2, starter du serveren på nytt for at endringene skal tre i kraft. Kontroller også at du har de nyeste Windows- og Exchange-oppdateringene installert.

Hvis du vil ha mer informasjon, kan du se:

- [Veiledning for Exchange Server TLS, del 1: Gjør deg klar for TLS 1.2 – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Veiledning for Exchange Server TLS Del 2: Aktivere TLS 1.2 og identifisere klienter som ikke bruker det – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Forstå e-postscenarioer hvis TLS-versjoner ikke kan avtales med Exchange Online – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
