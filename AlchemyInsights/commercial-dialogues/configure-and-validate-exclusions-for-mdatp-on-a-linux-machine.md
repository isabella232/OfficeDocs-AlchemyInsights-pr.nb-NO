---
title: Konfigurere og validere utelatelser for MDATP på en Linux-maskin
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749254"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="0a76b-102">Konfigurere og validere utelatelser for MDATP på en Linux-maskin</span><span class="sxs-lookup"><span data-stu-id="0a76b-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="0a76b-103">Du kan utelate bestemte filer, mapper, prosesser og prosessåpnede filer fra MDATP-skanninger.</span><span class="sxs-lookup"><span data-stu-id="0a76b-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="0a76b-104">Utelatelser bidrar til å forhindre feil gjenkjenning av programvare og filer som er unike eller tilpasset organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="0a76b-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="0a76b-105">Utelatelser bidrar også til å redusere ytelsesproblemer forårsaket av MDATP.</span><span class="sxs-lookup"><span data-stu-id="0a76b-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="0a76b-106">Hvis du vil ha mer informasjon, kan du se Konfigurere [og validere utelatelser for MDATP for Linux.](https://go.microsoft.com/fwlink/?linkid=2144517)</span><span class="sxs-lookup"><span data-stu-id="0a76b-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0a76b-107">Unntakene som er beskrevet i denne artikkelen, gjelder ikke for andre funksjoner i MDATP for Linux, inkludert gjenkjenning av endepunkter og svar (EDR).</span><span class="sxs-lookup"><span data-stu-id="0a76b-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="0a76b-108">Filer som du utelater ved hjelp av metodene som er beskrevet i denne artikkelen, kan fortsatt utløse EDR-varsler og andre gjenkjenningsfunksjoner.</span><span class="sxs-lookup"><span data-stu-id="0a76b-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
