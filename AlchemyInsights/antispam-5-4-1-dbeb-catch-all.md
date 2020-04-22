---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707920"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Løs leveringsproblemer for feilkode 550 5.4.1 Relétilgang nektet

Dette problemet oppstår når [du kontrollerer om en e-postadresse er gyldig for å hindre tilbakeslag](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) når du går inn i Microsoft-nettverket. Prøv følgende:

1. Finn ut om problemet er spesifikt for et helt domene eller en enkelt e-postadresse:
    - Hele domenet: Noen ganger må domenet synkroniseres. prøve [å sette domenet til Intern og deretter tilbake til Autoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Én e-postadresse: Noen ganger må adressen synkroniseres. endre smtp proxy-adressen og deretter endre den tilbake kan hjelpe.
2. Finn ut om problemet er spesifikt for en gruppe eller fellesmappe. For enkelte objekttyper må det hende at objektene opprettes manuelt i Azure Active Directory.

Hvis du trenger ekstra hjelp, må du åpne en støttebillett og angi omfanget av problemet (inkludert typen objekt du sender til), slik at vi kan hjelpe deg bedre.