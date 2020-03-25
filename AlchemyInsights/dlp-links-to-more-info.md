---
title: Mer informasjon om DLP-problemer
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932703"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="2e750-102">Informasjon om Problemer med DLP</span><span class="sxs-lookup"><span data-stu-id="2e750-102">Information about DLP issues</span></span>

<span data-ttu-id="2e750-103">**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen.</span><span class="sxs-lookup"><span data-stu-id="2e750-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="2e750-104">Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="2e750-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="2e750-105">I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.</span><span class="sxs-lookup"><span data-stu-id="2e750-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="2e750-106">Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene.</span><span class="sxs-lookup"><span data-stu-id="2e750-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="2e750-107">Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider.</span><span class="sxs-lookup"><span data-stu-id="2e750-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="2e750-108">I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.</span><span class="sxs-lookup"><span data-stu-id="2e750-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="2e750-109">**Informasjon om DLP-policy**</span><span class="sxs-lookup"><span data-stu-id="2e750-109">**Information on DLP policy**</span></span>

<span data-ttu-id="2e750-110">Med en DLP-policy kan du identifisere, overvåke og automatisk beskytte sensitiv informasjon på tvers av Office 365.</span><span class="sxs-lookup"><span data-stu-id="2e750-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="2e750-111">Vennligst besøk disse koblingene for mer informasjon:</span><span class="sxs-lookup"><span data-stu-id="2e750-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="2e750-112">Oversikt over forebygging av tap av data</span><span class="sxs-lookup"><span data-stu-id="2e750-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="2e750-113">Hva de sensitive informasjonstypene ser etter</span><span class="sxs-lookup"><span data-stu-id="2e750-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="2e750-114">Opprette en egendefinert sensitiv informasjonstype</span><span class="sxs-lookup"><span data-stu-id="2e750-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="2e750-115">Send e-postvarsler og vis tips om retningslinjene</span><span class="sxs-lookup"><span data-stu-id="2e750-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="2e750-116">Beskytte SharePoint Online-filer med oppbevaringsetiketter og DLP</span><span class="sxs-lookup"><span data-stu-id="2e750-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="2e750-117">DLP og Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2e750-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="2e750-118">Hvis du vil teste dataene med en innebygd eller egendefinert sensitiv informasjonstype, bruker du alternativet **Testtype** under **Klassifiseringer** > **Sensitive infotyper**.</span><span class="sxs-lookup"><span data-stu-id="2e750-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="2e750-119">Hvis du vil ha mer informasjon, kan du se [Teste egendefinerte sensitive informasjonstyper](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="2e750-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>