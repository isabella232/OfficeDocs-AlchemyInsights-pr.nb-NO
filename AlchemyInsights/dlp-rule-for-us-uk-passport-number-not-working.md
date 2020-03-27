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
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977115"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="a98fb-102">Problemer med DLP - US / UK passnumre</span><span class="sxs-lookup"><span data-stu-id="a98fb-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="a98fb-103">**Viktig:** I løpet av disse enestående tider, vi tar skritt for å sikre at SharePoint Online og OneDrive-tjenester forblir svært tilgjengelige - Vennligst besøk [SharePoint Online midlertidige funksjonsjusteringer](https://aka.ms/ODSPAdjustments) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="a98fb-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="a98fb-104">**DLP-problemer med amerikanske/britiske passnumre**</span><span class="sxs-lookup"><span data-stu-id="a98fb-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="a98fb-105">Har du problemer med at **DLP ikke** fungerer for innhold som inneholder et **amerikansk/britisk passnummer** når du bruker en DLP-sensitiv informasjonstype i O365?</span><span class="sxs-lookup"><span data-stu-id="a98fb-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="a98fb-106">I så fall må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-policyen leter etter når det evalueres.</span><span class="sxs-lookup"><span data-stu-id="a98fb-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="a98fb-107">For eksempel, for en **amerikansk / britisk passnummerpolicy** konfigurert med et konfidensnivå på 75%, evalueres følgende for at regelen skal utløses</span><span class="sxs-lookup"><span data-stu-id="a98fb-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="a98fb-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Ni sifre</span><span class="sxs-lookup"><span data-stu-id="a98fb-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="a98fb-109">**[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Ni tall på rad</span><span class="sxs-lookup"><span data-stu-id="a98fb-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="a98fb-110">**[Sjekksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nei, det er ingen Checksum</span><span class="sxs-lookup"><span data-stu-id="a98fb-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="a98fb-111">**[Definisjon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** En DLP-policy er 75% sikker på at den oppdages denne typen sensitiv informasjon hvis, i nærheten av 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="a98fb-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a98fb-112">Funksjonen Func_usa_uk_passport finner innhold som samsvarer med mønsteret.</span><span class="sxs-lookup"><span data-stu-id="a98fb-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="a98fb-113">Finner et nøkkelord fra Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="a98fb-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="a98fb-114">Følgende eksempel utløses for eksempel policyen for passnummer i **USA/Storbritannia:** US Passport-nummer 123456789</span><span class="sxs-lookup"><span data-stu-id="a98fb-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="a98fb-115">Hvis du vil ha mer informasjon om hva som kreves for at et amerikansk/britisk passnummer skal oppdages for innholdet ditt, kan du se følgende avsnitt i denne artikkelen: [Hva sensitive informasjonstyper ser etter us/uk passport nummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="a98fb-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="a98fb-116">Hvis du bruker en annen innebygd sensitiv informasjonstype, kan du se følgende artikkel for informasjon om hva som kreves for andre typer: [Hva sensitive informasjonstyper ser etter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a98fb-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  