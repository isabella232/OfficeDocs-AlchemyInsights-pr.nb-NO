---
title: Abonnements tilgang
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807716"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="15661-102">Kan ikke logge på Azure på grunn av nett leser problemer (nett leser henger, beholder rotering, lastes ikke inn, osv.)</span><span class="sxs-lookup"><span data-stu-id="15661-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="15661-103">Du kan bli påvirket av brudd.</span><span class="sxs-lookup"><span data-stu-id="15661-103">You might be impacted by an outage.</span></span> <span data-ttu-id="15661-104">Kontroller om det oppstår et løpende avbrudd: [Azure Health-status](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="15661-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="15661-105">Logg av alle aktive Azure-økter.</span><span class="sxs-lookup"><span data-stu-id="15661-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="15661-106">Start en privat eller inkognito modus for nett leseren.</span><span class="sxs-lookup"><span data-stu-id="15661-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="15661-107">Du kan også prøve å oppdatere nett leseren, bruke en annen nett leser, slette hurtig buffer informasjons kapsler hvis ovenfor ikke fungerer.</span><span class="sxs-lookup"><span data-stu-id="15661-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="15661-108">Les mer: [Feilsøke påloggings problemer](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="15661-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="15661-109">**Får ikke tilgang til abonnementer**</span><span class="sxs-lookup"><span data-stu-id="15661-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="15661-110">I [Azure-portalen](https://portal.azure.com/)må du kontrollere at riktig Azure-katalog er valgt fra kontoen øverst til høyre.</span><span class="sxs-lookup"><span data-stu-id="15661-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="15661-111">I [Azure-konto senteret](https://account.windowsazure.com/Subscriptions)kontrollerer du at kontoen som brukes, er konto administratoren.</span><span class="sxs-lookup"><span data-stu-id="15661-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="15661-112">Finn ut mer: [Feilsøke ingen abonnementer funnet](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="15661-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="15661-113">**Får ikke tilgang til fakturerings loggen**</span><span class="sxs-lookup"><span data-stu-id="15661-113">**Unable to access billing history**</span></span>

<span data-ttu-id="15661-114">Konto administratoren må sørge for at brukeren som har tilgang til fakturerings informasjonen, legges til i Azure Active Directory som gjeste bruker: [legge til eller slette en ny bruker](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="15661-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="15661-115">Brukeren må deretter gis en global administrator rolle: [Tilordne rolle til brukere](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="15661-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="15661-116">Legg inn dette, kan brukeren få tilgang til fakturering ved hjelp av RBAC-policyer: [gi tilgang til fakturering](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="15661-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="15661-117">**Anbefalte dokumenter**</span><span class="sxs-lookup"><span data-stu-id="15661-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="15661-118">Jeg kan ikke logge på for å administrere Azure-abonnementet mitt</span><span class="sxs-lookup"><span data-stu-id="15661-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)