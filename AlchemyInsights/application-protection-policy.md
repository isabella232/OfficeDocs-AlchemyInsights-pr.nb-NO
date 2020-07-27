---
title: Retningslinjer for programbeskyttelse
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423966"
---
# <a name="application-protection-policy"></a><span data-ttu-id="14c58-102">Retningslinjer for programbeskyttelse</span><span class="sxs-lookup"><span data-stu-id="14c58-102">Application protection policy</span></span>

<span data-ttu-id="14c58-103">Hvis du ikke har vært i bruksområdepolicy (APP) før), kan du se [oversikten over retningslinjene for appbeskyttelse](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="14c58-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="14c58-104">Hvis du vil begynne å bruke APP, kan du se [Opprette og tilordne retningslinjer for appbeskyttelse](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="14c58-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="14c58-105">Krav til retningslinjer for brukspolicy:</span><span class="sxs-lookup"><span data-stu-id="14c58-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="14c58-106">Brukeren har en Intune- eller EMS-lisens.</span><span class="sxs-lookup"><span data-stu-id="14c58-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="14c58-107">Brukeren tilhører en gruppe som er målrettet av policyer for programbeskyttelse.</span><span class="sxs-lookup"><span data-stu-id="14c58-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="14c58-108">Bare én bedriftsbruker er logget på beskyttede apper på en enhet.</span><span class="sxs-lookup"><span data-stu-id="14c58-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="14c58-109">Programmet har implementert [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="14c58-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="14c58-110">Hvis du vil ha en liste over apper som støtter SDK, kan du se [Microsoft Intune-beskyttede apper](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="14c58-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="14c58-111">Policyer gjelder etter at en bruker som oppfyller kravene ovenfor, logger inn i en Intune SDK-aktivert app.</span><span class="sxs-lookup"><span data-stu-id="14c58-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="14c58-112">Den enkleste måten å finne ut om en policy brukes, er ved å kreve at brukeren angir en pin i policyen.</span><span class="sxs-lookup"><span data-stu-id="14c58-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="14c58-113">Hvis du vil ha mer informasjon, kan du ta en titt på:</span><span class="sxs-lookup"><span data-stu-id="14c58-113">For more information, see:</span></span>

[<span data-ttu-id="14c58-114">Vanlige spørsmål om feilsøking av APP/MAM</span><span class="sxs-lookup"><span data-stu-id="14c58-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="14c58-115">Slik validerer du oppsettet for appbeskyttelsespolicyen</span><span class="sxs-lookup"><span data-stu-id="14c58-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="14c58-116">Forstå leveringstidstidspunktet for appbeskyttelsespolicy</span><span class="sxs-lookup"><span data-stu-id="14c58-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="14c58-117">Slik overvåker du retningslinjer for appbeskyttelse</span><span class="sxs-lookup"><span data-stu-id="14c58-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)