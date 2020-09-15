---
title: Teams 4c7-feil
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700212"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="49c28-102">4c7-feil i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="49c28-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="49c28-103">Denne feilen oppstår fordi Microsoft Teams krever skjema godkjenning.</span><span class="sxs-lookup"><span data-stu-id="49c28-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="49c28-104">Når du distribuerer Active Directory Federation Services (AD FS), aktiveres ikke skjema godkjenning for intranett som standard.</span><span class="sxs-lookup"><span data-stu-id="49c28-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="49c28-105">Hvis det oppstår feil i Windows-integrert godkjenning, blir du bedt om å logge på ved hjelp av skjema godkjenning.</span><span class="sxs-lookup"><span data-stu-id="49c28-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="49c28-106">Hvis du vil løse dette problemet, kan du aktivere skjema godkjenning ved hjelp av AD FS-snapin-modulen for Microsoft Management Console (MMC) på data maskinen som har den lokale kopien av Active Directory.</span><span class="sxs-lookup"><span data-stu-id="49c28-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="49c28-107">Dette gjør du slik:</span><span class="sxs-lookup"><span data-stu-id="49c28-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="49c28-108">Gå til **godkjennings policyer**i navigasjons ruten.</span><span class="sxs-lookup"><span data-stu-id="49c28-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="49c28-109">Velg **Rediger global primær godkjenning**under **handlinger** i Detaljer-ruten.</span><span class="sxs-lookup"><span data-stu-id="49c28-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="49c28-110">Velg **skjema godkjenning**på fanen **intranett** .</span><span class="sxs-lookup"><span data-stu-id="49c28-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="49c28-111">Velg **OK** (eller **Bruk**).</span><span class="sxs-lookup"><span data-stu-id="49c28-111">Select **OK** (or **Apply**).</span></span>