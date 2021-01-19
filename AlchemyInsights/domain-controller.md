---
title: Domene kontroller
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901308"
---
# <a name="domain-controller"></a><span data-ttu-id="b3ea6-102">Domene kontroller</span><span class="sxs-lookup"><span data-stu-id="b3ea6-102">Domain controller</span></span>

<span data-ttu-id="b3ea6-103">**Kan ikke aktivere AAD-DS eller distribusjon mislykkes**</span><span class="sxs-lookup"><span data-stu-id="b3ea6-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="b3ea6-104">Hvis du vil løse problemet med at Azure AD Domain Service (AAD-DS) ikke aktiveres eller ikke kan distribueres, utfører du følgende trinn:</span><span class="sxs-lookup"><span data-stu-id="b3ea6-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="b3ea6-105">Hvis du bruker et virtuelt nettverk som allerede finnes, må du kontrollere NSG for regler som blokkerer porter som er nødvendige for å synkronisere i AAD-DS i portalen https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="b3ea6-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="b3ea6-106">Kontroller om feil meldingen er besvart i denne veiledningen for feil søking som er tilgjengelig i  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="b3ea6-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="b3ea6-107">Prøv å distribuere Azure AD Domain Services i et nytt virtuelt nettverk.</span><span class="sxs-lookup"><span data-stu-id="b3ea6-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="b3ea6-108">Følg instruksjonene i komme i gang med hvordan du distribuerer AAD-DS, som er tilgjengelig i [opplæring for å opprette Azure ad Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="b3ea6-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="b3ea6-109">Hvis du har problemer med å distribuere Azure AD Domain Services, kan du se [Feilsøke Azure ad Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) for å løse vanlige feil for å få ting til å fungere på nytt.</span><span class="sxs-lookup"><span data-stu-id="b3ea6-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="b3ea6-110">**Kan ikke deaktivere AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="b3ea6-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="b3ea6-111">AAD-DS kan ikke stanses midlertidig.</span><span class="sxs-lookup"><span data-stu-id="b3ea6-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="b3ea6-112">Hvis du vil slutte å bruke det forvaltede domenet, må det slettes.</span><span class="sxs-lookup"><span data-stu-id="b3ea6-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="b3ea6-113">Hvis det oppstår problemer, kan du løse vanlige feil meldinger og for å få de tilknyttede feil søkings trinnene for å hjelpe deg med å kjøre dem igjen, se [Feilsøke Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="b3ea6-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
