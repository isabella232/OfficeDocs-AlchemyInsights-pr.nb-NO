---
title: Gjør dette hvis Azure-funksjonene ikke fungerer som de skal i Microsoft Edge
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583788"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="b49e7-102">Gjør dette hvis Azure-funksjonene ikke fungerer som de skal i Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b49e7-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="b49e7-103">Microsoft Edge har [kjente problemer](https://go.microsoft.com/fwlink/?linkid=2140608) som er relatert til sikkerhets soner, og kan påvirke hvordan Azure-brukere logger seg på administrasjons senteret for Windows.</span><span class="sxs-lookup"><span data-stu-id="b49e7-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="b49e7-104">Hvis du har problemer med å bruke Azure-funksjoner med Microsoft Edge, kan du prøve følgende trinn:</span><span class="sxs-lookup"><span data-stu-id="b49e7-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="b49e7-105">Søk etter **Alternativer for Internet t** på **Start** -menyen, og velg den.</span><span class="sxs-lookup"><span data-stu-id="b49e7-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="b49e7-106">Gå til fanen **sikkerhet** i dialog boksen **Egenskaper for Internet t** .</span><span class="sxs-lookup"><span data-stu-id="b49e7-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="b49e7-107">Velg sonen **Klarerte områder** , og velg deretter **områder** -knappen.</span><span class="sxs-lookup"><span data-stu-id="b49e7-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="b49e7-108">Legg til Netta DRESSen for gateway i tillegg til og i dialog boksen **Klarerte områder** , [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) og velg deretter **Lukk**.</span><span class="sxs-lookup"><span data-stu-id="b49e7-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="b49e7-109">Gå til **personvern** -fanen i dialog boksen **Egenskaper for Internet t** .</span><span class="sxs-lookup"><span data-stu-id="b49e7-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="b49e7-110">Velg **Innstillinger** i delen **popup-blokkering** .</span><span class="sxs-lookup"><span data-stu-id="b49e7-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="b49e7-111">Legg til Netta DRESSen for gateway i tillegg til og i dialog boksen som åpnes, [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) og velg deretter **Lukk**.</span><span class="sxs-lookup"><span data-stu-id="b49e7-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
