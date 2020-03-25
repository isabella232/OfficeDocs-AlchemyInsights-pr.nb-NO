---
title: DLP-regel for kredittkortnummer fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932452"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="dbc33-102">DLP-problemer med kredittkortnumre</span><span class="sxs-lookup"><span data-stu-id="dbc33-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="dbc33-103">**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen.</span><span class="sxs-lookup"><span data-stu-id="dbc33-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="dbc33-104">Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="dbc33-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="dbc33-105">I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.</span><span class="sxs-lookup"><span data-stu-id="dbc33-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="dbc33-106">Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene.</span><span class="sxs-lookup"><span data-stu-id="dbc33-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="dbc33-107">Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider.</span><span class="sxs-lookup"><span data-stu-id="dbc33-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="dbc33-108">I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.</span><span class="sxs-lookup"><span data-stu-id="dbc33-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="dbc33-109">**DLP-problemer med kredittkortnumre**</span><span class="sxs-lookup"><span data-stu-id="dbc33-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="dbc33-110">Har du problemer med at **DLP ikke** fungerer for innhold som inneholder et **kredittkortnummer** når du bruker en DLP-sensitiv informasjonstype i O365?</span><span class="sxs-lookup"><span data-stu-id="dbc33-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="dbc33-111">I så fall må du kontrollere at innholdet inneholder den nødvendige informasjonen for å utløse DLP-policyen når det evalueres.</span><span class="sxs-lookup"><span data-stu-id="dbc33-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="dbc33-112">For en **kredittkortpolicy** som er konfigurert med et konfidensnivå på 85 %, evalueres følgende for eksempel for at regelen skal utløses:</span><span class="sxs-lookup"><span data-stu-id="dbc33-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="dbc33-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 sifre som kan formateres eller uformateres (ddddddddddddddddddddddddddddd) og må bestå Luhn-testen.</span><span class="sxs-lookup"><span data-stu-id="dbc33-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="dbc33-114">**[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Svært komplekst og robust mønster som oppdager kort fra alle store merker over hele verden, inkludert Visa, MasterCard, Discover Card, JCB, American Express, gavekort og dinerkort.</span><span class="sxs-lookup"><span data-stu-id="dbc33-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="dbc33-115">**[Sjekksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, Luhn-sjekksummen</span><span class="sxs-lookup"><span data-stu-id="dbc33-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="dbc33-116">**[Definisjon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** En DLP-policy er 85% sikker på at den oppdages denne typen sensitiv informasjon hvis, i nærheten av 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="dbc33-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="dbc33-117">Funksjonen Func_credit_card finner innhold som samsvarer med mønsteret.</span><span class="sxs-lookup"><span data-stu-id="dbc33-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="dbc33-118">Ett av følgende er sant:</span><span class="sxs-lookup"><span data-stu-id="dbc33-118">One of the following is true:</span></span>

  - <span data-ttu-id="dbc33-119">Finner et nøkkelord fra Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="dbc33-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="dbc33-120">Finner et nøkkelord fra Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="dbc33-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="dbc33-121">Funksjonen Func_expiration_date finner en dato i riktig datoformat.</span><span class="sxs-lookup"><span data-stu-id="dbc33-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="dbc33-122">Kontrollsummen passerer</span><span class="sxs-lookup"><span data-stu-id="dbc33-122">The checksum passes</span></span>

    <span data-ttu-id="dbc33-123">Eksemplet nedenfor utløses for eksempel en DLP-kredittkortnummerpolicy:</span><span class="sxs-lookup"><span data-stu-id="dbc33-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="dbc33-124">Visum: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="dbc33-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="dbc33-125">Utløper: 2/2009</span><span class="sxs-lookup"><span data-stu-id="dbc33-125">Expires: 2/2009</span></span>

<span data-ttu-id="dbc33-126">Hvis du vil ha mer informasjon om hva som kreves for at et **kredittkortnummer** skal oppdages for innholdet ditt, kan du se følgende del i denne artikkelen: [Hvilke sensitive informasjonstyper ser etter kredittkort#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="dbc33-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="dbc33-127">Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: [Hva sensitive informasjonstyper ser etter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="dbc33-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  