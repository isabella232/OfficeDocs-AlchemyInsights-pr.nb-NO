---
title: DLP-regel for USA / UK passnummer fungerer ikke
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912113"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="d67bc-102">Problemer med DLP - USA / UK Passport tall</span><span class="sxs-lookup"><span data-stu-id="d67bc-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="d67bc-p101">Har du problemer med **Data tap forebygging (DLP)** fungerer ikke for innhold som inneholder en **US / UK passnummer** når du bruker en type for DLP sensitiv informasjon i O365? Hvis dette er tilfelle, kontroller at innholdet inneholder nødvendig informasjon for det DLP-policyen er ute etter når de evalueres.</span><span class="sxs-lookup"><span data-stu-id="d67bc-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="d67bc-105">For eksempel for en **US / UK passnummer** policy som er konfigurert med en konfidenskoeffisienten for 75% følgende evalueres og må registreres for at regelen skal utløse</span><span class="sxs-lookup"><span data-stu-id="d67bc-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="d67bc-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Ni sifre</span><span class="sxs-lookup"><span data-stu-id="d67bc-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="d67bc-107">**[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Ni etterfølgende sifre</span><span class="sxs-lookup"><span data-stu-id="d67bc-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="d67bc-108">**[Kontrollsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nei, det finnes ingen kontrollsum</span><span class="sxs-lookup"><span data-stu-id="d67bc-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="d67bc-109">**[Definisjon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP-policy er 75% sikker på at det har oppdaget at sensitive opplysninger hvis, i en avstand på 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="d67bc-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="d67bc-110">Til Func_usa_uk_passport å finne innhold som samsvarer med mønsteret.</span><span class="sxs-lookup"><span data-stu-id="d67bc-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="d67bc-111">Det finnes et nøkkelord fra Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="d67bc-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="d67bc-112">For eksempel følgende eksempel vil utløse den **US / UK passnummer** policy: amerikansk pass tallet 123456789</span><span class="sxs-lookup"><span data-stu-id="d67bc-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="d67bc-113">For mer informasjon om hva som trengs for en US / UK passnummer kan oppdages for innholdet, kan du se delen nedenfor i denne artikkelen: [Hva den Sensitive informasjonstyper utseende for USA / UK passnummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="d67bc-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="d67bc-114">Å bruke en annen innebygd sensitiv informasjon, se følgende artikkel for å få informasjon på det som er nødvendig for andre typer: [se hva den Sensitive informasjonstyper](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d67bc-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

