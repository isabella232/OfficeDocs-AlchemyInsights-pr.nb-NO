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
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063682"
---
# <a name="issues-with-credentials"></a>Problemer med legitimasjon

[Microsoft identity platform and the OAuth 2.0 client credentials flow describes](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) how to program directly against the OAuth 2.0 client credentials grant flow.

**Hvordan behandler jeg passord eller sertifikatlegitimasjon for et program?**

I Azure CLI kan du bruke [az ad-app-legitimasjon](https://docs.microsoft.com/cli/azure/ad/app/credential) til å slette, liste opp eller tilbakestille passordet eller sertifikatlegitimasjonen til et program.

**Hvordan tilbakestiller brukerne passordene sine?**

Brukere må registrere [seg for selvbetjent tilbakestilling](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) av passord før de kan tilbakestille passordene sine. Når en bruker har registrert seg, kan de følge instruksjonene i denne artikkelen for å tilbakestille passordet: Tilbakestill [jobb- eller skolepassordet.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Hvordan endrer brukerne passordene sine?**

Brukere kan følge fremgangsmåten i denne artikkelen for å endre passordene sine: [Slik endrer du passordet.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
De kan også [administrere app-passord for totrinnskontroll.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Brukeren får en feilmelding når jeg endrer eller tilbakestiller passordet**

Denne koblingen gir informasjon om vanlige problemer som kan oppstå når en bruker prøver å tilbakestille passordet sitt: [Vanlige problemer og deres løsninger](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Jeg har problemer med å tilbakestille passordet til en bruker**

- Kontroller at du er autorisert til å tilbakestille passord. *Bare globale passord og brukeradministratorer kan tilbakestille brukerpassord.* Globale administratorer kan også tilbakestille passordene til andre privilegerte administratorer.

- Kontroller at du forstår lisensieringskravene:

  - Du må ha minst én lisens tilordnet i organisasjonen:
    - **Bare skybrukere** – alle Office 365 (O365) betalte SKU-er, eller Azure AD Basic
    - **Skybrukere og/eller** lokale brukere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
    - Hvis du vil lære mer om lisensieringskrav, kan du se Lisensieringskrav [for selvbetjent tilbakestilling av passord for Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Hvis du vil tilbakestille passordet til en bruker, kan du finne brukeren i Azure AD. Klikk deretter Tilbakestill passord-knappen på oversiktsbladet for denne brukeren.

**Knappen for tilbakestilling av passord er nedtonet**

Du har ikke tillatelse til **å** tilbakestille denne brukerens passord. *Bare globale passord og brukeradministratorer kan tilbakestille brukerpassord.* Globale administratorer kan også tilbakestille passordene til andre privilegerte administratorer.

**Jeg ser ikke blad for tilbakestilling av passord**

Du har ikke tillatelse til å tilbakestille passord. *Bare globale passord og brukeradministratorer kan tilbakestille brukerpassord.* Globale administratorer kan også tilbakestille passordene til andre privilegerte administratorer.

**Jeg ser ikke det lokale integrasjonsbladet i tilbakestilling av passord**

- Det lokale integreringsbladet vises bare i hybridmiljøer, det vil si at du bruker tilbakeskriving av passord til å manipulere lokale brukerpassord.

- Du ser ikke dette bladet hvis:

  - Du bruker ikke tilbakeskriving av passord
  - Det er et problem med installasjon/tilkobling av passord-writeback
  - Det er et problem med installasjonen/tilkoblingen til Azure AD Connect
  - Hvis du vil ha flere feilsøkingstrinn for problemer med tilbakeskriving av passord, kan du se [Feilsøke tilbakeskriving av passord](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Jeg vet ikke hvordan jeg tilbakestiller passordet til en bruker**

1. Logg på Azure Portal som en passende administrator.
2. Gå til **bladbladet Brukere og** grupper, og velg Alle **brukere.**
3. Velg en bruker fra listen.
4. Velg Oversikt for den valgte **brukeren,** og velg deretter Tilbakestill passord på **kommandolinjen.**
5. Velg Tilbakestill **passord-knappen,** og følg instruksjonene på skjermen.
    - Bare tilbakestillinger utført gjennom **Azure Portal støtter** tilbakeskriving av passord.

**Jeg tilbakestiller passordet til en lokal bruker fra administrasjonsportalen for Office 365 eller mobilappen for Office 365, men brukeren kan fremdeles ikke logge på**

Tilbakeskriving av passord støttes ikke i denne portalen. Tilbakestill brukerens passord på nytt i Azure Portal.
