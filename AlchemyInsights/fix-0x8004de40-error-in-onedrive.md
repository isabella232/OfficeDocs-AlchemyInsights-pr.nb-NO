---
title: Fix 0x8004de40 feil i OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755857"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="b87a3-102">Fix 0x8004de40 feil i OneDrive</span><span class="sxs-lookup"><span data-stu-id="b87a3-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="b87a3-103">Hvis du får en 0x8004de40-feil med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="b87a3-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="b87a3-104">Gjenstarte det berørt computer stund koplet å din aktvi adresseliste domenen.</span><span class="sxs-lookup"><span data-stu-id="b87a3-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="b87a3-105">Hvis en omstart ikke løser problemet, melde deg ut og bli med enheten fra Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b87a3-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="b87a3-106">**Merk**: du bør være på bedriftsnettverket mens du utfører disse trinnene.</span><span class="sxs-lookup"><span data-stu-id="b87a3-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="b87a3-107">Ikke Utfør disse trinnene når du ikke kan koble til bedriftsinfrastrukturen (for eksempel mens du er på reise).</span><span class="sxs-lookup"><span data-stu-id="b87a3-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="b87a3-108">Åpne en hevet ledetekst.</span><span class="sxs-lookup"><span data-stu-id="b87a3-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="b87a3-109">Å åpen en opphøyet kommandere spørsmål, falle i staver- **starte**, rett-falle i staver **kommandere spørsmål**, og så falle **i staver løpe idet administrator**.</span><span class="sxs-lookup"><span data-stu-id="b87a3-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="b87a3-110">Skriv inn *dsregcmd/Leave* og trykk **Enter**.</span><span class="sxs-lookup"><span data-stu-id="b87a3-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="b87a3-111">Når du er ferdig, skriver du inn *dsregcmd/JOIN* og trykker **Enter**.</span><span class="sxs-lookup"><span data-stu-id="b87a3-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="b87a3-112">Når du er ferdig, lukker du ledeteksten.</span><span class="sxs-lookup"><span data-stu-id="b87a3-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="b87a3-113">Start datamaskinen på nytt, og Logg på OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b87a3-113">Reboot the computer, and log into OneDrive.</span></span>