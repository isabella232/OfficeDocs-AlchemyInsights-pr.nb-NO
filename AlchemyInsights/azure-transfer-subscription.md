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
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="85f68-102">Overføre eierskap for Azure-fakturering</span><span class="sxs-lookup"><span data-stu-id="85f68-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="85f68-103">Logg deg på [Azure-portalen](https://portal.azure.com/) som administrator for fakturerings kontoen som har abonnementet du vil overføre.</span><span class="sxs-lookup"><span data-stu-id="85f68-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="85f68-104">Hvis du ikke er sikker på om du er og administrator, eller hvis du må finne ut hvem som er, kan du se [bestemme konto fakturerings administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="85f68-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="85f68-105">Søke om **kostnads administrasjon + fakturering**.</span><span class="sxs-lookup"><span data-stu-id="85f68-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="85f68-106">Velg **abonnementer** fra venstre rute.</span><span class="sxs-lookup"><span data-stu-id="85f68-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="85f68-107">Avhengig av tilgangen, kan det hende du må velge et fakturerings omfang og deretter **abonnementer** eller **Azure-abonnementer**.</span><span class="sxs-lookup"><span data-stu-id="85f68-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="85f68-108">Velg **Overfør fakturerings eierskap** for abonnementet du vil overføre</span><span class="sxs-lookup"><span data-stu-id="85f68-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="85f68-109">Skriv inn e-postadressen til en bruker som er fakturerings administrator for kontoen som skal være den nye eieren for abonnementet, og velg deretter **Send overførings forespørsel**</span><span class="sxs-lookup"><span data-stu-id="85f68-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="85f68-110">Brukeren får en e-post med instruksjoner for å se gjennom overførings forespørselen.</span><span class="sxs-lookup"><span data-stu-id="85f68-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="85f68-111">Brukeren velger koblingen i e-postmeldingen og følger instruksjonene for å godkjenne overførings forespørselen.</span><span class="sxs-lookup"><span data-stu-id="85f68-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="85f68-112">**Obs** ! hvis du overfører fakturerings eierskapet for abonnementet til en brukers konto i en annen Azure ad-leier, fjernes alle [rolle BAS ert tilgangs kontroll (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)tildelinger for å administrere ressurser i abonnementet for godt.</span><span class="sxs-lookup"><span data-stu-id="85f68-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="85f68-113">Det er bare den nye eieren som har tilgang til å administrere ressurser i abonnementet.</span><span class="sxs-lookup"><span data-stu-id="85f68-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="85f68-114">Hvis du vil ha mer informasjon, kan du se [overføre abonnement til en bruker i en annen Azure ad-Tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="85f68-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="85f68-115">**Anbefalte dokumenter**</span><span class="sxs-lookup"><span data-stu-id="85f68-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="85f68-116">Overføre fakturerings eierskap for et Azure-abonnement til en annen konto</span><span class="sxs-lookup"><span data-stu-id="85f68-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="85f68-117">Om overføring av fakturerings eierskap for et Azure-abonnement</span><span class="sxs-lookup"><span data-stu-id="85f68-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="85f68-118">Overføring av Visual Studio, Microsoft partner Network (MPN) og betal etter hvert, dev/test-abonnementer</span><span class="sxs-lookup"><span data-stu-id="85f68-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="85f68-119">Vanlige spørsmål om overføring av eierskap</span><span class="sxs-lookup"><span data-stu-id="85f68-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="85f68-120">Feilsøke problemer med overførings eierskap</span><span class="sxs-lookup"><span data-stu-id="85f68-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
