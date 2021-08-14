---
title: Problemer med legitimasjon
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986828"
---
# <a name="issues-with-credentials"></a>Problemer med legitimasjon

[Microsofts identitetsplattform og OAuth 2.0-klientlegitimasjonsflyten](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) beskriver hvordan du programmerer direkte mot OAuth 2.0-klientlegitimasjon gir flyt.

**Hvordan administrerer jeg passordet eller sertifikatlegitimasjonen for et program?**

I Azure CLI kan du bruke az-annonseapplegitimasjon til å slette, føre opp eller tilbakestille passordet eller sertifikatlegitimasjonen til et program. [](https://docs.microsoft.com/cli/azure/ad/app/credential)

**Hvordan tilbakestiller brukerne passordene sine?**

Brukere må registrere [seg for selvbetjent](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) tilbakestilling av passord før de kan tilbakestille passordene sine. Når en bruker har registrert seg, kan de følge instruksjonene i denne artikkelen for å tilbakestille passordet: Tilbakestille jobb- [eller skolepassordet.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Hvordan endrer brukerne passordene sine?**

Brukere kan følge trinnene i denne artikkelen for å endre passordene sine: [Slik endrer du passordet](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
De kan også [administrere app-passord for totrinnskontroll.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Brukeren får en feilmelding når jeg endrer eller tilbakestiller passordet**

Denne koblingen gir informasjon om vanlige problemer som kan oppstå når en bruker prøver å tilbakestille passordet sitt: [Vanlige problemer og deres løsninger](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Jeg har problemer med å tilbakestille passordet til en bruker**

- Kontroller at du har tillatelse til å tilbakestille passord. *Bare globale, passord og brukeradministratorer kan tilbakestille brukerpassord.* Globale administratorer kan også tilbakestille andre privilegerte administratorpassord.

- Kontroller at du forstår lisenskravene:

  - Du må ha minst én lisens tilordnet i organisasjonen:
    - **Skybrukere –** alle Office 365 (O365) betalt SKU eller Azure AD Basic
    - **Sky- og/eller lokale** brukere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
    - Hvis du vil lære mer om lisensieringskrav, kan du se [Lisenskrav for selvbetjent tilbakestilling](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)av passord for Azure AD.
- Hvis du vil tilbakestille passordet til en bruker, finner du brukeren i Azure AD. Klikk deretter tilbakestill passord-knappen på oversiktsbladet for denne brukeren.

**Tilbakestillingsknappen for passord er nedtonet**

Du har ikke tillatelse til å **tilbakestille** denne brukerens passord. *Bare globale, passord og brukeradministratorer kan tilbakestille brukerpassord.* Globale administratorer kan også tilbakestille andre privilegerte administratorpassord.

**Jeg ser ikke tilbakestillingsbladet for passord**

Du har ikke tillatelse til å tilbakestille passord. *Bare globale, passord og brukeradministratorer kan tilbakestille brukerpassord.* Globale administratorer kan også tilbakestille andre privilegerte administratorpassord.

**Jeg ser ikke det lokale integreringsbladet i tilbakestilling av passord**

- Det lokale integreringsbladet vises bare i hybridmiljøer , noe som betyr at du bruker tilbakeskriving av passord til å manipulere lokale brukerpassord.

- Du ser ikke dette bladet hvis:

  - Du bruker ikke tilbakeskriving av passord
  - Det er et problem med installasjon/tilkobling av passord writeback
  - Det er et problem med installasjonen/tilkoblingen til Azure AD Koble til
  - Hvis du vil ha flere feilsøkingstrinn for problemer med tilbakeskriving av passord, kan du se [Feilsøke tilbakeskriving av passord](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Jeg vet ikke hvordan jeg tilbakestiller passordet til en bruker**

1. Logg på Azure-portalen som en passende administrator.
2. Gå til **blad for Brukere og** grupper, og velg Alle **brukere**.
3. Velg en bruker fra listen.
4. Velg Oversikt for den valgte **brukeren,** og velg deretter Tilbakestill passord på **kommandolinjen.**
5. Velg Tilbakestill **passord-knappen,** og følg instruksjonene på skjermen.
    - Bare tilbakestillinger utført via **Azure Portal støtter** tilbakeskriving av passord.

**Jeg tilbakestiller passordet til en lokal bruker fra Office 365 Admin-portalen eller Office 365 mobilappen, men brukeren kan fortsatt ikke logge på**

Tilbakeskriving av passord støttes ikke i denne portalen. Tilbakestill brukerens passord på nytt i Azure-portalen.
