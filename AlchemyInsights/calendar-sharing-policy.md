---
title: 618 Policy for kalenderdeling
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091612"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Policyfeil når du deler en kalender

1. Gjør ett av følgende etter behov for din situasjon:
    - Koble til å Exchange Online ved hjelp av Ekstern PowerShell. Hvis du vil ha mer [informasjon, Koble til du Exchange Online bruke Ekstern PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Åpne administrasjonsskallet for Exchange på den lokale serveren.
2. Bestem delingspolicyen som er tilordnet til brukeren. Hvis du vil gjøre dette, kjører du følgende kommando og noterer policyen som returneres:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Oppdater delingspolicyen for brukeren. Dette gjør du slik:
    - Åpne Exchange administrasjonssenteret.
    - Klikk **Organisasjon**, og dobbeltklikk deretter policyen som er tilordnet til brukeren, under **Individuell deling**. Dette er policyen som ble returnert i trinn 2.
    - Velg kalenderdelingsnivået du vil tillate under Angi hvilken informasjon du vil dele, på **delingsregelsiden.** klikk **Lagre**.

Hvis du vil ha mer informasjon, kan du se: Policyen tillater ikke tildeling av tillatelser på dette nivået til én eller flere av [mottakerne](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)når brukeren prøver å dele kalenderen .
