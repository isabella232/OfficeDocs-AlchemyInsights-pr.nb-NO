---
title: Programvarelager mangler eller er unøyaktig
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676509"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="20fa1-102">Programvarelager mangler eller er unøyaktig</span><span class="sxs-lookup"><span data-stu-id="20fa1-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="20fa1-103">Programvarebeholdningen i Håndtering av trusler og sikkerhetsproblemer (TVM) er en liste over kjent programvare i organisasjonen med offisielle Common Platform Enumerations (CPE).</span><span class="sxs-lookup"><span data-stu-id="20fa1-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="20fa1-104">Programvareprodukter uten en offisiell CPE har ikke publisert sikkerhetsproblemer.</span><span class="sxs-lookup"><span data-stu-id="20fa1-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="20fa1-105">Beholdningen inneholder også detaljer som navnet på leverandøren, antall svakheter, trusler og antall eksponerte enheter.</span><span class="sxs-lookup"><span data-stu-id="20fa1-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="20fa1-106">Programvareendringer på enheter gjenspeiles vanligvis i sikkerhetsportaler innen to timer.</span><span class="sxs-lookup"><span data-stu-id="20fa1-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="20fa1-107">Det kan imidlertid noen ganger ta lengre tid.</span><span class="sxs-lookup"><span data-stu-id="20fa1-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="20fa1-108">Det er for øyeblikket ikke mulig å fremtvinge en synkronisering. dette er en kontinuerlig vurdering.</span><span class="sxs-lookup"><span data-stu-id="20fa1-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="20fa1-109">Hvis du har gjort en programvareendring og endringen ikke gjenspeiles nøyaktig i TVM etter fem timer, følger du disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="20fa1-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="20fa1-110">Se delen om programvarebevis for å forstå hvordan programvaren ble oppdaget.</span><span class="sxs-lookup"><span data-stu-id="20fa1-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="20fa1-111">Kontroller at programvaren støttes.</span><span class="sxs-lookup"><span data-stu-id="20fa1-111">Make sure that the software is supported.</span></span> <span data-ttu-id="20fa1-112">Programvaren kan bare være synlig på enhetsnivå selv om den for øyeblikket ikke støttes av Håndtering av trusler og sikkerhetsproblemer.</span><span class="sxs-lookup"><span data-stu-id="20fa1-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="20fa1-113">Men bare begrensede data er tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="20fa1-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="20fa1-114">Hvis du vil se fremgangsmåten for å rapportere unøyaktighet fra portalen, kan du se [Rapportere unøyaktighet](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span><span class="sxs-lookup"><span data-stu-id="20fa1-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="20fa1-115">**Obs!** Rapportering av unøyaktighet fra MDE-portalen er en enveis kanal til ingeniørarbeid.</span><span class="sxs-lookup"><span data-stu-id="20fa1-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="20fa1-116">Hvis problemet haster, åpner du en støtteforespørsel.</span><span class="sxs-lookup"><span data-stu-id="20fa1-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="20fa1-117">Hvis du vil ha mer informasjon, kan [du se Programvarebeholdning – Håndtering av trusler og sikkerhetsproblemer](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="20fa1-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>