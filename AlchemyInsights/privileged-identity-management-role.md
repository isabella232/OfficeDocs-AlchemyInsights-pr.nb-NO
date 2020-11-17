---
title: Rolle for privilegert identitets behandling
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088878"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="4e0cb-102">PIM-rolle (Privileged Identity Management)</span><span class="sxs-lookup"><span data-stu-id="4e0cb-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="4e0cb-103">**Tillatelser gis ikke etter aktivering av en rolle**</span><span class="sxs-lookup"><span data-stu-id="4e0cb-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="4e0cb-104">Når du aktiverer en rolle i Azure AD Privileged Identity Management (PIM), kan det hende at aktiveringen ikke overføres direkte til alle portaler som krever rollen som privilegerte rettigheter.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="4e0cb-105">Noen ganger, selv om endringen er overført, kan Web buffer i en portal føre til at endringen trer i kraft umiddelbart.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="4e0cb-106">Hvis aktiveringen er forsinket, følger du disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="4e0cb-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="4e0cb-107">Logg av Azure-portalen, og logg deretter på igjen.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="4e0cb-108">Når du aktiverer en Azure AD-rolle eller en Azure-ressurs rolle, vil du se trinnene for aktiveringen.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="4e0cb-109">Når alle trinnene er fullført, vil du se koblingen Logg av.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="4e0cb-110">Du kan bruke denne koblingen til å logge av. Dette vil løse de fleste tilfeller for aktiverings forsinkelse.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="4e0cb-111">Kontroller at du er oppført som medlem av rollen i PIM.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="4e0cb-112">Hvis du aktiverer Exchange Administrator-rollen, må du passe på at du logger av og logger deg på igjen.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="4e0cb-113">Hvis problemet vedvarer, åpner du en støtte forespørsel og opphever dette som et problem.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="4e0cb-114">Hvis du bruker Exchange Administrator-rollen til å få tilgang til sikkerhets-og Samsvars senteret, kan du se neste trinn.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="4e0cb-115">Hvis du aktiverer en rolle for å få tilgang til sikkerhets-og Samsvars senteret, eller hvis du aktiverer SharePoint-Administrator rollen, får du noen timer på opptil et par minutter.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="4e0cb-116">Dette er et kjent problem, og vi jobber aktivt med disse teamene for å løse dette problemet så snart som mulig.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="4e0cb-117">Hvis du vil ha mer informasjon, kan du ta en titt på:</span><span class="sxs-lookup"><span data-stu-id="4e0cb-117">For more information, see:</span></span>

- [<span data-ttu-id="4e0cb-118">Aktivere mine Azure AD-roller i PIM</span><span class="sxs-lookup"><span data-stu-id="4e0cb-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="4e0cb-119">Aktivere mine Azure-ressurser-roller i PIM</span><span class="sxs-lookup"><span data-stu-id="4e0cb-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="4e0cb-120">**Tillatelser fjernes ikke etter at en rolle er deaktivert eller rolle aktiveringen utløper**</span><span class="sxs-lookup"><span data-stu-id="4e0cb-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="4e0cb-121">Når du deaktiverer en rolle i Azure AD Privileged Identity Management eller når en aktiverings periode for en rolle utløper, kan det oppstå en forsinkelse der du fortsatt har tilgang.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="4e0cb-122">Hvis deaktivering er forsinket, følger du denne Fremgangs måten:</span><span class="sxs-lookup"><span data-stu-id="4e0cb-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="4e0cb-123">Hvis du deaktiverer Exchange Administrator-rollen eller aktiverings perioden for rolle utløper, og du legger merke til en betydelig forsinkelse før tillatelsene fjernes, kan du åpne en støtte forespørsel og be kunde støtte teknikeren om å hjelpe deg med å arkivere en billett med den privilegerte tilgangs behandlings gruppen (PAM) i Office om dette problemet.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="4e0cb-124">Hvis aktiverings perioden er utløpt, men du fremdeles har åpnet nett leser økten, lukker du nett leseren.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="4e0cb-125">Du kan fortsette å bruke rollen til du lukker den økten.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="4e0cb-126">Dette er et kjent problem, og vi ser på en mulig løsning for aktivt å oppheve hver økt når aktiveringen er utløpt.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="4e0cb-127">Hvis forsinkelsen er forskjellig fra disse to scenariene, kan du åpne en støtte forespørsel.</span><span class="sxs-lookup"><span data-stu-id="4e0cb-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
