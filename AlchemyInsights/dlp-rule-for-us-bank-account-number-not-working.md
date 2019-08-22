---
title: DLP-regel for oss bankkontonummeret fungerer ikke
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
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529885"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="bf752-102">DLP-problemer med oss bankkontonumre</span><span class="sxs-lookup"><span data-stu-id="bf752-102">DLP issues with US Bank Account Numbers</span></span>

<span data-ttu-id="bf752-103">Har du problemer med **Data tap forebygging (DLP)** fungerer ikke for innhold som inneholder et **Amerikansk bankkontonummeret** når du bruker en type for DLP sensitiv informasjon i O365?</span><span class="sxs-lookup"><span data-stu-id="bf752-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="bf752-104">Hvis dette er tilfelle, kontroller at innholdet inneholder nødvendig informasjon for det DLP-policyen er ute etter når de evalueres.</span><span class="sxs-lookup"><span data-stu-id="bf752-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="bf752-105">For eksempel, for en **Amerikansk bankkontonummeret** policy konfigurert med en konfidenskoeffisienten for 85%, følgende evalueres og må registreres for at regelen skal utløse:</span><span class="sxs-lookup"><span data-stu-id="bf752-105">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="bf752-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17-sifre</span><span class="sxs-lookup"><span data-stu-id="bf752-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="bf752-107">**[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 etterfølgende sifre.</span><span class="sxs-lookup"><span data-stu-id="bf752-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="bf752-108">**[Kontrollsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nei, det finnes ingen kontrollsum</span><span class="sxs-lookup"><span data-stu-id="bf752-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="bf752-109">**[Definisjon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP-policy er 75% sikker på at det har oppdaget at sensitive opplysninger hvis, i en avstand på 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="bf752-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="bf752-110">Det vanlige uttrykket Regex_usa_bank_account_number finner innhold som samsvarer med mønsteret</span><span class="sxs-lookup"><span data-stu-id="bf752-110">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="bf752-111">Det finnes et nøkkelord fra Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="bf752-111">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="bf752-112">Hvis du for eksempel følgende eksempel vil utløse for **Amerikanske bankkontonummeret** policyen: sjekkonto 78344011</span><span class="sxs-lookup"><span data-stu-id="bf752-112">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="bf752-113">Hvis du vil ha mer informasjon om hva som trengs for et **Amerikansk bankkontonummeret** kan oppdages for innholdet, kan du se delen nedenfor i denne artikkelen: [Hva the Sensitive informasjonstyper se etter Amerikanske bankkontonummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="bf752-113">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="bf752-114">Å bruke en annen innebygd sensitiv informasjon, se følgende artikkel for å få informasjon på det som er nødvendig for andre typer: [se hva den Sensitive informasjonstyper](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="bf752-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  