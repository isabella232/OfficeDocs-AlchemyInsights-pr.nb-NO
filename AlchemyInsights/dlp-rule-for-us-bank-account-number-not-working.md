---
title: DLP-regel for us-bankkontonummer fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932556"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="1b17e-102">DLP-problemer med amerikanske bankkontonumre</span><span class="sxs-lookup"><span data-stu-id="1b17e-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="1b17e-103">**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen.</span><span class="sxs-lookup"><span data-stu-id="1b17e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="1b17e-104">Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="1b17e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="1b17e-105">I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.</span><span class="sxs-lookup"><span data-stu-id="1b17e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="1b17e-106">Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene.</span><span class="sxs-lookup"><span data-stu-id="1b17e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="1b17e-107">Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider.</span><span class="sxs-lookup"><span data-stu-id="1b17e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="1b17e-108">I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.</span><span class="sxs-lookup"><span data-stu-id="1b17e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="1b17e-109">**DLP-problemer med amerikanske bankkontonumre**</span><span class="sxs-lookup"><span data-stu-id="1b17e-109">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="1b17e-110">Har du problemer med at **DLP (Data Loss Prevention)** ikke fungerer for innhold som inneholder et **amerikansk bankkontonummer** når du bruker en DLP-sensitiv informasjonstype i O365?</span><span class="sxs-lookup"><span data-stu-id="1b17e-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="1b17e-111">I så fall må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-policyen leter etter når det evalueres.</span><span class="sxs-lookup"><span data-stu-id="1b17e-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="1b17e-112">For en policy for **us-bankkontonummer** som er konfigurert med et konfidensnivå på 85 %, evalueres følgende for eksempel for at regelen skal utløses:</span><span class="sxs-lookup"><span data-stu-id="1b17e-112">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="1b17e-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 sifre</span><span class="sxs-lookup"><span data-stu-id="1b17e-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="1b17e-114">**[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 påfølgende sifre.</span><span class="sxs-lookup"><span data-stu-id="1b17e-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="1b17e-115">**[Sjekksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nei, det er ingen Checksum</span><span class="sxs-lookup"><span data-stu-id="1b17e-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="1b17e-116">**[Definisjon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** En DLP-policy er 75% sikker på at den oppdages denne typen sensitiv informasjon hvis, i nærheten av 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="1b17e-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="1b17e-117">Det regulære uttrykket Regex_usa_bank_account_number finner innhold som samsvarer med mønsteret</span><span class="sxs-lookup"><span data-stu-id="1b17e-117">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="1b17e-118">Finner et nøkkelord fra Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="1b17e-118">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="1b17e-119">Eksemplet nedenfor utløses for policyen **for us-bankkontonummer:** Kontrollere konto 78344011</span><span class="sxs-lookup"><span data-stu-id="1b17e-119">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="1b17e-120">Hvis du vil ha mer informasjon om hva som kreves for at et **amerikansk bankkontonummer** skal oppdages for innholdet ditt, kan du se følgende del i denne artikkelen: [Hvilke sensitive informasjonstyper ser etter us bankkontonummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="1b17e-120">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="1b17e-121">Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: [Hva sensitive informasjonstyper ser etter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="1b17e-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  