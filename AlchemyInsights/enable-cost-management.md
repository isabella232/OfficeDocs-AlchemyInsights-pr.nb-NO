---
title: Aktivere kostnads styring
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677741"
---
# <a name="enable-cost-management"></a><span data-ttu-id="7822c-102">Aktivere kostnads styring</span><span class="sxs-lookup"><span data-stu-id="7822c-102">Enable cost management</span></span>

<span data-ttu-id="7822c-103">**Hva er kostnadene deaktivert for organisasjonen?**</span><span class="sxs-lookup"><span data-stu-id="7822c-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="7822c-104">Organisasjoner som bruker Enterprise Agreement (EA) eller MCA-kontoer (Microsoft Customer Agreement), kan deaktivere tilgang til kostnads informasjon og pris informasjon.</span><span class="sxs-lookup"><span data-stu-id="7822c-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="7822c-105">Når du logger deg på Azure-portalen, kan de bruke fakturerings-APIene til å få fakturaer i en programmatisk (når det er registrert) og bruks detaljer.</span><span class="sxs-lookup"><span data-stu-id="7822c-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="7822c-106">**Slik tillater du at flere brukere får tilgang til fakturaer**</span><span class="sxs-lookup"><span data-stu-id="7822c-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="7822c-107">Gå til **abonnements blad** i Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="7822c-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="7822c-108">Velg **fakturaer** og deretter **tilgang til fakturaer**.</span><span class="sxs-lookup"><span data-stu-id="7822c-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="7822c-109">Slå på Access, etterfulgt av endringer, slik at brukere i abonnements relaterte roller kan laste ned fakturaer.</span><span class="sxs-lookup"><span data-stu-id="7822c-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="7822c-110">Konto administratoren kan også konfigurere til å få fakturaer sendt via e-post.</span><span class="sxs-lookup"><span data-stu-id="7822c-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="7822c-111">Hvis du vil ha mer informasjon, kan du se [få fakturaen i e-post](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="7822c-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="7822c-112">**Slik legger du til brukere i rollen som fakturerings leser**</span><span class="sxs-lookup"><span data-stu-id="7822c-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="7822c-113">Gå til **abonnements blad** i Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="7822c-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="7822c-114">Velg **tilgangs kontroll (iam)** , og klikk deretter **Legg til**.</span><span class="sxs-lookup"><span data-stu-id="7822c-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="7822c-115">Velg **fakturerings leser** på siden **Velg en rolle** .</span><span class="sxs-lookup"><span data-stu-id="7822c-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="7822c-116">Skriv inn e-postadressen til brukeren du vil invitere, og klikk deretter **OK** for å sende invitasjonen.</span><span class="sxs-lookup"><span data-stu-id="7822c-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="7822c-117">Følg instruksjonene som er oppgitt i invitasjons-e-post for å logge på som en fakturerings leser.</span><span class="sxs-lookup"><span data-stu-id="7822c-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="7822c-118">Hvis du vil ha mer informasjon, kan du se [gi tilgang til fakturering](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="7822c-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="7822c-119">**Anbefalte dokumenter**</span><span class="sxs-lookup"><span data-stu-id="7822c-119">**Recommended documents**</span></span>

- [<span data-ttu-id="7822c-120">Aktiver DA og AO visninger via Enterprise Portal</span><span class="sxs-lookup"><span data-stu-id="7822c-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="7822c-121">Kostnader som er inkludert i kostnads styring</span><span class="sxs-lookup"><span data-stu-id="7822c-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="7822c-122">Støttet Microsoft Azure-tilbud</span><span class="sxs-lookup"><span data-stu-id="7822c-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="7822c-123">Se gjennom kostnader i kostnads analyse</span><span class="sxs-lookup"><span data-stu-id="7822c-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="7822c-124">Gi tilgang til fakturerings informasjon</span><span class="sxs-lookup"><span data-stu-id="7822c-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="7822c-125">Kontrollere tilgang til en Microsoft-kunde avtale</span><span class="sxs-lookup"><span data-stu-id="7822c-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






