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
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529964"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="f4bb7-102">DLP-problemer med kredittkortnumre</span><span class="sxs-lookup"><span data-stu-id="f4bb7-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="f4bb7-103">Har du problemer med **Data tap forebygging (DLP)** fungerer ikke for innhold som inneholder et **Kredittkortnummer** når du bruker en type for DLP sensitiv informasjon i O365?</span><span class="sxs-lookup"><span data-stu-id="f4bb7-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="f4bb7-104">I så fall må du kontrollere innholdet inneholder nødvendig informasjon til å utløse den DLP-policyen når de evalueres.</span><span class="sxs-lookup"><span data-stu-id="f4bb7-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="f4bb7-105">For eksempel et **kredittkort policy** konfigurert med en konfidenskoeffisienten for 85%, for følgende evalueres og må registreres for at regelen skal utløse:</span><span class="sxs-lookup"><span data-stu-id="f4bb7-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="f4bb7-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 sifre, noe som kan være formatert eller uformatert (dddddddddddddddd) og må bestå testen Luhn.</span><span class="sxs-lookup"><span data-stu-id="f4bb7-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="f4bb7-107">**[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Svært komplekse og robust mønster som oppdager kort fra alle store merker over hele verden, inkludert Visa, MasterCard, oppdage kort, JCB, American Express, gavekort og diner-kort.</span><span class="sxs-lookup"><span data-stu-id="f4bb7-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="f4bb7-108">**[Kontrollsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, Luhn-kontrollsum</span><span class="sxs-lookup"><span data-stu-id="f4bb7-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="f4bb7-109">**[Definisjon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP-policy er 85% sikker på at det har oppdaget at sensitive opplysninger hvis, i en avstand på 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="f4bb7-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="f4bb7-110">Til Func_credit_card å finne innhold som samsvarer med mønsteret.</span><span class="sxs-lookup"><span data-stu-id="f4bb7-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="f4bb7-111">Ett av følgende er sant:</span><span class="sxs-lookup"><span data-stu-id="f4bb7-111">One of the following is true:</span></span>

  - <span data-ttu-id="f4bb7-112">Det finnes et nøkkelord fra Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="f4bb7-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="f4bb7-113">Du finner et nøkkelord fra Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="f4bb7-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="f4bb7-114">Funksjonen Func_expiration_date søker etter en dato i formatet riktig dato.</span><span class="sxs-lookup"><span data-stu-id="f4bb7-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="f4bb7-115">Kontrollsummen sender</span><span class="sxs-lookup"><span data-stu-id="f4bb7-115">The checksum passes</span></span>

    <span data-ttu-id="f4bb7-116">Hvis du for eksempel vil følgende eksempel utløse for en Policy for DLP kredittkort nummer:</span><span class="sxs-lookup"><span data-stu-id="f4bb7-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="f4bb7-117">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="f4bb7-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="f4bb7-118">Utløper: 2/2009</span><span class="sxs-lookup"><span data-stu-id="f4bb7-118">Expires: 2/2009</span></span>

<span data-ttu-id="f4bb7-119">Hvis du vil ha mer informasjon om hva som trengs for et **Kredittkortnummer** kan oppdages for innholdet, kan du se delen nedenfor i denne artikkelen: [Hva the Sensitive informasjonstyper se etter kredittkort #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="f4bb7-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="f4bb7-120">Å bruke en annen innebygd sensitiv informasjon, se følgende artikkel for å få informasjon på det som er nødvendig for andre typer: [se hva den Sensitive informasjonstyper](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="f4bb7-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  