---
title: DLP-regel for kredittkortnummer fungerer ikke
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919089"
---
<span data-ttu-id="70d95-p101">Har du problemer med **Data tap forebygging (DLP)** fungerer ikke for innhold som inneholder et **Kredittkortnummer** når du bruker en type for DLP sensitiv informasjon i O365? I så fall må du kontrollere innholdet inneholder nødvendig informasjon til å utløse den DLP-policyen når de evalueres. For eksempel et **kredittkort policy** konfigurert med en konfidenskoeffisienten for 85%, for følgende evalueres og må registreres for at regelen skal utløse:</span><span class="sxs-lookup"><span data-stu-id="70d95-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="70d95-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 sifre, noe som kan være formatert eller uformatert (dddddddddddddddd) og må bestå testen Luhn.</span><span class="sxs-lookup"><span data-stu-id="70d95-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="70d95-106">**[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Svært komplekse og robust mønster som oppdager kort fra alle store merker over hele verden, inkludert Visa, Mastercard, oppdage kort, JCB, American Express, gavekort og diner-kort.</span><span class="sxs-lookup"><span data-stu-id="70d95-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="70d95-107">**[Kontrollsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, Luhn-kontrollsum</span><span class="sxs-lookup"><span data-stu-id="70d95-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="70d95-108">**[Definisjon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP-policy er 85% sikker på at det har oppdaget at sensitive opplysninger hvis, i en avstand på 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="70d95-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="70d95-109">Til Func_credit_card å finne innhold som samsvarer med mønsteret.</span><span class="sxs-lookup"><span data-stu-id="70d95-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="70d95-110">Ett av følgende er sant:</span><span class="sxs-lookup"><span data-stu-id="70d95-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="70d95-111">Det finnes et nøkkelord fra Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="70d95-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="70d95-112">Du finner et nøkkelord fra Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="70d95-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="70d95-113">Funksjonen Func_expiration_date søker etter en dato i formatet riktig dato.</span><span class="sxs-lookup"><span data-stu-id="70d95-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="70d95-114">Kontrollsummen sender</span><span class="sxs-lookup"><span data-stu-id="70d95-114">The checksum passes</span></span>
    
    <span data-ttu-id="70d95-115">Hvis du for eksempel vil følgende eksempel utløse for en Policy for DLP kredittkort nummer:</span><span class="sxs-lookup"><span data-stu-id="70d95-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="70d95-116">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="70d95-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="70d95-117">Utløper: 2/2009</span><span class="sxs-lookup"><span data-stu-id="70d95-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="70d95-118">Hvis du vil ha mer informasjon om hva som trengs for et **Kredittkortnummer** kan oppdages for innholdet, kan du se delen nedenfor i denne artikkelen: [Hva the Sensitive informasjonstyper se etter kredittkort #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="70d95-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="70d95-119">Å bruke en annen innebygd sensitiv informasjon, se følgende artikkel for å få informasjon på det som er nødvendig for andre typer: [se hva den Sensitive informasjonstyper](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="70d95-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

