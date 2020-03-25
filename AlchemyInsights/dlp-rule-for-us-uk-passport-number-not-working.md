---
title: DLP-regel for us/UK Passport-nummer fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931271"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="84c6a-102">Problemer med DLP - US / UK passnumre</span><span class="sxs-lookup"><span data-stu-id="84c6a-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="84c6a-103">**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen.</span><span class="sxs-lookup"><span data-stu-id="84c6a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="84c6a-104">Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="84c6a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="84c6a-105">I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.</span><span class="sxs-lookup"><span data-stu-id="84c6a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="84c6a-106">Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene.</span><span class="sxs-lookup"><span data-stu-id="84c6a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="84c6a-107">Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider.</span><span class="sxs-lookup"><span data-stu-id="84c6a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="84c6a-108">I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.</span><span class="sxs-lookup"><span data-stu-id="84c6a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="84c6a-109">**DLP-problemer med amerikanske/britiske passnumre**</span><span class="sxs-lookup"><span data-stu-id="84c6a-109">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="84c6a-110">Har du problemer med at **DLP ikke** fungerer for innhold som inneholder et **amerikansk/britisk passnummer** når du bruker en DLP-sensitiv informasjonstype i O365?</span><span class="sxs-lookup"><span data-stu-id="84c6a-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="84c6a-111">I så fall må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-policyen leter etter når det evalueres.</span><span class="sxs-lookup"><span data-stu-id="84c6a-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="84c6a-112">For eksempel, for en **amerikansk / britisk passnummerpolicy** konfigurert med et konfidensnivå på 75%, evalueres følgende for at regelen skal utløses</span><span class="sxs-lookup"><span data-stu-id="84c6a-112">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="84c6a-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Ni sifre</span><span class="sxs-lookup"><span data-stu-id="84c6a-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="84c6a-114">**[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Ni tall på rad</span><span class="sxs-lookup"><span data-stu-id="84c6a-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="84c6a-115">**[Sjekksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nei, det er ingen Checksum</span><span class="sxs-lookup"><span data-stu-id="84c6a-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="84c6a-116">**[Definisjon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** En DLP-policy er 75% sikker på at den oppdages denne typen sensitiv informasjon hvis, i nærheten av 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="84c6a-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="84c6a-117">Funksjonen Func_usa_uk_passport finner innhold som samsvarer med mønsteret.</span><span class="sxs-lookup"><span data-stu-id="84c6a-117">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="84c6a-118">Finner et nøkkelord fra Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="84c6a-118">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="84c6a-119">Følgende eksempel utløses for eksempel policyen for passnummer i **USA/Storbritannia:** US Passport-nummer 123456789</span><span class="sxs-lookup"><span data-stu-id="84c6a-119">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="84c6a-120">Hvis du vil ha mer informasjon om hva som kreves for at et amerikansk/britisk passnummer skal oppdages for innholdet ditt, kan du se følgende avsnitt i denne artikkelen: [Hva sensitive informasjonstyper ser etter us/uk passport nummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="84c6a-120">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="84c6a-121">Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: [Hva sensitive informasjonstyper ser etter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="84c6a-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  