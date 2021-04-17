---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821456"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Løse leveringsproblemer for feilkode 550 5.4.1 Videresendingstilgang nektet

Dette problemet oppstår når [du kontrollerer om en e-postadresse er](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) gyldig for å forhindre returmeldinger når du går inn i Microsoft-nettverket. Prøv følgende:

1. Finn ut om problemet er spesifikt for et helt domene eller én enkelt e-postadresse:
    - Hele domenet: Noen ganger må domenet synkroniseres. prøv [å sette domenet til Internt, og deretter tilbake til Autoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Enkel e-postadresse: Noen ganger må adressen synkroniseres. Det kan hjelpe å endre smtp-proxy-adressen og deretter endre den tilbake.
2. Finn ut om problemet er spesifikt for en gruppe eller fellesmappe. For enkelte objekttyper kan det hende at objektene må opprettes manuelt i Azure Active Directory.

Hvis du trenger mer hjelp, kan du åpne en støtteforespørsel og angi omfanget av problemet (inkludert objekttypen du sender til), slik at vi kan hjelpe deg bedre.