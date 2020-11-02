---
title: 0x8004de40-feil når du starter OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823112"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="cc787-102">0x8004de40-feil når du starter OneDrive</span><span class="sxs-lookup"><span data-stu-id="cc787-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="cc787-103">Hvis du får en feil melding **0x8004de40** når du logger deg på OneDrive, må du starte data maskinen på nytt mens du er koblet til jobb-eller skole domenet.</span><span class="sxs-lookup"><span data-stu-id="cc787-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="cc787-104">Hvis du får denne feil meldingen når du starter på nytt, kan du prøve dette mens du er koblet til jobb-eller skole domenet:</span><span class="sxs-lookup"><span data-stu-id="cc787-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="cc787-105">Klikk Start, **og skriv inn** kommando **linje**  eller lede tekst i søke boksen, høyre klikk på lede tekst appen, og velg  **Kjør som administrator** .</span><span class="sxs-lookup"><span data-stu-id="cc787-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="cc787-106">Hvis du blir bedt om å oppgi et administrator passord eller en bekreftelse, skriver du inn passordet eller klikker **Tillat** .</span><span class="sxs-lookup"><span data-stu-id="cc787-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="cc787-107">Skriv inn **dsregcmd/Leave**  i lede tekst vinduet, og vent til kommandoen er fullført.</span><span class="sxs-lookup"><span data-stu-id="cc787-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="cc787-108">Skriv deretter inn **dsregcmd/JOIN** , og vent til kommandoen er fullført.</span><span class="sxs-lookup"><span data-stu-id="cc787-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="cc787-109">Start data maskinen på nytt.</span><span class="sxs-lookup"><span data-stu-id="cc787-109">Reboot your computer.</span></span>
