---
title: DLP-regel for SSN fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: cfe884a207490a19325ce059652de158c16dc801
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704094"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="b08c9-102">DLP-problemer med personnummer</span><span class="sxs-lookup"><span data-stu-id="b08c9-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="b08c9-103">**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="b08c9-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="b08c9-104">**DLP-problemer med SSN-er**</span><span class="sxs-lookup"><span data-stu-id="b08c9-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="b08c9-105">Har du problemer med at **dlp (Data Loss Prevention)** ikke fungerer for innhold som inneholder et **personnummer (SSN)** når du bruker en sensitiv informasjonstype i Office 365?</span><span class="sxs-lookup"><span data-stu-id="b08c9-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="b08c9-106">I så fall må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-retningslinjene ser ut.</span><span class="sxs-lookup"><span data-stu-id="b08c9-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="b08c9-107">For en SSN-policy som er konfigurert med et konfidensnivå på 85 %, evalueres følgende for eksempel for at regelen skal utløses:</span><span class="sxs-lookup"><span data-stu-id="b08c9-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="b08c9-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 sifre, som kan være i et formatert eller uformatert mønster</span><span class="sxs-lookup"><span data-stu-id="b08c9-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="b08c9-109">**[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funksjoner ser etter SSNer i fire forskjellige mønstre:</span><span class="sxs-lookup"><span data-stu-id="b08c9-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="b08c9-110">Func_ssn finner SSNer med sterk formatering før 2011 som er formatert med bindestreker eller mellomrom (dddd-dddd eller ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="b08c9-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="b08c9-111">Func_unformatted_ssn finner SSNer med sterk formatering før 2011 som ikke er formatert som ni påfølgende sifre (ddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="b08c9-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="b08c9-112">Func_randomized_formatted_ssn finner som-koder etter 2011 som er formatert med bindestreker eller mellomrom (dddd-dddd ddd dd dd ddd)</span><span class="sxs-lookup"><span data-stu-id="b08c9-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="b08c9-113">Func_randomized_unformatted_ssn finner som-koder etter 2011 som ikke er formatert som ni påfølgende sifre (dddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="b08c9-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="b08c9-114">**[Sjekksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nei, det er ingen Checksum</span><span class="sxs-lookup"><span data-stu-id="b08c9-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="b08c9-115">**[Definisjon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** En DLP-policy er 85% sikker på at den oppdages denne typen sensitiv informasjon hvis, i nærheten av 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="b08c9-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="b08c9-116">[Funksjonen Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finner innhold som samsvarer med mønsteret.</span><span class="sxs-lookup"><span data-stu-id="b08c9-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="b08c9-117">Finner et nøkkelord fra [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="b08c9-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="b08c9-118">Eksempler på søkeord inkluderer: *Trygd, Trygd#, Soc Sec , SSN* .</span><span class="sxs-lookup"><span data-stu-id="b08c9-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="b08c9-119">Følgende eksempel utløses for eksempel DLP SSN-policyen: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="b08c9-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="b08c9-120">Hvis du vil ha mer informasjon om hva som kreves for at SSN-er skal oppdages for innholdet ditt, kan du se følgende del i denne artikkelen: [Hvilke sensitive informasjonstyper ser etter SSN-er](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="b08c9-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="b08c9-121">Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: [Hva sensitive informasjonstyper ser etter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="b08c9-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  