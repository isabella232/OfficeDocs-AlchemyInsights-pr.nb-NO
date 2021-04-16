---
title: 0x8004de40 feilmelding når du starter OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813661"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="3b486-102">0x8004de40 feilmelding når du starter OneDrive</span><span class="sxs-lookup"><span data-stu-id="3b486-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="3b486-103">Hvis du får en feilmelding **0x8004de40** logge på OneDrive, starter du datamaskinen på nytt mens du er koblet til jobb- eller skoledomenet.</span><span class="sxs-lookup"><span data-stu-id="3b486-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="3b486-104">Hvis du får denne feilen etter omstart, kan du prøve dette mens du er koblet til jobb- eller skoledomenet:</span><span class="sxs-lookup"><span data-stu-id="3b486-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="3b486-105">Klikk Start, og skriv **inn cmd** eller **ledetekst**  i søkeboksen, høyreklikk på ledetekstappen, og velg  **Kjør som administrator**.</span><span class="sxs-lookup"><span data-stu-id="3b486-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="3b486-106">Hvis du blir bedt om et administratorpassord eller en bekreftelse, skriver du inn passordet eller klikker **Tillat**.</span><span class="sxs-lookup"><span data-stu-id="3b486-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="3b486-107">Skriv inn **dsregcmd /leave**  i ledetekstvinduet, og vent til kommandoen er fullført.</span><span class="sxs-lookup"><span data-stu-id="3b486-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="3b486-108">Skriv deretter **inn dsregcmd /join,** og vent til kommandoen er fullført.</span><span class="sxs-lookup"><span data-stu-id="3b486-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="3b486-109">Start datamaskinen på nytt.</span><span class="sxs-lookup"><span data-stu-id="3b486-109">Reboot your computer.</span></span>
