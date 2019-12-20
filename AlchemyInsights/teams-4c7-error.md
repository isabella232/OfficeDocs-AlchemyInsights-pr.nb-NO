---
title: Teams 4c 7-feil
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796264"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="5e2ae-102">4c 7 feil i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="5e2ae-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="5e2ae-103">Denne feilen oppstår fordi Microsoft Teams krever skjemagodkjenning.</span><span class="sxs-lookup"><span data-stu-id="5e2ae-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="5e2ae-104">Når du distribuerer Active Directory Federation Services (AD FS), aktiveres ikke skjemagodkjenning for intranettet som standard.</span><span class="sxs-lookup"><span data-stu-id="5e2ae-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="5e2ae-105">Hvis Windows-integrert godkjenning mislykkes, blir du bedt om å logge på ved hjelp av skjemagodkjenning.</span><span class="sxs-lookup"><span data-stu-id="5e2ae-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="5e2ae-106">Hvis du vil løse dette problemet, kan du aktivere skjemagodkjenning ved hjelp av snapin-modul for AD FS Microsoft Management Console (MMC) på datamaskinen som har den lokale kopien av Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5e2ae-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="5e2ae-107">Hvis du vil gjøre dette, følger du denne fremgangsmåten:</span><span class="sxs-lookup"><span data-stu-id="5e2ae-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="5e2ae-108">I navigasjonsruten blar du til **godkjennings policyer**.</span><span class="sxs-lookup"><span data-stu-id="5e2ae-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="5e2ae-109">Velg **Rediger global primær godkjenning**under **handlinger** i detaljruten.</span><span class="sxs-lookup"><span data-stu-id="5e2ae-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="5e2ae-110">Velg **skjemagodkjenning**i kategorien **intranett** .</span><span class="sxs-lookup"><span data-stu-id="5e2ae-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="5e2ae-111">Velg **OK** (eller **Bruk**).</span><span class="sxs-lookup"><span data-stu-id="5e2ae-111">Select **OK** (or **Apply**).</span></span>