---
title: Opprette bruker
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569740"
---
# <a name="create-user"></a><span data-ttu-id="e93e0-102">Opprette bruker</span><span class="sxs-lookup"><span data-stu-id="e93e0-102">Create user</span></span>

<span data-ttu-id="e93e0-103">**KUNNGJØRING:**</span><span class="sxs-lookup"><span data-stu-id="e93e0-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="e93e0-104">[Avvikling av støtte for WebView-pålogging fra Google fra og med 4. januar 2021.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="e93e0-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="e93e0-105">Test om appene kan bli påvirket ved å følge [Googles veiledning](https://go.microsoft.com/fwlink/?linkid=2157323) om testing av kompatibilitet.</span><span class="sxs-lookup"><span data-stu-id="e93e0-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="e93e0-106">Kontroller at du bruker systemets nettvisning eller systemleser når du logger på brukerne med forbrukerkontoer fra Google.</span><span class="sxs-lookup"><span data-stu-id="e93e0-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="e93e0-107">Hvis du vil ha mer informasjon, kan du se Problemer med å logge [på programmer bare ved hjelp av Chrome-nettleseren.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)</span><span class="sxs-lookup"><span data-stu-id="e93e0-107">For more information, see [Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="e93e0-108">**Jeg kan ikke opprette en ny bruker i Azure AD-katalogen**</span><span class="sxs-lookup"><span data-stu-id="e93e0-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="e93e0-109">Kontroller at du er autorisert til å opprette en ny standardbruker.</span><span class="sxs-lookup"><span data-stu-id="e93e0-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="e93e0-110">Bare rollen global administrator eller brukeradministrator i Azure Active Directory (AD) kan opprette en ny standardbruker.</span><span class="sxs-lookup"><span data-stu-id="e93e0-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="e93e0-111">Hvis du ikke er i en av disse rollene, kan du be en administrator om å legge deg til i en av disse rollene eller opprette den nye brukerkontoen for deg.</span><span class="sxs-lookup"><span data-stu-id="e93e0-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="e93e0-112">Kontroller at brukernavnet er i et domene som er bekreftet i Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e93e0-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="e93e0-113">Hvis du ikke har noen bekreftede egendefinerte domenenavn i Azure AD, kan du bruke det opprinnelige Azure AD-domenet, som slutter med \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="e93e0-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="e93e0-114">Kontroller at brukernavnet er i et domene som ikke er forbundsbasert til Azure AD fra den lokale AD-en.</span><span class="sxs-lookup"><span data-stu-id="e93e0-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="e93e0-115">Brukere kan ikke legges til i skyen med domenenavn som er forbundsbasert fra lokalt.</span><span class="sxs-lookup"><span data-stu-id="e93e0-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="e93e0-116">Kontroller at ingen andre brukere eller kontakter allerede har brukernavnet du vil tilordne til den nye brukeren.</span><span class="sxs-lookup"><span data-stu-id="e93e0-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="e93e0-117">Brukernavn må være unike på tvers av Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e93e0-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="e93e0-118">Se [Azure AD-roller og -administratorer](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e93e0-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="e93e0-119">Se [domenenavnene](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e93e0-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="e93e0-120">Se [gjennom overvåkingslogger](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for å se mer detaljert informasjon om en nylig opprettet eller slettet bruker, for eksempel hvem som utførte handlingen og når.</span><span class="sxs-lookup"><span data-stu-id="e93e0-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="e93e0-121">Hvis du vil ha mer informasjon om hvordan du legger til nye brukere, kan du se Bruke [Azure-portalen til å opprette en ny bruker i Azure AD.](/azure/active-directory/active-directory-users-create-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="e93e0-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="e93e0-122">[Administrative roller i Azure AD:](/azure/active-directory/active-directory-assign-admin-roles)Administratorrolletillatelser i Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e93e0-122">[Azure AD administrative roles](/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="e93e0-123">Du kan også [bruke Azure AD PowerShell til å opprette en ny bruker.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="e93e0-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
