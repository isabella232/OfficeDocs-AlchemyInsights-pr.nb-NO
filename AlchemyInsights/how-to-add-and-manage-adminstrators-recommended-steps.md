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
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="f85c8-102">Slik legger du til og administrerer administratorer – anbefalte trinn</span><span class="sxs-lookup"><span data-stu-id="f85c8-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="f85c8-103">Basert på problem beskrivelsen har vi funnet en løsning for deg.</span><span class="sxs-lookup"><span data-stu-id="f85c8-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="f85c8-104">De fleste kunder kunne løse problemet sitt på egen hånd etter å ha følge dokumentasjonen vår.</span><span class="sxs-lookup"><span data-stu-id="f85c8-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="f85c8-105">**Redigere abonnement administratoren eller medadministratoren**</span><span class="sxs-lookup"><span data-stu-id="f85c8-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="f85c8-106">Konto administratoren kan redigere begge rollene, men abonnement administratoren kan bare endre administratorer i [Azure-portalen](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="f85c8-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="f85c8-107">Legge til eller endre Azure-abonnements administratorer</span><span class="sxs-lookup"><span data-stu-id="f85c8-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="f85c8-108">**Oppdatere abonnement administratoren eller Co-Administrator for interne abonnementer (AIRS)**</span><span class="sxs-lookup"><span data-stu-id="f85c8-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="f85c8-109">Tjeneste administratoren eller medadministratoren kan selv betjene denne handlingen ved hjelp av følgende Fremgangs måte:</span><span class="sxs-lookup"><span data-stu-id="f85c8-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="f85c8-110">Logg på Azure- [portalen](https://ms.portal.azure.com/#home) , og klikk **kostnads behandling + fakturering** i det venstre blad.</span><span class="sxs-lookup"><span data-stu-id="f85c8-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="f85c8-111">Klikk linje elementet med abonnementet ditt.</span><span class="sxs-lookup"><span data-stu-id="f85c8-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="f85c8-112">Dette åpner oversikten for abonnementet ditt.</span><span class="sxs-lookup"><span data-stu-id="f85c8-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="f85c8-113">Klikk **Egenskaper** på **abonnements** blad.</span><span class="sxs-lookup"><span data-stu-id="f85c8-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="f85c8-114">Klikk på knappen **tjeneste administrator** .</span><span class="sxs-lookup"><span data-stu-id="f85c8-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="f85c8-115">Skriv inn e-postadressen til brukeren du vil angi som en tjeneste administrator, og klikk **OK**.</span><span class="sxs-lookup"><span data-stu-id="f85c8-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="f85c8-116">**Legge til/endre/fjerne medadministrator**</span><span class="sxs-lookup"><span data-stu-id="f85c8-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="f85c8-117">Logg deg på [Azure-portalen](https://ms.portal.azure.com/#home) som en tjeneste administrator.</span><span class="sxs-lookup"><span data-stu-id="f85c8-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="f85c8-118">Åpne [abonnementer](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) , og velg et abonnement.</span><span class="sxs-lookup"><span data-stu-id="f85c8-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="f85c8-119">(Medforfattere kan bare tilordnes til abonnements området.)</span><span class="sxs-lookup"><span data-stu-id="f85c8-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="f85c8-120">Gå til **tilgangs kontroll (iam)**  >  **klassiske administratorer**  >  **Legg**  >  **til medadministrator** for å åpne ruten **Legg til samtidig** administrator (Hvis alternativet for samtidighet er deaktivert, betyr det at du ikke har tilgang).</span><span class="sxs-lookup"><span data-stu-id="f85c8-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="f85c8-121">Velg brukeren du vil legge til, og klikk **Legg til**.</span><span class="sxs-lookup"><span data-stu-id="f85c8-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="f85c8-122">**få mer informasjon:**</span><span class="sxs-lookup"><span data-stu-id="f85c8-122">**Learn more:**</span></span>
- [<span data-ttu-id="f85c8-123">Legge til en medadministrator</span><span class="sxs-lookup"><span data-stu-id="f85c8-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="f85c8-124">Fjerne en medadministrator</span><span class="sxs-lookup"><span data-stu-id="f85c8-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="f85c8-125">Endre tjeneste administratoren</span><span class="sxs-lookup"><span data-stu-id="f85c8-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="f85c8-126">Vise konto administratoren</span><span class="sxs-lookup"><span data-stu-id="f85c8-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="f85c8-127">Behandle tilgang ved hjelp av RBAC og Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="f85c8-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="f85c8-128">**Legge til/slette brukere ved hjelp av Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="f85c8-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="f85c8-129">Du kan legge til nye brukere eller slette eksisterende brukere fra Azure Active Directory-organisasjonen (Azure AD):</span><span class="sxs-lookup"><span data-stu-id="f85c8-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="f85c8-130">Hvis du vil legge til en ny bruker, logger du deg på [Azure-portalen](https://ms.portal.azure.com/#home) som en bruker administrator for organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="f85c8-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="f85c8-131">Velg **Azure Active Directory**, velg **brukere** , og klikk deretter **ny bruker**.</span><span class="sxs-lookup"><span data-stu-id="f85c8-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="f85c8-132">Fyll ut den nødvendige informasjonen på **bruker** -siden.</span><span class="sxs-lookup"><span data-stu-id="f85c8-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="f85c8-133">Klikk **Opprett**.</span><span class="sxs-lookup"><span data-stu-id="f85c8-133">Click **Create**.</span></span> <span data-ttu-id="f85c8-134">Brukeren blir opprettet og lagt til i Azure AD-leieren din.</span><span class="sxs-lookup"><span data-stu-id="f85c8-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="f85c8-135">**Finn ut mer**:</span><span class="sxs-lookup"><span data-stu-id="f85c8-135">**Learn more**:</span></span>

- [<span data-ttu-id="f85c8-136">Legge til en ny bruker</span><span class="sxs-lookup"><span data-stu-id="f85c8-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="f85c8-137">Slette en bruker</span><span class="sxs-lookup"><span data-stu-id="f85c8-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="f85c8-138">Legge til eller oppdatere en brukers profil informasjon ved hjelp av Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="f85c8-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="f85c8-139">**Anbefalte dokumenter**</span><span class="sxs-lookup"><span data-stu-id="f85c8-139">**Recommended documents**</span></span>

- [<span data-ttu-id="f85c8-140">Hva er rolle BAS ert tilgangs kontroll (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="f85c8-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="f85c8-141">Forstå de ulike rollene i Azure</span><span class="sxs-lookup"><span data-stu-id="f85c8-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="f85c8-142">Administrator rolle tillatelser i Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="f85c8-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="f85c8-143">Opplæring: gi tilgang til en bruker ved hjelp av RBAC og Azure-portalen</span><span class="sxs-lookup"><span data-stu-id="f85c8-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="f85c8-144">Feilsøke RBAC i Azure</span><span class="sxs-lookup"><span data-stu-id="f85c8-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="f85c8-145">Organisere ressurser med administrasjons grupper for Azure</span><span class="sxs-lookup"><span data-stu-id="f85c8-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="f85c8-146">Slik ber du om kopi av Azure fakturaen via e-post</span><span class="sxs-lookup"><span data-stu-id="f85c8-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="f85c8-147">Slik legger du til, oppdaterer eller fjerner et kreditt kort eller et debetkort fra Azure</span><span class="sxs-lookup"><span data-stu-id="f85c8-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="f85c8-148">Behandle (reaktivere/avbryte/bytte) abonnement</span><span class="sxs-lookup"><span data-stu-id="f85c8-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



