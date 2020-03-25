---
title: DLP fungerer ikke som forventet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932631"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="9ce7b-102">DLP fungerer ikke som forventet</span><span class="sxs-lookup"><span data-stu-id="9ce7b-102">DLP not working as expected</span></span>

<span data-ttu-id="9ce7b-103">**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen.</span><span class="sxs-lookup"><span data-stu-id="9ce7b-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="9ce7b-104">Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="9ce7b-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="9ce7b-105">I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.</span><span class="sxs-lookup"><span data-stu-id="9ce7b-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="9ce7b-106">Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene.</span><span class="sxs-lookup"><span data-stu-id="9ce7b-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="9ce7b-107">Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider.</span><span class="sxs-lookup"><span data-stu-id="9ce7b-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="9ce7b-108">I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.</span><span class="sxs-lookup"><span data-stu-id="9ce7b-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="9ce7b-109">**Sette opp DLP**</span><span class="sxs-lookup"><span data-stu-id="9ce7b-109">**Setting up DLP**</span></span>

<span data-ttu-id="9ce7b-110">Har du problemer med **at dlp (Data Loss Prevention)** i Office 365 ikke fungerer som forventet?</span><span class="sxs-lookup"><span data-stu-id="9ce7b-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="9ce7b-111">I så fall må du kontrollere at **DLP-policyen** er riktig konfigurert, og at dataene inneholder hva **DLP-policyen** leter etter når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="9ce7b-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="9ce7b-112">Med DLP-policyer kan du identifisere og beskytte sensitiv informasjon i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="9ce7b-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="9ce7b-113">Hvis du vil konfigurere DLP-policyer, bruker du informasjonen [her](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="9ce7b-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="9ce7b-114">**Hvilke DLP-retningslinjer ser etter**</span><span class="sxs-lookup"><span data-stu-id="9ce7b-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="9ce7b-115">Når du bruker de **innebygde sensitive informasjonstypene** i Office 365 sikkerhets- og samsvarssenter, ser DLP-policyer etter bestemte mønstre og elementer når du oppdager disse sensitive typene.</span><span class="sxs-lookup"><span data-stu-id="9ce7b-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="9ce7b-116">**Innebygde sensitive informasjonstyper**</span><span class="sxs-lookup"><span data-stu-id="9ce7b-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="9ce7b-117">Hvis du vil ha informasjon om de innebygde sensitive typene og hva en DLP-policy ser etter når du oppdager sensitivetypen, kan du se: [Hva de sensitive informasjonstypene ser etter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="9ce7b-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="9ce7b-118">**Egendefinerte sensitive informasjonstyper**</span><span class="sxs-lookup"><span data-stu-id="9ce7b-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="9ce7b-119">Hvis du prøver å opprette egendefinerte sensitive informasjonstyper, bruker du følgende artikkel for informasjon om hvordan du oppretter en egendefinert sensitiv type: [Opprette en egendefinert sensitiv informasjonstype](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="9ce7b-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="9ce7b-120">**Teste en DLP-policy**</span><span class="sxs-lookup"><span data-stu-id="9ce7b-120">**Test a DLP policy**</span></span>

<span data-ttu-id="9ce7b-121">Hvis du vil teste dataene med en innebygd eller egendefinert sensitiv informasjonstype, bruker du alternativet **Testtype** under **Klassifiseringer** > **Sensitive infotyper**.</span><span class="sxs-lookup"><span data-stu-id="9ce7b-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="9ce7b-122">Hvis du vil ha mer informasjon, kan du se [Teste egendefinerte sensitive informasjonstyper](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="9ce7b-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="9ce7b-123">**Rapporter**</span><span class="sxs-lookup"><span data-stu-id="9ce7b-123">**Reports**</span></span>
  
- <span data-ttu-id="9ce7b-124">Få sensitiv datainnsikt med [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="9ce7b-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="9ce7b-125">Se bestemte detaljer om hendelsen med en [hendelsesrapport](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="9ce7b-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
