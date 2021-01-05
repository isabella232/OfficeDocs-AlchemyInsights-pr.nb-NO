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
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755844"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Slik legger du til og administrerer administratorer – anbefalte trinn

Basert på problem beskrivelsen har vi funnet en løsning for deg. De fleste kunder kunne løse problemet sitt på egen hånd etter å ha følge dokumentasjonen vår.

**Redigere abonnement administratoren eller medadministratoren**

- Konto administratoren kan redigere begge rollene, men abonnement administratoren kan bare endre administratorer i [Azure-portalen](https://ms.portal.azure.com/#home).
- [Legge til eller endre Azure-abonnements administratorer](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Oppdatere abonnement administratoren eller Co-Administrator for interne abonnementer (AIRS)**

Tjeneste administratoren eller medadministratoren kan selv betjene denne handlingen ved hjelp av følgende Fremgangs måte:

1. Logg på Azure- [portalen](https://ms.portal.azure.com/#home) , og klikk **kostnads behandling + fakturering** i det venstre blad.
2. Klikk linje elementet med abonnementet ditt. Dette åpner oversikten for abonnementet ditt.
3. Klikk **Egenskaper** på **abonnements** blad. 
4. Klikk på knappen **tjeneste administrator** .
5. Skriv inn e-postadressen til brukeren du vil angi som en tjeneste administrator, og klikk **OK**.

**Legge til/endre/fjerne medadministrator**

1. Logg deg på [Azure-portalen](https://ms.portal.azure.com/#home) som en tjeneste administrator.
2. Åpne [abonnementer](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) , og velg et abonnement. (Medforfattere kan bare tilordnes til abonnements området.)
3. Gå til **tilgangs kontroll (iam)**  >  **klassiske administratorer**  >  **Legg**  >  **til medadministrator** for å åpne ruten **Legg til samtidig** administrator (Hvis alternativet for samtidighet er deaktivert, betyr det at du ikke har tilgang).
4. Velg brukeren du vil legge til, og klikk **Legg til**.

**få mer informasjon:**
- [Legge til en medadministrator](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Fjerne en medadministrator](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Endre tjeneste administratoren](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Vise konto administratoren](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Behandle tilgang ved hjelp av RBAC og Azure-Portal](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Legge til/slette brukere ved hjelp av Azure Active Directory (AD)**

Du kan legge til nye brukere eller slette eksisterende brukere fra Azure Active Directory-organisasjonen (Azure AD):

1. Hvis du vil legge til en ny bruker, logger du deg på [Azure-portalen](https://ms.portal.azure.com/#home) som en bruker administrator for organisasjonen.
2. Velg **Azure Active Directory**, velg **brukere** , og klikk deretter **ny bruker**.
3. Fyll ut den nødvendige informasjonen på **bruker** -siden. Klikk **Opprett**. Brukeren blir opprettet og lagt til i Azure AD-leieren din.

**Finn ut mer**:

- [Legge til en ny bruker](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Slette en bruker](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Legge til eller oppdatere en brukers profil informasjon ved hjelp av Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Anbefalte dokumenter**

- [Hva er rolle BAS ert tilgangs kontroll (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Forstå de ulike rollene i Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Administrator rolle tillatelser i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Opplæring: gi tilgang til en bruker ved hjelp av RBAC og Azure-portalen](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Feilsøke RBAC i Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organisere ressurser med administrasjons grupper for Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Slik ber du om kopi av Azure fakturaen via e-post](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Slik legger du til, oppdaterer eller fjerner et kreditt kort eller et debetkort fra Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Behandle (reaktivere/avbryte/bytte) abonnement](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



