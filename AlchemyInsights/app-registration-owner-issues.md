---
title: Problemer med appregistreringseier
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404779"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="da1b4-102">Problemer med appregistreringseier</span><span class="sxs-lookup"><span data-stu-id="da1b4-102">App Registration Owner issues</span></span>

<span data-ttu-id="da1b4-103">Her er de tilgjengelige metodene for å legge til hovedstoler som eiere for appregistreringer:</span><span class="sxs-lookup"><span data-stu-id="da1b4-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="da1b4-104">Bruke Azure AD PowerShell-modulen –</span><span class="sxs-lookup"><span data-stu-id="da1b4-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="da1b4-105">Referanse: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="da1b4-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="da1b4-106">Bruke Azure CLI – `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="da1b4-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="da1b4-107">Referanse: [eier av az-annonseappen](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="da1b4-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="da1b4-108">Bruke MS Graph –</span><span class="sxs-lookup"><span data-stu-id="da1b4-108">Using MS Graph -</span></span>

    <span data-ttu-id="da1b4-109">Referanse: [Legg til eier – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="da1b4-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="da1b4-110">Bruke Azure AD Portal – Gå til [portal.azure.com](https://portal.azure.com/) > Azure Active Directory >-appregistrering > Velg programmet > Eiere > Legg til eiere</span><span class="sxs-lookup"><span data-stu-id="da1b4-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="da1b4-111">**Kan du ikke vise programmet på appregistreringsbladet selv om du er eieren av programmet?**</span><span class="sxs-lookup"><span data-stu-id="da1b4-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="da1b4-112">Eieren av en app er ikke en administrativ rolle.</span><span class="sxs-lookup"><span data-stu-id="da1b4-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="da1b4-113">Hvis innstillingen [Begrens tilgang](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) til administrasjonsportalen for Azure AD er aktivert, kan bare administrator vise programmene i appregistreringsportalen.</span><span class="sxs-lookup"><span data-stu-id="da1b4-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="da1b4-114">Hvis en eier skal kunne vise programmene, kan du enten deaktivere denne innstillingen (Angi denne til NEI) eller tilordne administratorrollen til eieren for bare det bestemte programmet.</span><span class="sxs-lookup"><span data-stu-id="da1b4-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="da1b4-115">Men for dette krever du en Azure AD Premium P2-lisens og aktiverer [privilegert identitetsbehandling.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="da1b4-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
