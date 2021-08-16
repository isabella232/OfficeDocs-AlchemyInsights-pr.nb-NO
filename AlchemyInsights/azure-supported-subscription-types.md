---
title: Abonnementstyper som støttes
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
- "9003560"
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072169"
---
# <a name="supported-subscription-types"></a>Abonnementstyper som støttes

Se gjennom abonnementstypene som støttes, for å gå videre.

[Abonnementstyper som støttes](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Overfør eierskap for fakturering**

Azure-portalen som [kontoadministrator](https://ms.portal.azure.com/) for faktureringskontoen som har abonnementet du vil overføre

- Søk på **Kostnadsadministrasjon + fakturering**. Velg **Abonnementer** fra ruten til venstre. Avhengig av hvilken tilgang du har, kan det hende at du må velge et faktureringsomfang og deretter **Abonnementer** eller **Azure-abonnementer**.
- Velg Overfør eierskap for fakturering for abonnementet du vil overføre
- Skriv inn e-postadressen til en bruker som er en faktureringsadministrator for kontoen som vil bli den nye eieren for abonnementet, og velg deretter **send overføringsforespørsel**
- Brukeren får en e-post med instruksjoner for å gjennomgå overføringsforespørselen din. For å godkjenne overføringsforespørselen klikker brukeren på koblingen i e-postmeldingen, og følger instruksjonene.

Obs! Hvis du overfører eierskap for fakturering av abonnementet til en brukerkonto i en annen Azure AD-leier, vil alle [rollebaserte tilgangskontroll (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)-oppgaver for å administrere ressurser i abonnementet bli fjernet. Bare den nye eieren får tilgang til å administrere ressurser i abonnementet. Hvis du vil ha mer informasjon, kan du se [Overføring av abonnement til en bruker i en annen Azure AD-leier](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Overføre eierskap for abonnement**

Rollebasert tilgang (RBAC) for forutsetninger for overføring av abonnementseierskap for å administrere ressurser i abonnementet mister tilgangen. Hvis du vil ha mer informasjon om å legge til et eksisterende abonnement i en leier, kan du se [Knytte eller legge til et Azure-abonnement i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Overføring av abonnement med et eksisterende utestående beløp fra gjeldende faktureringssyklus vil ikke bli overført til det nye betalingsmidlet i den nye kontoen. Den eneste informasjonen som er tilgjengelig for brukerne i den nye kontoen, er siste måneders kostnad for abonnementet. Resten av forbruket og faktureringshistorikken overføres ikke med abonnementet.
- Overføre faktureringseierskap for abonnementer for foretaksavtale (EA) støttes for øyeblikket bare i portalen for foretaksavtalen
- Overføring av et kredittorientert abonnement, for eksempel Visual Studio, BizSpark, Microsoft Partner Network, til en ny bruker krever at du har en Visual Studio / Microsoft Partner-nettverkslisens for å godta overføringsforespørselen
- Alle ressurser som for eksempel virtuelle maskiner, disker og nettsteder, overføres til den nye kontoen. Følgende ressurser kan bli berørt i en abonnementsoverføring på tvers av leier:

**Azure AD Domain Services**

Azure Key Vaults

- [SQL-relaterte brukere og databaser](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) kan påvirkes, særlig hvis kunden bruker Azure Active Directory-relatert godkjenning.
- **App-tjenester** som er konfigurert med Azure Active Directory-godkjenning kan påvirkes.
- **Visual Studio Team**-tjenestekontoer som er koblet til Azure-abonnementer, kan midlertidig miste tilgang når det tilkoblede Azure-abonnementet kanselleres.

**Anbefalte dokumenter**

Trinn etter å ha godtatt faktureringseierskap:

- For å beholde faktureringseierskapet, men endre typen abonnement, kan du se: [Bytte Azure-abonnementet til et annet tilbud](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Overføring av Visual Studio, Microsoft Partner Network (MPN) og bruksbaserte Dev/Test-abonnementer](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Overføre faktureringseierskap for abonnementer for foretaksavtale (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Vanlige spørsmål om overføring av eierskap](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Feilsøke problemer om overføring av eierskap](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)