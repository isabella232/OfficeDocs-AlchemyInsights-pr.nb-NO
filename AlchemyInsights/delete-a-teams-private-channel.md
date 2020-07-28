---
title: Slette en privat kanal for Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439908"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="15d2a-102">Slette en privat kanal for Teams</span><span class="sxs-lookup"><span data-stu-id="15d2a-102">Delete a Teams private channel</span></span>

<span data-ttu-id="15d2a-103">Microsoft er klar over et problem med å slette en privat kanal for Teams hvis du har SharePoint-oppbevaringspolicyer aktivert for det underliggende SharePoint-området.</span><span class="sxs-lookup"><span data-stu-id="15d2a-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="15d2a-104">Microsoft jobber med en løsning.</span><span class="sxs-lookup"><span data-stu-id="15d2a-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="15d2a-105">I mellomtiden kan du bruke følgende løsninger til å slette den private kanalen.</span><span class="sxs-lookup"><span data-stu-id="15d2a-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="15d2a-106">**Utelate gruppe-/områdesamlingen fra sharepoint-oppbevaringspolicyen.**</span><span class="sxs-lookup"><span data-stu-id="15d2a-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="15d2a-107">Gå til administrasjonsportalen for Office 365, og velg **Vis alt** i navigasjonsruten til venstre.</span><span class="sxs-lookup"><span data-stu-id="15d2a-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="15d2a-108">Gå til **Sikkerhets- &** Policy for hindring av datatap for samsvar under **Administrasjonssentre**  >  **Data Loss Prevention**  >  **Policy**.</span><span class="sxs-lookup"><span data-stu-id="15d2a-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="15d2a-109">Identifiser eventuelle policyer som gjelder for Sharepoint-områder, og endre policyen slik at Sharepoint-området for teamet som inneholder den private kanalen, IKKE er inkludert i oppbevaringspolicyen.</span><span class="sxs-lookup"><span data-stu-id="15d2a-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="15d2a-110">Lagre retningslinjene.</span><span class="sxs-lookup"><span data-stu-id="15d2a-110">Save the policy.</span></span>
    <span data-ttu-id="15d2a-111">Det kan ta opptil 24 timer før policyinnstillingene trer i kraft.</span><span class="sxs-lookup"><span data-stu-id="15d2a-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="15d2a-112">Når nettstedet er utelukket, kan du slette den private kanalen.</span><span class="sxs-lookup"><span data-stu-id="15d2a-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="15d2a-113">Du ***kan kanskje*** slette den private kanalen ved hjelp av Microsoft Teams på Android-enheten din.</span><span class="sxs-lookup"><span data-stu-id="15d2a-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="15d2a-114">Hvis du vil ha relatert SharePoint-informasjon, kan du se [Kan ikke slette elementer i SharePoint Online eller OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="15d2a-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>