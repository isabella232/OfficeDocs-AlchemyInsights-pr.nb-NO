---
title: 451 4.7.0 Midlertidig serverfeil. Prøv på nytt senere. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812585"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Midlertidig serverfeil. Prøv på nytt senere. PRX4

Det kan være et problem når du sender e-post via Smarthost «smtp.office365.com» ved hjelp av SMTP-klientinnsendingsmetoden og får feilmeldingen: «451 4.7.0 Midlertidig serverfeil. Prøv på nytt senere. PRX4 er for det meste midlertidig.» 

Kontroller at du ikke bruker en delt postboks for SMTP-klientinnsending, da SMTP-klientens innsendingsmetode krever en lisensiert postboks å sende e-post gjennom. Hvis du imidlertid ikke bruker en delt postboks og problemet vedvarer, kontrollerer du følgende:

1. Aktiver SMTP-klientinnsending på den lisensierte postboksen som brukes ved å kjøre denne PowerShell-kommandoen:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    ELLER

    1. Gå til Administrasjonssenter for Microsoft 365 > **Aktive brukere**, og velg brukeren.
    1. Gå til E-post-fanen > **e-postapper** > **behandle e-postapper**. 
    1. Kontroller at godkjent **SMTP-innstillingen** er avmerket (aktivert).
    1. Velg **Lagre endringer**.
    
    Hvis du vil aktivere SMTP-godkjenning for en hel organisasjon, kjører du denne kommandoen:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Obs!** Av sikkerhetsgrunner anbefales det at du aktiverer SMTP-godkjenning bare for postboksen som brukes. Innstillingen for brukernivå overstyrer innstillingen for organisasjonsnivå.

2. Deaktiver Azure-sikkerhetsstandarder ved å slå **aktiver sikkerhetsstandarder** til **Nei:**

    1. Logg deg på Azure-portalen som sikkerhetsadministrator, betinget tilgangsadministrator eller global administrator.
    1. Bla til Azure Active Directory >**  egenskaper**, og velg **Behandle sikkerhetsstandarder**.
    1. Sett **veksleknappen Aktiver sikkerhetsstandarder** til **Nei**.
    1. Velg **Lagre**.

3. Deaktiver godkjenning med flere faktorer (MFA) på den lisensierte postboksen som brukes.

    1. Gå til Administrasjonssenter for Microsoft 365, og velg Brukere aktive brukere i  >  **navigasjonsmenyen til venstre.**
    1. Velg Godkjenning **med flere** faktorer på Aktive **brukere-siden.**
    1. Velg brukeren, og deaktiver **godkjenning med flere faktorer**.

