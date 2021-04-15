---
title: Teams 4c7-feil
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786678"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="bd047-102">4c7-feil i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="bd047-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="bd047-103">Denne feilen oppstår fordi Microsoft Teams krever skjemagodkjenning.</span><span class="sxs-lookup"><span data-stu-id="bd047-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="bd047-104">Når du distribuerer Active Directory Federation Services (AD FS), er skjemagodkjenning ikke aktivert for intranettet som standard.</span><span class="sxs-lookup"><span data-stu-id="bd047-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="bd047-105">Hvis Integrert windows-godkjenning mislykkes, blir du bedt om å logge på ved hjelp av Skjemagodkjenning.</span><span class="sxs-lookup"><span data-stu-id="bd047-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="bd047-106">Du kan løse dette problemet ved å aktivere Skjemagodkjenning ved hjelp av snapin-modulen AD FS Microsoft Management Console (MMC) på datamaskinen som har den lokale kopien av Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bd047-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="bd047-107">Dette gjør du slik:</span><span class="sxs-lookup"><span data-stu-id="bd047-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="bd047-108">Bla til Godkjenningspolicyer i **navigasjonsruten.**</span><span class="sxs-lookup"><span data-stu-id="bd047-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="bd047-109">Velg **Rediger** global primær godkjenning under Handlinger i **detaljruten.**</span><span class="sxs-lookup"><span data-stu-id="bd047-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="bd047-110">Velg Skjemagodkjenning på **Intranett-fanen.** </span><span class="sxs-lookup"><span data-stu-id="bd047-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="bd047-111">Velg **OK** (eller **Bruk**).</span><span class="sxs-lookup"><span data-stu-id="bd047-111">Select **OK** (or **Apply**).</span></span>