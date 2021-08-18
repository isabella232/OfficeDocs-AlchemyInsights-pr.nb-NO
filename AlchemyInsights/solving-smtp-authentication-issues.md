---
title: Aktivere SMTP-godkjenning og feilsøking
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 14f1454ad687b4d76cf419583b442685fa19b5a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321762"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Aktivere SMTP-godkjenning og feilsøking

Hvis du vil aktivere SMTP-godkjenning for en postboks eller du får feilmeldingen «Klient ikke godkjent», «Godkjenning mislyktes» eller «SmtpClientAuthentication» med kode 5.7.57 eller 5.7.3 eller 5.7.139 når du prøver å videresende e-post ved å godkjenne en enhet eller et program med Microsoft 365, utfører du disse tre handlingene for å løse problemet:

1. Deaktiver [sikkerhetsstandardene for Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) ved å slå **Aktiver sikkerhetsstandarder** til **Nei**.

    a. Logg på Azure-portalen som sikkerhetsadministrator, betinget tilgangsadministrator eller global administrator.<BR/>
    b. Bla til Azure Active Directory > **egenskaper**.<BR/>
    c. Velg **Behandle sikkerhetsstandarder**.<BR/>
    d. Angi **Aktiver sikkerhetsstandarder** til **Nei**.<BR/>
    e. Velg **Lagre**.

2. [Aktiver SMTP-klientinnsending](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) på den lisensierte postboksen.

    a. Fra Administrasjonssenter for Microsoft 365 går du til **Aktive brukere**, og velger brukeren.<BR/>
    b. Gå til E-post-fanen, og velg Behandle **e-postapper** under E-postapper . <BR/>
    d. Kontroller at **Godkjent SMTP er** avmerket (aktivert).<BR/>
    e. Velg **Lagre endringer**.<BR/>

3. [Deaktiver godkjenning med flere faktorer (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) på den lisensierte postboksen.

    a. Gå til Administrasjonssenter for Microsoft 365, og velg Brukere aktive brukere i navigasjonsmenyen  >  **til venstre.**<BR/>
    b. Velg **Godkjenning med flere faktorer**.<BR/>
    c. Velg brukeren, og deaktiver **godkjenning med flere faktorer**.<BR/>
