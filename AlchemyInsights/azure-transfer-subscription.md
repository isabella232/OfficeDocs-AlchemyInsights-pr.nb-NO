---
title: Overfør eierskap for Azure-fakturering
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
ms.openlocfilehash: 454ce626862bb4a2361abccd92ad0099b534388c
ms.sourcegitcommit: 059ad2936788266ea9714ec8c66d407d7261aeb6
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/29/2020
ms.locfileid: "49736887"
---
# <a name="transfer-azure-billing-ownership"></a>Overfør eierskap for Azure-fakturering

Logg på [Azure-portal](https://portal.azure.com/) som administrator av faktureringskontoen som har abonnementet du vil overføre. Hvis du ikke er sikker på om du er administrator, eller hvis du trenger å finne ut hvem som er, kan du se [Fastslå faktureringsadministrator for konto](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Søk på _Kostnadsadministrasjon + fakturering_.
1. Velg **Abonnementer** fra ruten til venstre. Avhengig av hvilken tilgang du har, kan det hende at du må velge et faktureringsomfang og deretter **Abonnementer** eller **Azure-abonnementer**.
1. Velg **Overfør eierskap for fakturering** for abonnementet du vil overføre.
1. Skriv inn e-postadressen til en bruker som er en faktureringsadministrator for kontoen som vil bli den nye eieren av abonnementet, og velg deretter **send overføringsforespørsel**.
1. Brukeren får en e-post med instruksjoner for å gjennomgå overføringsforespørselen din. For å godkjenne overføringsforespørselen klikker brukeren på koblingen i e-postmeldingen, og følger instruksjonene.

Vær oppmerksom på at hvis du overfører faktureringseier av abonnementet til en brukerkonto i en annen Azure AD-leier, vil alle [rollebasert tilgangskontroll (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)-oppgaver til å administrere ressurser i abonnementet bli fjernet. Bare den nye eieren får tilgang til å administrere ressurser i abonnementet. Hvis du vil ha mer informasjon om hvordan du endrer katalogen for et abonnement, se [Overføring av abonnement til en bruker i en annen Azure AD-leier](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Viktig innvirkning på fakturaene**_: Hvis du har overført faktureringseier for et Azure-abonnement, vil kostnadene dine være fordelt. Du får tilgang til fakturaene i henhold til følgende:  

1. Velg abonnementet fra [Abonnementer-siden](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) i Azure-portal som [en bruker med tilgang til fakturaer](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), og velg deretter **Faktura**.
1. Klikk **Last ned faktura** for å se en kopi av PDF-fakturaen. Hvis det står _Ikke tilgjengelig_, kan du se [Hvorfor ser jeg ikke en faktura for siste faktureringsperiode?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Du kan også vise daglig bruk ved å klikke på **faktureringsperiode** for å få en PDF-fil av fakturaen og en kopi av den detaljerte dagligbruksfilen (.CSV). Hvis du vil ha mer informasjon, kan du se [Få faktura-og bruker data](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Anbefalte dokumenter**

- [Overfør faktureringseier til et Azure-abonnement for en annen konto](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Om overføring av faktureringseier til et Azure-abonnement](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Overføring av Visual Studio, Microsoft Partner Network (MPN) og forbruksbetalte Dev/Test-abonnementer](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Vanlige spørsmål om overføring av eierskap](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Feilsøke problemer om overføring av eierskap](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
