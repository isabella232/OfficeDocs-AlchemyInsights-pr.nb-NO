---
title: Problem med utskrifts køen er løst
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801850"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="25b86-102">Problem med utskrifts køen er løst</span><span class="sxs-lookup"><span data-stu-id="25b86-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="25b86-103">Hvis enheten ble oppdatert med Windows 10  **OS bygg 19041,329**, kan du ha observert et problem der visse skrivere ikke kunne skrives ut.</span><span class="sxs-lookup"><span data-stu-id="25b86-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="25b86-104">Utskrifts køen kan kanskje iverksette en feil eller lukkes uventet når du prøver å skrive ut, og ingen utdata kommer fra den berørte skrive ren.</span><span class="sxs-lookup"><span data-stu-id="25b86-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="25b86-105">Dette problemet er løst i OS Build  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="25b86-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="25b86-106">**Pågående undersøkelse**</span><span class="sxs-lookup"><span data-stu-id="25b86-106">**Ongoing investigation**</span></span>

<span data-ttu-id="25b86-107">LSASS-filen (Local Security Authority Subsystem Service) (**Isass.exe**) kan mislykkes på enkelte enheter med feil meldingen «en kritisk system prosess, C:\WINDOWS\system32\Isass.exe, mislyktes med status kode c0000008.</span><span class="sxs-lookup"><span data-stu-id="25b86-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="25b86-108">Maskinen må nå startes på nytt.</span><span class="sxs-lookup"><span data-stu-id="25b86-108">The machine must now be restarted".</span></span>  <span data-ttu-id="25b86-109">**Microsoft arbeider med en løsning og vil gi en oppdatering i en kommende utgivelse.**</span><span class="sxs-lookup"><span data-stu-id="25b86-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="25b86-110">Hvis du vil ha mer informasjon, kan du se  [kjente problemer med Windows 10 versjon 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="25b86-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>