---
title: AntiSpam 5.4.1 DBEB Catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717370"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Løse leverings problemer for feilkode 550 5.4.1 relé ingen tilgang

Dette problemet oppstår når [du ser etter at en e-postadresse er gyldig for å forhindre bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) når du skriver inn Microsoft-nettverket. Prøv følgende:

1. Finn ut om problemet er spesifikt for et helt domene eller én enkelt e-post adresse:
    - Hele domenet: noen ganger må domenet synkroniseres. Prøv å [Angi domenet til internt, og deretter tilbake til autoritativt](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Enkel e-post adresse: noen ganger må adressen synkroniseres. å endre SMTP-proxy-adressen og deretter endre den tilbake kan hjelpe deg.
2. Finn ut om problemet er spesifikke for en gruppe eller en felles mappe. For enkelte objekt typer kan det hende at objektene må opprettes manuelt i Azure Active Directory.

Hvis du trenger mer hjelp, kan du åpne en støtte forespørsel og angi omfanget av problemet (inkludert objekt typen du sender til), slik at vi kan hjelpe deg bedre.