---
title: Eksterne ikke-Windows-enheter fra Microsoft Defender Advanced Threat Protection (ATP)
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748477"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="a9e44-102">Eksterne ikke-Windows-enheter fra Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="a9e44-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="a9e44-103">Slik gjør du det:</span><span class="sxs-lookup"><span data-stu-id="a9e44-103">Here's how:</span></span>

1. <span data-ttu-id="a9e44-104">Følg tredjepartsdokumentasjonen for å koble fra tredjepartsløsningen fra Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="a9e44-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="a9e44-105">Fjern tillatelser for tredjepartsløsningen fra Azure Active Directory-leieren:</span><span class="sxs-lookup"><span data-stu-id="a9e44-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="a9e44-106">Logg på [Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="a9e44-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="a9e44-107">Velg **Alle tjenester** Azure Active  >  **Directory** Enterprise  >  **Applications**.</span><span class="sxs-lookup"><span data-stu-id="a9e44-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="a9e44-108">Velg programmet du vil sette av.</span><span class="sxs-lookup"><span data-stu-id="a9e44-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="a9e44-109">Velg **Slett**.</span><span class="sxs-lookup"><span data-stu-id="a9e44-109">Select **Delete**.</span></span>

<span data-ttu-id="a9e44-110">Hvis du vil ha mer informasjon, [kan du se Eksterne enheter uten Windows](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="a9e44-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
