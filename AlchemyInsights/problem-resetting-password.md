---
title: Problem med tilbakestilling av passord
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696272"
---
# <a name="problems-resetting-password"></a>Problemer med å tilbakestille passord

Nedenfor finner du noen av problemene du kan møte på når du tilbakestiller passord og mulige løsninger:

**Jeg har et problem med tilbakestilling av passord, som ikke dekkes i de andre kategoriene**

- Kontroller at du er autorisert til å tilbakestille passord. Bare globale passord og brukeradministratorer kan tilbakestille brukerpassord. Globale administratorer kan også tilbakestille passordene til andre privilegerte administratorer.
- Kontroller at du forstår lisensieringskravene:
    - Du må ha minst én lisens tilordnet i organisasjonen
        - Bare skybrukere – alle Office 365 (O365) betalte SKU-er, eller Azure AD Basic
        - Skybrukere og/eller lokale brukere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
        - Hvis du vil lese mer om lisensieringskrav, kan du se artikkelen Lisensieringskrav [for selvbetjent tilbakestilling av](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)passord for Azure AD.

**Jeg har problemer med å teste policyen for tilbakestilling av passord jeg har angitt**

- Det kan ta flere minutter å replikere nylig brukte policyer på tvers av alle datasentre og sluttpunkter. Fysisk avstand fra datasenteret påvirker også hvor raskt endringer brukes.
- Test med en sluttbruker, ikke en administrator, og pilot med et lite sett med brukere. Policyene som er konfigurert i Azure Portal, gjelder BARE for sluttbrukere, ikke administratorer. Microsoft håndhever en sterk policy for tilbakestilling av passord med to porter for en hvilken som helst Azure-administratorrolle (eksempel: Global administrator, Brukerstøtteadministrator, passordadministrator osv.)
    - Lær mer om [policyer for administratorer.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Jeg ønsker å distribuere tilbakestilling av passord, men jeg ønsker ikke at brukerne mine skal registrere mer sikkerhetsinformasjon**

Forhåndsutmuler data for brukerne, slik at de ikke trenger å gjøre det! – Som administrator kan du angi telefon- og e-postegenskaper for brukerne før du ruller ut tilbakestilling av passord til organisasjonen. Du kan gjøre dette ved hjelp av en API, PowerShell eller Azure AD Connect. Mer informasjon her:
- [Distribuere tilbakestilling av passord uten at brukere må registrere seg](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Hvilke data som brukes av tilbakestilling av passord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Knappen for tilbakestilling av passord er nedtonet**

Du har ikke tillatelse til å tilbakestille denne brukerens passord. Bare globale passord og brukeradministratorer kan tilbakestille brukerpassord. Globale administratorer kan også tilbakestille passordene til andre privilegerte administratorer.

**Jeg ser ikke blad for tilbakestilling av passord**

Du har ikke tillatelse til å tilbakestille passord. Bare globale passord og brukeradministratorer kan tilbakestille brukerpassord. Globale administratorer kan også tilbakestille passordene til andre privilegerte administratorer.

**Jeg ser ikke det lokale integrasjonsbladet i tilbakestilling av passord**

- Det lokale integreringsbladet vises bare i hybridmiljøer, det vil si at du bruker tilbakeskriving av passord til å manipulere lokale brukerpassord.
- Du ser ikke dette bladet hvis:
    - Du bruker ikke tilbakeskriving av passord
    - Det er et problem med installasjon/tilkobling av passord-writeback
    - Det er et problem med installasjonen/tilkoblingen til Azure AD Connect
    - Hvis du vil ha flere feilsøkingstrinn for problemer med tilbakeskriving av passord, kan du se delen [Feilsøke passordskriving](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jeg vet ikke hvordan jeg tilbakestiller passordet til en bruker**

1. Logg på Azure Portal som en passende administrator.
1. Gå til bladbladet Brukere og grupper, og velg **Alle brukere.**
1. Velg en bruker fra listen.
1. Velg Oversikt for den valgte **brukeren,** og klikk deretter Tilbakestill passord på **kommandolinjen.**
1. Følg instruksjonene på skjermen.
    - Bare tilbakestillinger utført gjennom Azure Portal støtter tilbakeskriving av passord.

**Jeg tilbakestiller passordet til en lokal bruker fra administrasjonsportalen for Office 365 eller mobilappen for Office 365, men brukeren kan fremdeles ikke logge på**

Tilbakeskriving av passord støttes ikke i denne portalen. Tilbakestill brukerens passord på nytt i Azure Portal – portal.azure.com

