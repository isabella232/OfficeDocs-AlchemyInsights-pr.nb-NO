---
title: Overføre eierskap for Azure-fakturering
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
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922164"
---
# <a name="transfer-azure-billing-ownership"></a>Overføre eierskap for Azure-fakturering

Logg deg på [Azure-portalen](https://portal.azure.com/) som administrator for fakturerings kontoen som har abonnementet du vil overføre. Hvis du ikke er sikker på om du er og administrator, eller hvis du må finne ut hvem som er, kan du se [bestemme konto fakturerings administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Søke om **kostnads administrasjon + fakturering**.
- Velg **abonnementer** fra venstre rute. Avhengig av tilgangen, kan det hende du må velge et fakturerings omfang og deretter **abonnementer** eller **Azure-abonnementer**.
- Velg **Overfør fakturerings eierskap** for abonnementet du vil overføre
- Skriv inn e-postadressen til en bruker som er fakturerings administrator for kontoen som skal være den nye eieren for abonnementet, og velg deretter **Send overførings forespørsel**
- Brukeren får en e-post med instruksjoner for å se gjennom overførings forespørselen. Brukeren velger koblingen i e-postmeldingen og følger instruksjonene for å godkjenne overførings forespørselen.

**Obs** ! hvis du overfører fakturerings eierskapet for abonnementet til en brukers konto i en annen Azure ad-leier, fjernes alle [rolle BAS ert tilgangs kontroll (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)tildelinger for å administrere ressurser i abonnementet for godt. Det er bare den nye eieren som har tilgang til å administrere ressurser i abonnementet. Hvis du vil ha mer informasjon, kan du se [overføre abonnement til en bruker i en annen Azure ad-Tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Anbefalte dokumenter**

- [Overføre fakturerings eierskap for et Azure-abonnement til en annen konto](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Om overføring av fakturerings eierskap for et Azure-abonnement](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Overføring av Visual Studio, Microsoft partner Network (MPN) og betal etter hvert, dev/test-abonnementer](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Vanlige spørsmål om overføring av eierskap](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Feilsøke problemer med overførings eierskap](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
