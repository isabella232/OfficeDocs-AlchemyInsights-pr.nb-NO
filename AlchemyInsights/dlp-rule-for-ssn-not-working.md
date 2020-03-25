---
title: DLP-regel for SSN fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932544"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="16cfc-102">DLP-problemer med personnummer</span><span class="sxs-lookup"><span data-stu-id="16cfc-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="16cfc-103">**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen.</span><span class="sxs-lookup"><span data-stu-id="16cfc-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="16cfc-104">Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="16cfc-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="16cfc-105">I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.</span><span class="sxs-lookup"><span data-stu-id="16cfc-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="16cfc-106">Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene.</span><span class="sxs-lookup"><span data-stu-id="16cfc-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="16cfc-107">Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider.</span><span class="sxs-lookup"><span data-stu-id="16cfc-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="16cfc-108">I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.</span><span class="sxs-lookup"><span data-stu-id="16cfc-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="16cfc-109">**DLP-problemer med SSN-er**</span><span class="sxs-lookup"><span data-stu-id="16cfc-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="16cfc-110">Har du problemer med at **dlp (Data Loss Prevention)** ikke fungerer for innhold som inneholder et **personnummer (SSN)** når du bruker en sensitiv informasjonstype i Office 365?</span><span class="sxs-lookup"><span data-stu-id="16cfc-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="16cfc-111">I så fall må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-retningslinjene ser ut.</span><span class="sxs-lookup"><span data-stu-id="16cfc-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="16cfc-112">For en SSN-policy som er konfigurert med et konfidensnivå på 85 %, evalueres følgende for eksempel for at regelen skal utløses:</span><span class="sxs-lookup"><span data-stu-id="16cfc-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="16cfc-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 sifre, som kan være i et formatert eller uformatert mønster</span><span class="sxs-lookup"><span data-stu-id="16cfc-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="16cfc-114">**[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funksjoner ser etter SSNer i fire forskjellige mønstre:</span><span class="sxs-lookup"><span data-stu-id="16cfc-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="16cfc-115">Func_ssn finner SSNer med sterk formatering før 2011 som er formatert med bindestreker eller mellomrom (dddd-dddd eller ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="16cfc-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="16cfc-116">Func_unformatted_ssn finner SSNer med sterk formatering før 2011 som ikke er formatert som ni påfølgende sifre (ddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="16cfc-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="16cfc-117">Func_randomized_formatted_ssn finner som-koder etter 2011 som er formatert med bindestreker eller mellomrom (dddd-dddd ddd dd dd ddd)</span><span class="sxs-lookup"><span data-stu-id="16cfc-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="16cfc-118">Func_randomized_unformatted_ssn finner som-koder etter 2011 som ikke er formatert som ni påfølgende sifre (dddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="16cfc-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="16cfc-119">**[Sjekksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nei, det er ingen Checksum</span><span class="sxs-lookup"><span data-stu-id="16cfc-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="16cfc-120">**[Definisjon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** En DLP-policy er 85% sikker på at den oppdages denne typen sensitiv informasjon hvis, i nærheten av 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="16cfc-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="16cfc-121">[Funksjonen Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finner innhold som samsvarer med mønsteret.</span><span class="sxs-lookup"><span data-stu-id="16cfc-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="16cfc-122">Finner et nøkkelord fra [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="16cfc-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="16cfc-123">Eksempler på søkeord inkluderer: *Trygd, Trygd#, Soc Sec , SSN* .</span><span class="sxs-lookup"><span data-stu-id="16cfc-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="16cfc-124">Følgende eksempel utløses for eksempel DLP SSN-policyen: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="16cfc-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="16cfc-125">Hvis du vil ha mer informasjon om hva som kreves for at SSN-er skal oppdages for innholdet ditt, kan du se følgende del i denne artikkelen: [Hvilke sensitive informasjonstyper ser etter SSN-er](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="16cfc-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="16cfc-126">Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: [Hva sensitive informasjonstyper ser etter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="16cfc-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  