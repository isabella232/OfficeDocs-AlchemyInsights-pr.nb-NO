---
title: Abonnements typer som støttes
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807974"
---
# <a name="supported-subscription-types"></a>Abonnements typer som støttes

Se gjennom abonnements typene som støttes for å fortsette ytterligere.

[Abonnements typer som støttes](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Overføre eierskap for fakturering**

Azure-Portal som [konto administrator](https://ms.portal.azure.com/) for fakturerings kontoen som har abonnementet du vil overføre

- Søke om **kostnads administrasjon + fakturering** . Velg **abonnementer** fra venstre rute. Avhengig av tilgangen, kan det hende du må velge et fakturerings omfang og deretter **abonnementer** eller **Azure-abonnementer** .
- Velg Overfør fakturerings eierskap for abonnementet du vil overføre
- Skriv inn e-postadressen til en bruker som er fakturerings administrator for kontoen som skal være den nye eieren for abonnementet, og velg deretter **Send overførings forespørsel**
- Brukeren får en e-post med instruksjoner for å se gjennom overførings forespørselen. Brukeren velger koblingen i e-postmeldingen og følger instruksjonene for å godkjenne overførings forespørselen.

Obs! hvis du overfører fakturerings eierskapet for abonnementet til en brukers konto i en annen Azure AD-leier, fjernes alle [rolle BAS ert tilgangs kontroll (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) tildelinger for å administrere ressurser i abonnementet for godt. Det er bare den nye eieren som har tilgang til å administrere ressurser i abonnementet. Hvis du vil ha mer informasjon, kan du se [overføre abonnement til en bruker i en annen Azure ad-Tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Overføre eierskap av abonnement**

Overføring av eierskap for abonnements rolle BAS ert tilgang (RBAC) for å behandle ressurser i abonnementet mister tilgangen. Hvis du vil ha mer informasjon om å legge til et eksisterende abonnement i en Tenant, kan du se [knytte til eller legge til et Azure-abonnement i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Abonnements overføring med eksisterende ute stående beløp fra den gjeldende fakturerings syklusen, blir ikke overført til det nye betalings middelet i den nye kontoen. Den eneste informasjonen som er tilgjengelig for brukerne i ny konto, er den siste månedens kostnad for abonnementet. Resten av loggen for bruk og fakturering overføres ikke til abonnementet.
- Overføring av fakturerings eierskap for organisasjons avtale abonnement (EA) abonnementer støttes for øyeblikket bare i Enterprise Agreement-portalen
- Overføring av et kredit orientert abonnement som Visual Studio, BizSpark, Microsoft partner Network til en ny bruker krever at du har en Visual Studio/Microsoft partner Network-lisens til å godta overførings forespørselen
- Alle ressurser som virtuelle maskiner, disker og nett steder overføring til den nye kontoen er utført. Følgende ressurser kan bli påvirket i en kryss abonnements overføring:

**Azure AD Domain Services**

Azure-tasters hvelv

- [SQL-relaterte brukere og databaser](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) kan påvirkes, spesielt hvis kunden bruker en Azure Active Directory-relatert godkjenning
- **App-tjenester** som er konfigurert med Azure Active Directory-godkjenning, kan påvirkes
- **Visual Studio Team** Tjeneste kontoer som er koblet til Azure-abonnementer, kan miste tilgang midlertidig når det tilkoblede Azure-abonnementet avbrytes

**Anbefalte dokumenter**

Trinn etter å ha godtakelse av fakturerings eierskap:

- Hvis du vil beholde fakturerings eierskapet, men endre typen abonnement, kan du se: [bytte Azure-abonnementet til et annet tilbud](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Overføring av Visual Studio, Microsoft partner Network (MPN) og betal etter hvert, dev/test-abonnementer](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Overføre eierskap for fakturering av Enterprise Agreement (EA)-abonnementer](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Vanlige spørsmål om overføring av eierskap](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Feilsøke problemer med overførings eierskap](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)