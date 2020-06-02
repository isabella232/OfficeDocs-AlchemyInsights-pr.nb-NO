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
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507379"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="02351-102">DLP-problemer med personnummer</span><span class="sxs-lookup"><span data-stu-id="02351-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="02351-103">**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="02351-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="02351-104">**DLP-problemer med SSN-er**</span><span class="sxs-lookup"><span data-stu-id="02351-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="02351-105">Har du problemer med **at Data Loss Prevention (DLP)** ikke fungerer for innhold som inneholder et **SSN (Social Security Number)** når du bruker en sensitiv informasjonstype i Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="02351-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="02351-106">I så fall må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-retningslinjene ser ut.</span><span class="sxs-lookup"><span data-stu-id="02351-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="02351-107">For en SSN-policy som er konfigurert med et konfidensnivå på 85 %, evalueres følgende og må oppdages for at regelen skal utløses:</span><span class="sxs-lookup"><span data-stu-id="02351-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="02351-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 sifre, som kan være i et formatert eller uformatert mønster</span><span class="sxs-lookup"><span data-stu-id="02351-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="02351-109">**[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funksjoner ser etter SSNer i fire forskjellige mønstre:</span><span class="sxs-lookup"><span data-stu-id="02351-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="02351-110">Func_ssn finner SSNer med før 2011 sterk formatering som er formatert med bindestreker eller mellomrom (ddd-dddd ELLER ddd ddd ddddd)</span><span class="sxs-lookup"><span data-stu-id="02351-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="02351-111">Func_unformatted_ssn finner SSNer med før 2011 sterk formatering som er uformatert som ni påfølgende sifre (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="02351-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="02351-112">Func_randomized_formatted_ssn finner SSN-er etter 2011 som er formatert med bindestreker eller mellomrom (ddd-dddd ELLER ddd ddd ddddd)</span><span class="sxs-lookup"><span data-stu-id="02351-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="02351-113">Func_randomized_unformatted_ssn finner SSNer etter 2011 som ikke er formatert som ni påfølgende sifre (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="02351-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="02351-114">**[Sjekksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nei, det er ingen kontrollsum</span><span class="sxs-lookup"><span data-stu-id="02351-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="02351-115">**[Definisjon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** En DLP-policy er 85 % sikker på at den oppdages denne typen sensitiv informasjon hvis, i nærheten av 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="02351-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="02351-116">[Funksjonen Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finner innhold som samsvarer med mønsteret.</span><span class="sxs-lookup"><span data-stu-id="02351-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="02351-117">Du finner et nøkkelord fra [Keyword_ssn.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="02351-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="02351-118">Eksempler på nøkkelord inkluderer: *Social Security, Social Security#, Soc Sec , SSN* .</span><span class="sxs-lookup"><span data-stu-id="02351-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="02351-119">Følgende eksempel utløses for eksempel for DLP SSN-policyen: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="02351-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="02351-120">Hvis du vil ha mer informasjon om hva som kreves for at SSNer skal oppdages for innholdet ditt, kan du se følgende del i denne artikkelen: [Hva sensitive informasjonstyper ser etter SSNer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="02351-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="02351-121">Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: [Hva sensitive informasjonstyper ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="02351-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  