---
title: Løs 0x8004de40-feil i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716037"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="ca4f1-102">Løs 0x8004de40-feil i OneDrive</span><span class="sxs-lookup"><span data-stu-id="ca4f1-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="ca4f1-103">Hvis du får en 0x8004de40-feil med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="ca4f1-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="ca4f1-104">Start den berørte datamaskinen på nytt mens den er koblet til Acitve Directory-domenet.</span><span class="sxs-lookup"><span data-stu-id="ca4f1-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="ca4f1-105">Hvis en omstart ikke løser problemet, kan du slutte å bli med på enheten og bli med på nytt fra Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ca4f1-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="ca4f1-106">**Merk:** Du bør være på bedriftsnettverket mens du utfører disse trinnene.</span><span class="sxs-lookup"><span data-stu-id="ca4f1-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="ca4f1-107">Ikke utfør disse trinnene når du ikke kan koble til bedriftens infrastruktur (for eksempel mens du reiser).</span><span class="sxs-lookup"><span data-stu-id="ca4f1-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="ca4f1-108">Åpne en hevet ledetekst.</span><span class="sxs-lookup"><span data-stu-id="ca4f1-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="ca4f1-109">Hvis du vil åpne en hevet ledetekst, klikker du - **Start**, høyreklikker **Ledetekst**, og deretter klikker du Kjør **som administrator**.</span><span class="sxs-lookup"><span data-stu-id="ca4f1-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="ca4f1-110">Skriv *inn dsregcmd /leave,* og trykk **Enter**.</span><span class="sxs-lookup"><span data-stu-id="ca4f1-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="ca4f1-111">Når du er ferdig, skriver du inn *dsregcmd /join* og trykker **Enter**.</span><span class="sxs-lookup"><span data-stu-id="ca4f1-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="ca4f1-112">Når du er ferdig, lukker du ledeteksten.</span><span class="sxs-lookup"><span data-stu-id="ca4f1-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="ca4f1-113">Start datamaskinen på nytt, og logg på OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ca4f1-113">Reboot the computer, and log into OneDrive.</span></span>