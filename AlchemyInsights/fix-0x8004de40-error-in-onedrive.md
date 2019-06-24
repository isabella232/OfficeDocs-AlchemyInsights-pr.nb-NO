---
title: Rette opp feil i 0x8004de40 i OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133985"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="9c860-102">Rette opp feil i 0x8004de40 i OneDrive</span><span class="sxs-lookup"><span data-stu-id="9c860-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="9c860-103">Hvis du får en 0x8004de40-feil i OneDrive:</span><span class="sxs-lookup"><span data-stu-id="9c860-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="9c860-104">Start på nytt den berørte datamaskinen mens du er koblet til aktvi Directory-domene.</span><span class="sxs-lookup"><span data-stu-id="9c860-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="9c860-105">Hvis en omstart ikke løser problemet, melde deg ut og bli med enheten fra Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9c860-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="9c860-106">**Merk**: du bør være på firmanettverket mens du utfører disse trinnene.</span><span class="sxs-lookup"><span data-stu-id="9c860-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="9c860-107">Ikke Utfør denne fremgangsmåten når du ikke kan koble til din bedriftens infrastruktur (for eksempel mens du reiser).</span><span class="sxs-lookup"><span data-stu-id="9c860-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="9c860-108">Åpne en ledetekst.</span><span class="sxs-lookup"><span data-stu-id="9c860-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="9c860-109">For å åpne en ledetekst, klikk - **Start**, høyreklikk **ledetekst**, og deretter klikker du **Kjør som administrator**.</span><span class="sxs-lookup"><span data-stu-id="9c860-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="9c860-110">Skriv *dsregcmd /leave* , og trykk **Enter**.</span><span class="sxs-lookup"><span data-stu-id="9c860-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="9c860-111">Når operasjonen er fullført, skriver du inn *dsregcmd-/join* , og trykk **Enter**.</span><span class="sxs-lookup"><span data-stu-id="9c860-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="9c860-112">Når det er fullført, lukker du ledeteksten.</span><span class="sxs-lookup"><span data-stu-id="9c860-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="9c860-113">Start datamaskinen på nytt og logge på OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9c860-113">Reboot the computer, and log into OneDrive.</span></span>