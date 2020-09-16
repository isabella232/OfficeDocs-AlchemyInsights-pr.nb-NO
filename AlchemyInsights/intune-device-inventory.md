---
title: Enhets beholdning for Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667887"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="c6246-102">Enhets beholdning for Intune</span><span class="sxs-lookup"><span data-stu-id="c6246-102">Intune Device Inventory</span></span>

<span data-ttu-id="c6246-103">Enheter-bladserveren gir administrator innsikt i enheter under administrasjon i Intune på per enhets basis.</span><span class="sxs-lookup"><span data-stu-id="c6246-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="c6246-104">Informasjonen som vises, omfatter: maskin vare, oppdagede programmer, enhets Samsvars tilstand og enhets konfigurasjons tilstand.</span><span class="sxs-lookup"><span data-stu-id="c6246-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="c6246-105">Lager data for maskin vare og oppdagede programmer samles inn på en sju dagers syklus.</span><span class="sxs-lookup"><span data-stu-id="c6246-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="c6246-106">Programmer og bestemte elementer med maskin vare som er rapportert, varierer avhengig av enhetens operativ system og om enheten er personlig eller bedrifts eid.</span><span class="sxs-lookup"><span data-stu-id="c6246-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="c6246-107">Hvis du vil ha mer informasjon, kan du se [se enhets detaljer i Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="c6246-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="c6246-108">**SPØRSMÅL OG SVAR**</span><span class="sxs-lookup"><span data-stu-id="c6246-108">**FAQ**</span></span>

<span data-ttu-id="c6246-109">Spørsmål: jeg mottar ikke en fullstendig innholds liste over programmer som finnes på Intune-registrerte Windows-enheter.</span><span class="sxs-lookup"><span data-stu-id="c6246-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="c6246-110">hvorfor ikke?</span><span class="sxs-lookup"><span data-stu-id="c6246-110">Why not?</span></span>

<span data-ttu-id="c6246-111">A: for øyeblikket er det bare moderne apper som er oppført for Windows 10-PC-er som er identifisert som firma enheter.</span><span class="sxs-lookup"><span data-stu-id="c6246-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="c6246-112">Intune samler ikke inn informasjon om Win32-apper som er installert på disse enhetene.</span><span class="sxs-lookup"><span data-stu-id="c6246-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="c6246-113">Spørsmål: Hvorfor blir ikke telefon numre samlet inn fra alle enheter?</span><span class="sxs-lookup"><span data-stu-id="c6246-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="c6246-114">A: telefoner som er kategorisert som firma enheter i Intune, er ikke identifisert med sitt fulle telefon nummer når du for eksempel kjører en rapport om en mobil enhets beholdning.</span><span class="sxs-lookup"><span data-stu-id="c6246-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="c6246-115">Mobil telefon numre for enheter er alltid delvis maskert med stjerner (\* \* \* \*), og viser bare de fire siste sifrene.</span><span class="sxs-lookup"><span data-stu-id="c6246-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>