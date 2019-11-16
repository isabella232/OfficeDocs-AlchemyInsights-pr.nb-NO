---
title: AntiSpam 5.4.1 DBEB fange-alle
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
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672442"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Løs leveringsproblemer for feilkode 550 5.4.1 Relay tilgang avslått

Dette problemet oppstår når du [kontrollerer om en e-postadresse er gyldig for å forhindre bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) når du angir Office 365-nettverket. Prøv følgende:

1. Finn ut om problemet er spesifikt for et helt domene eller en enkelt e-postadresse:
    - Hele domenet: noen ganger må domenet synkroniseres. Prøv [å sette domenet til intern og deretter tilbake til autoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Enkelt e-postadresse: noen ganger må adressen være synkronisert; skiftende det SMTP proxy henvende seg og så skiftende den rygg kanne hjelpe.
2. Finn ut om problemet er spesifikt for en gruppe eller fellesmappe. For noen objekttyper kan det hende at objektene må opprettes manuelt i Azure Active Directory.

Hvis du trenger mer hjelp, kan du åpne en støtte billett og angi omfanget av problemet (includidng typen objekt du sender til), slik at vi kan hjelpe deg bedre.