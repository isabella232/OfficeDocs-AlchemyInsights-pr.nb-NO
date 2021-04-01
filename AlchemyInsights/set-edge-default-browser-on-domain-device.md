---
title: Angi Microsoft Edge som standardleser på en domenekretsenhet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491884"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="82638-102">Angi Microsoft Edge som standardleser på en domenekretsenhet</span><span class="sxs-lookup"><span data-stu-id="82638-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="82638-103">Angi Microsoft Edge som standard nettleser:</span><span class="sxs-lookup"><span data-stu-id="82638-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="82638-104">[Opprett en standard konfigurasjonsfil for tilknytninger,](https://go.microsoft.com/fwlink/?linkid=2132437) og lagre den lokalt eller på en delt nettverksressurs.</span><span class="sxs-lookup"><span data-stu-id="82638-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="82638-105">Åpne redigeringsprogrammet for gruppepolicy, og gå deretter til Administrative maler **for datamaskinkonfigurasjon**  >    >  **Windows Components**  >  **File Explorer**.</span><span class="sxs-lookup"><span data-stu-id="82638-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="82638-106">Velg **Angi en standard konfigurasjonsfil for tilknytninger**.</span><span class="sxs-lookup"><span data-stu-id="82638-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="82638-107">Velg **Policyinnstilling**, og velg deretter **Aktivert**.</span><span class="sxs-lookup"><span data-stu-id="82638-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="82638-108">Angi **plasseringen** til konfigurasjonsfilen for standardtilknytninger under Alternativer, og velg deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="82638-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
