---
title: DLP trenger kanskje en egendefinert type
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932667"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="724bd-102">DLP trenger kanskje en egendefinert type</span><span class="sxs-lookup"><span data-stu-id="724bd-102">DLP might need a custom type</span></span>

<span data-ttu-id="724bd-103">**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen.</span><span class="sxs-lookup"><span data-stu-id="724bd-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="724bd-104">Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="724bd-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="724bd-105">I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.</span><span class="sxs-lookup"><span data-stu-id="724bd-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="724bd-106">Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene.</span><span class="sxs-lookup"><span data-stu-id="724bd-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="724bd-107">Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider.</span><span class="sxs-lookup"><span data-stu-id="724bd-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="724bd-108">I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.</span><span class="sxs-lookup"><span data-stu-id="724bd-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="724bd-109">**DLP kan kreve en egendefinert informasjonstype**</span><span class="sxs-lookup"><span data-stu-id="724bd-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="724bd-110">Med en policy for hindring av tap av data (DLP) kan du identifisere og beskytte sensitive data i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="724bd-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="724bd-111">I noen scenarier må du kanskje opprette din egen **egendefinerte** sensitive informasjonstype for å beskytte organisasjonens data.</span><span class="sxs-lookup"><span data-stu-id="724bd-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="724bd-112">Organisasjonen må for eksempel kanskje identifisere og beskytte ansatt-IDer eller andre data i et format som er spesifikt for organisasjonen. I så fall kan du se følgende artikler for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="724bd-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="724bd-113">**Tilpasse en innebygd sensitiv informasjonstype**</span><span class="sxs-lookup"><span data-stu-id="724bd-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="724bd-114">Hvis en innebygd sensitiv informasjonstype vil møte dine behov med bare noen få tweaks, kan du [tilpasse en innebygd sensitiv informasjonstype](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="724bd-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="724bd-115">Du kan for eksempel legge til eller fjerne søkeord, eller legge til eller fjerne støttebevis, for eksempel en dato eller adresse.</span><span class="sxs-lookup"><span data-stu-id="724bd-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="724bd-116">**Opprette en egendefinert sensitiv informasjonstype**</span><span class="sxs-lookup"><span data-stu-id="724bd-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="724bd-117">Men hvis du trenger å identifisere og beskytte en annen type sensitiv informasjon helt, kan du [opprette en egendefinert sensitiv informasjonstype](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) i brukergrensesnittet i Security & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="724bd-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="724bd-118">**Opprette en egendefinert sensitiv informasjonstype i Security & Compliance Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="724bd-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="724bd-119">Til slutt, hvis brukergrensesnittet ikke inneholder alle alternativene du trenger, kan du [opprette en egendefinert sensitiv informasjonstype i Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="724bd-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="724bd-120">Ved å starte med en XML-fil kan du bruke alle tilgjengelige alternativer.</span><span class="sxs-lookup"><span data-stu-id="724bd-120">By starting with an XML file, you can use every option available.</span></span>
