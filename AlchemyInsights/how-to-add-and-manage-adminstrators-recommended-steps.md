---
title: Slik legger du til og administrerer administratorer – anbefalte trinn
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 5aa6f11d31ed62078fdd05090af5722289544c5ab2244a369182f4e0f9214183
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963796"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Slik legger du til og administrerer administratorer – anbefalte trinn

Basert på beskrivelsen av problemet har vi funnet en løsning for deg. De fleste kunder kunne løse problemet på egen hånd etter å ha fulgt dokumentasjonen vår.

**Redigere abonnementsadministratoren eller medadministratoren**

- Kontoadministratoren kan redigere begge rollene, mens abonnementsadministratoren bare kan endre medadministratorer i [Azure-portalen.](https://ms.portal.azure.com/#home)
- [Legge til eller endre Azure-abonnementsadministratorer](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Oppdatere abonnementsadministratoren eller Co-Administrator for interne abonnementer (AIRS)**

Tjenesteadministratoren eller medadministratoren kan selvbetjente denne handlingen ved hjelp av følgende fremgangsmåte:

1. Logg på [Azure-portalen,](https://ms.portal.azure.com/#home) og klikk **Kostnadsstyring + Fakturering** i venstre blad.
2. Klikk linjeelementet med abonnementet. Dette åpner oversikten for abonnementet.
3. Klikk Egenskaper på Abonnement-bladet.   
4. Klikk **tjenesteadministrator-knappen.**
5. Skriv inn e-postmeldingen til brukeren du vil angi som tjenesteadministrator, og klikk **OK**.

**Legge til/endre/fjerne medadministrator**

1. Logg på [Azure-portalen](https://ms.portal.azure.com/#home) som tjenesteadministrator.
2. Åpne [Abonnementer,](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) og velg et abonnement. (Medadministratorer kan bare tilordnes i abonnementsomfanget.)
3. Gå til  >    >    >   **Access-kontroll** (IAM) Klassiske administratorer Legg til medadministrator for å åpne ruten Legg til medadministrator (Hvis alternativet Legg til medadministrator er deaktivert, betyr det at du ikke har tillatelser).
4. Velg brukeren du vil legge til, og klikk Legg **til**.

**få mer informasjon:**
- [Legge til en medadministrator](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Fjerne en medadministrator](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Endre tjenesteadministratoren](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Vis kontoadministratoren](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Administrere tilgang ved hjelp av RBAC og Azure Portal](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Legge til/slette brukere ved hjelp av Azure Active Directory (AD)**

Du kan legge til nye brukere eller slette eksisterende brukere fra Azure Active Directory (Azure AD)-organisasjonen:

1. Hvis du vil legge til en ny bruker, logger du på [Azure-portalen](https://ms.portal.azure.com/#home) som brukeradministrator for organisasjonen.
2. Velg **Azure Active Directory**, velg **Brukere,** og klikk deretter **Ny bruker**.
3. Fyll ut **den** nødvendige informasjonen på Bruker-siden. Klikk **Opprett**. Brukeren opprettes og legges til i Azure AD-leieren.

**Finn ut mer:**

- [Legge til en ny bruker](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Slette en bruker](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Legge til eller oppdatere en brukers profilinformasjon ved hjelp av Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Anbefalte dokumenter**

- [Hva er rollebasert tilgangskontroll (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Forstå de ulike rollene i Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Administratorrolletillatelser i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Opplæring: Gi tilgang til en bruker ved hjelp av RBAC og Azure-portalen](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Feilsøke RBAC i Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organisere ressursene dine med Azure-administrasjonsgrupper](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Slik ber du om kopi av Azure-faktura via e-post](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Slik legger du til, oppdaterer eller fjerner et kreditt- eller debetkort fra Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Behandle (aktivere på nytt/avbryte/bytte) abonnement](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



