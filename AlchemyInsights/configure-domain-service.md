---
title: Konfigurere Domain service
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885693"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="0dfae-102">Kan ikke aktivere AAD-DS eller distribusjon mislykkes</span><span class="sxs-lookup"><span data-stu-id="0dfae-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="0dfae-103">Hvis du vil løse problemet med at Azure AD Domain Service (AAD-DS) ikke aktiveres eller ikke kan distribueres, utfører du følgende trinn:</span><span class="sxs-lookup"><span data-stu-id="0dfae-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="0dfae-104">Hvis du bruker et virtuelt nettverk som allerede finnes, må du kontrollere NSG for regler som blokkerer porter som er nødvendige for å synkronisere i AAD-DS i portalen https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="0dfae-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="0dfae-105">Kontroller om feil meldingen er besvart i denne veiledningen for feil søking som er tilgjengelig i  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="0dfae-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="0dfae-106">Prøv å distribuere Azure AD Domain Services i et nytt virtuelt nettverk.</span><span class="sxs-lookup"><span data-stu-id="0dfae-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="0dfae-107">Følg instruksjonene i komme i gang med hvordan du distribuerer AAD-DS: [opprette og konfigurere AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="0dfae-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="0dfae-108">Hvis du har problemer med å distribuere Azure AD Domain Services, kan du se [Feilsøke Azure ad Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) for å løse vanlige feil for å få ting til å fungere på nytt.</span><span class="sxs-lookup"><span data-stu-id="0dfae-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="0dfae-109">**Kan ikke deaktivere AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="0dfae-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="0dfae-110">AAD-DS kan ikke stanses midlertidig.</span><span class="sxs-lookup"><span data-stu-id="0dfae-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="0dfae-111">Hvis du vil slutte å bruke det forvaltede domenet, må det slettes.</span><span class="sxs-lookup"><span data-stu-id="0dfae-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="0dfae-112">Hvis du vil slette det administrerte domenet, kan du se [slette AAD Domain service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="0dfae-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



