---
title: Slett Tenant
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564615"
---
# <a name="delete-tenant"></a><span data-ttu-id="9ad86-102">Slett Tenant</span><span class="sxs-lookup"><span data-stu-id="9ad86-102">Delete tenant</span></span>

<span data-ttu-id="9ad86-103">Hvis du vil slette en Azure AD, må du kontrollere følgende:</span><span class="sxs-lookup"><span data-stu-id="9ad86-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="9ad86-104">Du er en global administrator på katalogen.</span><span class="sxs-lookup"><span data-stu-id="9ad86-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="9ad86-105">Du er ikke logget på med en konto som har standard katalogen, for eksempel contoso.onmicrosoft.com i den påloggede kontoen, for eksempel admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="9ad86-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="9ad86-106">Fjern alle aktive programmer i katalogen før sletting.</span><span class="sxs-lookup"><span data-stu-id="9ad86-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="9ad86-107">Hvis du vil fjerne aktive programmer, går du til app-registreringer og fjerner eksisterende programmer.</span><span class="sxs-lookup"><span data-stu-id="9ad86-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="9ad86-108">Det finnes ingen aktive abonnementer for noen Microsoft Online-tjenester, for eksempel Microsoft Azure, Office 365 eller Azure AD Premium, som er knyttet til katalogen.</span><span class="sxs-lookup"><span data-stu-id="9ad86-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="9ad86-109">Overfør abonnementene dine eller ekspedere annulleringer av aktive abonnementer via Azure kunde støtte og fakturering.</span><span class="sxs-lookup"><span data-stu-id="9ad86-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="9ad86-110">Finn ut mer om hvordan du avbryter Office-365 og Azure-abonnementer.</span><span class="sxs-lookup"><span data-stu-id="9ad86-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="9ad86-111">Hvis du vil ha veiledning om hvordan du knytter eller legger til et eksisterende abonnement på en leier, kan du se [knytte til eller legge til et Azure-abonnement i Azure ad-leieren](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="9ad86-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="9ad86-112">Det er ingen aktiv lisens.</span><span class="sxs-lookup"><span data-stu-id="9ad86-112">There are no Active license.</span></span> <span data-ttu-id="9ad86-113">Hvis du vil fjerne lisenser, kan du se [hvordan du fjerner abonnementet for å fjerne lisensen](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="9ad86-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="9ad86-114">Det er ingen andre aktive brukere i katalogen enn deg selv som den globale administratoren når du prøver å slette Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9ad86-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="9ad86-115">Fjern alle andre aktive brukere, og eventuelle avhengigheter i et egen definert domene navn i leieren må også fjernes, for eksempel brukere som er opprettet med admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="9ad86-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="9ad86-116">Hvis du vil ha mer informasjon om hvordan du gjør følgende:</span><span class="sxs-lookup"><span data-stu-id="9ad86-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="9ad86-117">Slett Azure Active Directory eller abonnement, se [slette Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="9ad86-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="9ad86-118">Hvis du fjerner programmer i katalogen, kan du se [fjerne programmer](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="9ad86-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
