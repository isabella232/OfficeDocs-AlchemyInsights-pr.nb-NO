---
title: 618 Retningslinjer for deling av kalender
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373008"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Policyfeil ved deling av en kalender

1. Gjør ett av følgende, avhengig av situasjonen:
    - Koble til Exchange Online ved hjelp av Ekstern PowerShell. Hvis du vil ha mer informasjon, kan du se [Koble til Exchange Online ved hjelp av Ekstern PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Åpne Exchange Management Shell på den lokale serveren.
2. Bestem delingspolicyen som er tilordnet til brukeren. Hvis du vil gjøre dette, kjører du følgende kommando og noterer policyen som returneres:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Oppdater delingspolicyen for brukeren. Hvis du vil gjøre dette, gjør du følgende:
    - Åpne administrasjonssenteret for Exchange.
    - Klikk **Organisasjon**, og dobbeltklikk deretter policyen som er tilordnet til brukeren under **Individuell deling**. Dette er policyen som ble returnert i trinn 2.
    - Velg kalenderdelingsnivået du vil tillate, under Angi **hvilken informasjon du vil dele**. klikk **Lagre**.

Hvis du vil ha mer informasjon, kan du se: ["Policyen tillater ikke tildeling av tillatelser på dette nivået til én eller flere av mottakeren(e)"-feil når brukeren prøver å dele kalenderen](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
