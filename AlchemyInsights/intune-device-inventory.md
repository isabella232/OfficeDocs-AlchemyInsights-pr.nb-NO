---
title: Intune-enhet inventar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440483"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="63575-102">Intune-enhet inventar</span><span class="sxs-lookup"><span data-stu-id="63575-102">Intune Device Inventory</span></span>

<span data-ttu-id="63575-103">Enheter-bladet gir administratorinnsikt i enheter under administrasjon i Intune per enhet.</span><span class="sxs-lookup"><span data-stu-id="63575-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="63575-104">Informasjonen som vises inkluderer: Maskinvare, Oppdagede programmer, Enhetssamsvar-tilstand og Enhetskonfigurasjon.The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span><span class="sxs-lookup"><span data-stu-id="63575-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="63575-105">Lagerdata for maskinvare og oppdagede programmer samles inn på en syv-dagers syklus.</span><span class="sxs-lookup"><span data-stu-id="63575-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="63575-106">Programmene og de spesifikke elementene i maskinvare som rapporteres varierer avhengig av enhetens operativsystem og om enheten er personlig eller bedriftseid.</span><span class="sxs-lookup"><span data-stu-id="63575-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="63575-107">Hvis du vil ha mer informasjon, kan du se [Se enhetsdetaljer i Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="63575-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="63575-108">**SPØRSMÅL OG SVAR**</span><span class="sxs-lookup"><span data-stu-id="63575-108">**FAQ**</span></span>

<span data-ttu-id="63575-109">Spørsmål: Jeg mottar ikke en fullstendig lagerliste over programmer som finnes på Intune-registrerte Windows-enheter.</span><span class="sxs-lookup"><span data-stu-id="63575-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="63575-110">hvorfor ikke?</span><span class="sxs-lookup"><span data-stu-id="63575-110">Why not?</span></span>

<span data-ttu-id="63575-111">Svar: For øyeblikket er bare moderne apper oppført for Windows 10-PCer som er identifisert som firmaenheter.</span><span class="sxs-lookup"><span data-stu-id="63575-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="63575-112">Intune samler ikke inn informasjon om Win32-apper som er installert på disse enhetene.</span><span class="sxs-lookup"><span data-stu-id="63575-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="63575-113">Spørsmål: Hvorfor samles ikke telefonnumre fra alle enheter?</span><span class="sxs-lookup"><span data-stu-id="63575-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="63575-114">Svar: Telefoner kategorisert som firmaenheter i Intune identifiseres ikke med hele telefonnummeret når du for eksempel kjører en lagerrapport for mobilenheter.</span><span class="sxs-lookup"><span data-stu-id="63575-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="63575-115">Bring-you-own-device telefonnumre er alltid delvis maskert med stjerner (\*\*\*\*), og viser bare de fire siste sifrene.</span><span class="sxs-lookup"><span data-stu-id="63575-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>