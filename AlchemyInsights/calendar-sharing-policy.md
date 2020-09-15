---
title: Delings policy for 618-kalender
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
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684239"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Policy feil ved deling av en kalender

1. Gjør ett av følgende, avhengig av situasjonen:
    - Koble til Exchange Online ved hjelp av Remote PowerShell. Hvis du vil ha mer informasjon, kan du se [Koble til Exchange Online ved hjelp av Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Åpne administrasjons grensesnittet for Exchange på den lokale serveren.
2. Bestemme Delings policyen som er tilordnet til brukeren. Hvis du vil gjøre dette, kjører du følgende kommando og noterer policyen som returneres:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Oppdater Delings policyen for brukeren. Dette gjør du slik:
    - Åpne administrasjons senteret for Exchange.
    - Klikk **organisasjon**, og dobbelt klikk deretter policyen som er tilordnet brukeren under **individuell deling**. Dette er policyen som ble returnert i trinn 2.
    - På siden Delings regel velger du Kalender Delings nivået du vil tillate under **Angi hvilken informasjon du vil dele**. Klikk **Lagre**.

Hvis du vil ha mer informasjon, kan du se [«policyen tillater ikke tildeling av tillatelser på dette nivået til én eller flere mottakere av mottaker (s) når brukeren prøver å dele kalenderen](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
