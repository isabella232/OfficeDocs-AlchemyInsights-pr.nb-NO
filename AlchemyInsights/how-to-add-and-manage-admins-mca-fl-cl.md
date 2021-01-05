---
title: Slik legger du til og behandler administratorer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755504"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="45509-102">Slik legger du til og behandler administratorer</span><span class="sxs-lookup"><span data-stu-id="45509-102">How to add and manage admins</span></span>

<span data-ttu-id="45509-103">Basert på problem beskrivelsen har vi funnet en løsning for deg.</span><span class="sxs-lookup"><span data-stu-id="45509-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="45509-104">De fleste kunder kunne løse problemet sitt på egen hånd etter å ha følge dokumentasjonen vår.</span><span class="sxs-lookup"><span data-stu-id="45509-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="45509-105">Hvis du vil administrere betalings kontoen for en Microsoft Customer Agreement (MCA), kan du bruke forskjellige roller med det ønskede tilgangs nivået.</span><span class="sxs-lookup"><span data-stu-id="45509-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="45509-106">Disse rollene er i tillegg til de innebygde Azure-tjeneste rollene som hjelper deg med å kontrollere ressursene.</span><span class="sxs-lookup"><span data-stu-id="45509-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="45509-107">**Slik legger du til fakturerings roller i Azure-portalen:**</span><span class="sxs-lookup"><span data-stu-id="45509-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="45509-108">Logg deg på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="45509-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="45509-109">Søke etter *kostnads administrasjon + fakturering*.</span><span class="sxs-lookup"><span data-stu-id="45509-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="45509-110">Velg tilgangs kontroll (IAM) i et omfang, for eksempel fakturerings konto, fakturerings profil eller faktura del, der du vil gi tilgang.</span><span class="sxs-lookup"><span data-stu-id="45509-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="45509-111">Siden for tilgangs kontroll (IAM) viser brukere og grupper som er tilordnet hver rolle for området.</span><span class="sxs-lookup"><span data-stu-id="45509-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="45509-112">Hvis du vil gi tilgang til en bruker, velger du **Legg til** fra toppen av siden.</span><span class="sxs-lookup"><span data-stu-id="45509-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="45509-113">Velg en rolle i rulle gardin listen *rolle* .</span><span class="sxs-lookup"><span data-stu-id="45509-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="45509-114">Skriv inn e-postadressen til brukeren du vil gi tilgang til.</span><span class="sxs-lookup"><span data-stu-id="45509-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="45509-115">Velg **Lagre** for å tilordne rollen.</span><span class="sxs-lookup"><span data-stu-id="45509-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="45509-116">Hvis du vil fjerne tilgang for en bruker, velger du brukeren med rolle tildelingen du vil fjerne.</span><span class="sxs-lookup"><span data-stu-id="45509-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="45509-117">Velg **Fjern**.</span><span class="sxs-lookup"><span data-stu-id="45509-117">Select **Remove**.</span></span>

<span data-ttu-id="45509-118">**Anbefalte dokumenter**</span><span class="sxs-lookup"><span data-stu-id="45509-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="45509-119">Fakturerings rolle definisjoner</span><span class="sxs-lookup"><span data-stu-id="45509-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="45509-120">Konto roller og oppgaver for fakturering</span><span class="sxs-lookup"><span data-stu-id="45509-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="45509-121">Kom i gang med en MCA-fakturerings konto</span><span class="sxs-lookup"><span data-stu-id="45509-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="45509-122">Kontrollere tilgang til en Microsoft-kunde avtale</span><span class="sxs-lookup"><span data-stu-id="45509-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
