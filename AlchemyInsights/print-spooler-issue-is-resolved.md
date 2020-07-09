---
title: Problemet med utskriftskøen er løst
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088402"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="b3901-102">Problemet med utskriftskøen er løst</span><span class="sxs-lookup"><span data-stu-id="b3901-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="b3901-103">Hvis enheten ble oppdatert med Windows 10 **OS Build 19041.329**, kan det hende du har observert et problem der enkelte skrivere ikke kan skrive ut.</span><span class="sxs-lookup"><span data-stu-id="b3901-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="b3901-104">Utskriftskøen kan kaste en feil eller lukke uventet når du prøver å skrive ut, og ingen utskrift kommer fra den berørte skriveren.</span><span class="sxs-lookup"><span data-stu-id="b3901-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="b3901-105">Dette problemet er løst i OS Build **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="b3901-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="b3901-106">**Pågående etterforskning**</span><span class="sxs-lookup"><span data-stu-id="b3901-106">**Ongoing investigation**</span></span>

<span data-ttu-id="b3901-107">Den lokale security authority delsystem service (LSASS) filen\*\* (Isass.exe\*\*) kan mislykkes på enkelte enheter med feilmeldingen "En kritisk systemprosess, C:\WINDOWS\system32\Isass.exe, mislyktes med statuskode c0000008.</span><span class="sxs-lookup"><span data-stu-id="b3901-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="b3901-108">Maskinen må nå startes på nytt".</span><span class="sxs-lookup"><span data-stu-id="b3901-108">The machine must now be restarted".</span></span>  <span data-ttu-id="b3901-109">**Microsoft arbeider med en løsning og vil gi en oppdatering i en kommende utgivelse.**</span><span class="sxs-lookup"><span data-stu-id="b3901-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="b3901-110">Hvis du vil ha mer informasjon, kan du sjekke ut [kjente problemer med Windows 10 versjon 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="b3901-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>