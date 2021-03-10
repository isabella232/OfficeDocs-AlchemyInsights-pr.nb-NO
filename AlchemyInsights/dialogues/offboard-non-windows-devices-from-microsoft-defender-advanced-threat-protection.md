---
title: Offboard ikke-Windows-enheter fra Microsoft Defender Advanced Threat Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695154"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="8905e-102">Offboard ikke-Windows-enheter fra Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="8905e-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="8905e-103">Slik gjør du det:</span><span class="sxs-lookup"><span data-stu-id="8905e-103">Here's how:</span></span>

1. <span data-ttu-id="8905e-104">Følg tredjepartsdokumentasjonen for å koble fra tredjepartsløsningen fra Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="8905e-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="8905e-105">Fjern tillatelser for tredjepartsløsningen fra Azure Active Directory-leieren:</span><span class="sxs-lookup"><span data-stu-id="8905e-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="8905e-106">Logg på [Azure Portal.](https://go.microsoft.com/fwlink/?linkid=2125612)</span><span class="sxs-lookup"><span data-stu-id="8905e-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="8905e-107">Velg **Alle tjenester** for Azure Active  >  **Directory**  >  **Enterprise-programmer.**</span><span class="sxs-lookup"><span data-stu-id="8905e-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="8905e-108">Velg programmet du vil sette av.</span><span class="sxs-lookup"><span data-stu-id="8905e-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="8905e-109">Velg **Slett.**</span><span class="sxs-lookup"><span data-stu-id="8905e-109">Select **Delete**.</span></span>

<span data-ttu-id="8905e-110">Hvis du vil ha mer informasjon, [kan du se Offboard-enheter som](https://go.microsoft.com/fwlink/?linkid=2143630)ikke bruker Windows.</span><span class="sxs-lookup"><span data-stu-id="8905e-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
