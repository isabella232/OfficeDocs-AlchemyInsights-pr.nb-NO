---
title: Løse 0x8004de40-feil i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745139"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="b8ae6-102">Løse 0x8004de40-feil i OneDrive</span><span class="sxs-lookup"><span data-stu-id="b8ae6-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="b8ae6-103">Hvis du får en 0x8004de40-feil med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="b8ae6-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="b8ae6-104">Start den berørte data maskinen på nytt mens du er koblet til Acitve Directory-domenet.</span><span class="sxs-lookup"><span data-stu-id="b8ae6-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="b8ae6-105">Hvis en omstart ikke løser problemet, kan du koble fra enheten og koble den til på nytt fra Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b8ae6-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="b8ae6-106">**Merk**: du bør være på bedrifts nettverket mens du utfører disse trinnene.</span><span class="sxs-lookup"><span data-stu-id="b8ae6-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="b8ae6-107">Ikke Utfør denne Fremgangs måten når du ikke kan koble til infrastrukturen for bedriften (for eksempel mens du er på reise).</span><span class="sxs-lookup"><span data-stu-id="b8ae6-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="b8ae6-108">Åpne en hevet lede tekst.</span><span class="sxs-lookup"><span data-stu-id="b8ae6-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="b8ae6-109">Hvis du vil åpne en hevet lede tekst, klikker du- **Start**, høyre klikker lede **tekst**, og klikker deretter **Kjør som administrator**.</span><span class="sxs-lookup"><span data-stu-id="b8ae6-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="b8ae6-110">Skriv inn *dsregcmd/Leave* , og trykk **Enter**.</span><span class="sxs-lookup"><span data-stu-id="b8ae6-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="b8ae6-111">Når du er ferdig, skriver du inn *dsregcmd/JOIN* og trykker **Enter**.</span><span class="sxs-lookup"><span data-stu-id="b8ae6-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="b8ae6-112">Når du er ferdig, lukker du lede teksten.</span><span class="sxs-lookup"><span data-stu-id="b8ae6-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="b8ae6-113">Start data maskinen på nytt, og Logg på OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b8ae6-113">Reboot the computer, and log into OneDrive.</span></span>