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
ms.openlocfilehash: fffd355279b064b31c0a8bf60518b15ee1ed1848
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389442"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="cee52-102">DLP-problemer med personnumre</span><span class="sxs-lookup"><span data-stu-id="cee52-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="cee52-103">Har du problemer med **Data tap forebygging (DLP)** fungerer ikke for innhold som inneholder et **Personnummer (SSN)** når du bruker en type sensitiv informasjon i Office 365?</span><span class="sxs-lookup"><span data-stu-id="cee52-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="cee52-104">I så fall må du kontrollere at innholdet inneholder nødvendig informasjon for det DLP-policyen er ute.</span><span class="sxs-lookup"><span data-stu-id="cee52-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="cee52-105">For eksempel for en SSN-policy er konfigurert med en konfidenskoeffisienten for 85%, følgende blir evaluert, og må registreres for at regelen skal utløse:</span><span class="sxs-lookup"><span data-stu-id="cee52-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="cee52-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 sifre, noe som kan være i en formatert eller uformatert mønster</span><span class="sxs-lookup"><span data-stu-id="cee52-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="cee52-107">**[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funksjoner se etter SSNs i fire ulike mønstre:</span><span class="sxs-lookup"><span data-stu-id="cee52-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="cee52-108">Func_ssn søker etter SSNs med pre-2011 Sterk formatering som er formatert med bindestreker eller mellomrom (ddd-dd-dddd eller ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="cee52-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="cee52-109">Func_unformatted_ssn søker etter SSNs med pre-2011 Sterk formatering som er formatert med ni etterfølgende sifre (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="cee52-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="cee52-110">Func_randomized_formatted_ssn søker etter post-2011-SSNs som er formatert med bindestreker eller mellomrom (ddd-dd-dddd eller ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="cee52-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="cee52-111">Func_randomized_unformatted_ssn søker etter post-2011-SSNs som er formatert med ni etterfølgende sifre (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="cee52-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="cee52-112">**[Kontrollsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nei, det finnes ingen kontrollsum</span><span class="sxs-lookup"><span data-stu-id="cee52-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="cee52-113">**[Definisjon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP-policy er 85% sikker på at det har oppdaget at sensitive opplysninger hvis, i en avstand på 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="cee52-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="cee52-114">[Funksjonen Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) søker etter innhold som samsvarer med mønsteret.</span><span class="sxs-lookup"><span data-stu-id="cee52-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="cee52-115">Det finnes et nøkkelord fra [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="cee52-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="cee52-116">Eksempler på nøkkelord inkluderer: *Social Security, Trygd #, Orb sek, Personnummeret* .</span><span class="sxs-lookup"><span data-stu-id="cee52-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="cee52-117">Hvis du for eksempel følgende eksempel vil utløse for policyen DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="cee52-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="cee52-118">Hvis du vil ha mer informasjon om hva som er nødvendig for SSNs blir registrert for innholdet, kan du se delen nedenfor i denne artikkelen: [Hva the Sensitive informasjonstyper se etter SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="cee52-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="cee52-119">Å bruke en annen innebygd sensitiv informasjon, se følgende artikkel for å få informasjon på det som er nødvendig for andre typer: [se hva den Sensitive informasjonstyper](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="cee52-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  