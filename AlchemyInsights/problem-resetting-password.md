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
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039975"
---
# <a name="problems-resetting-password"></a>Problemer med tilbakestilling av passord

Dette er noen av problemene du kan møte når du tilbakestiller passord og mulige løsninger:

**Jeg har et problem med tilbakestilling av passord som ikke dekkes i de andre kategoriene**

- Kontroller at du er autorisert til å tilbakestille passord. Bare globale, passord og brukeradministratorer kan tilbakestille brukerpassord. Globale administratorer kan også tilbakestille andre privilegerte administratorpassord.
- Kontroller at du forstår lisenskravene:
    - Du må ha minst én lisens tilordnet i organisasjonen
        - Skybrukere – alle Office 365 (O365) betalt SKU eller Azure AD Basic
        - Sky- og/eller lokale brukere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
        - Hvis du vil lese mer om lisensieringskrav, kan du se artikkelen [Lisenskrav for selvbetjent tilbakestilling](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)av passord for Azure AD.

**Jeg har problemer med å teste policyen for tilbakestilling av passord jeg har angitt**

- Nylig brukte policyer kan ta flere minutter å replikere på tvers av alle datasentre og sluttpunkter. Fysisk avstand fra datasenteret påvirker også hvor raskt endringer brukes.
- Test med en sluttbruker, ikke en administrator, og prøv med et lite sett med brukere. Policyene som er konfigurert i Azure-portalen, gjelder bare for sluttbrukere, ikke for administratorer. Microsoft håndhever en sterk standard policy for tilbakestilling av passord med to porter for enhver Azure-administratorrolle (eksempel: Global administrator, brukerstøtteadministrator, passordadministrator osv.)
    - Lær mer om [policyer for administratorer](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Jeg vil distribuere tilbakestilling av passord, men jeg vil ikke at brukerne skal registrere mer sikkerhetsinformasjon**

Forhåndsutligne data for brukerne, slik at de ikke trenger det! – Som administrator kan du angi telefon- og e-postegenskaper for brukerne før du ruller ut tilbakestilling av passord til organisasjonen. Du kan gjøre dette ved hjelp av en API, PowerShell eller Azure AD Koble til. Mer informasjon her:
- [Distribuere tilbakestilling av passord uten at brukerne må registrere seg](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Hvilke data som brukes av tilbakestilling av passord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tilbakestillingsknappen for passord er nedtonet**

Du har ikke tillatelse til å tilbakestille denne brukerens passord. Bare globale, passord og brukeradministratorer kan tilbakestille brukerpassord. Globale administratorer kan også tilbakestille andre privilegerte administratorpassord.

**Jeg ser ikke tilbakestillingsbladet for passord**

Du har ikke tillatelse til å tilbakestille passord. Bare globale, passord og brukeradministratorer kan tilbakestille brukerpassord. Globale administratorer kan også tilbakestille andre privilegerte administratorpassord.

**Jeg ser ikke det lokale integreringsbladet i tilbakestilling av passord**

- Det lokale integreringsbladet vises bare i hybridmiljøer , noe som betyr at du bruker tilbakeskriving av passord til å manipulere lokale brukerpassord.
- Du ser ikke dette bladet hvis:
    - Du bruker ikke tilbakeskriving av passord
    - Det er et problem med installasjon/tilkobling av passord writeback
    - Det er et problem med installasjonen/tilkoblingen til Azure AD Koble til
    - Hvis du vil ha flere feilsøkingstrinn for problemer med tilbakeskriving av passord, kan du se delen [Feilsøke tilbakeskriving av passord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jeg vet ikke hvordan jeg tilbakestiller passordet til en bruker**

1. Logg på Azure-portalen som en passende administrator.
1. Gå til blad for Brukere og grupper, og velg **Alle brukere**.
1. Velg en bruker fra listen.
1. Velg Oversikt for den valgte **brukeren,** og klikk deretter Tilbakestill passord på **kommandolinjen.**
1. Følg instruksjonene på skjermen.
    - Bare tilbakestillinger utført via Azure Portal støtter tilbakeskriving av passord.

**Jeg tilbakestiller passordet til en lokal bruker fra Office 365 Admin-portalen eller Office 365 mobilappen, men brukeren kan fortsatt ikke logge på**

Tilbakeskriving av passord støttes ikke i denne portalen. Tilbakestill brukerens passord på nytt i Azure-portalen – portal.azure.com

