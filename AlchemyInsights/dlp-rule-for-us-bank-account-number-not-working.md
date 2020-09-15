---
title: DLP-regel for amerikansk bank konto nummer fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679305"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="4c724-102">DLP-problemer med amerikanske bank konto numre</span><span class="sxs-lookup"><span data-stu-id="4c724-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="4c724-103">**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="4c724-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="4c724-104">**DLP-problemer med amerikanske bank konto numre**</span><span class="sxs-lookup"><span data-stu-id="4c724-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="4c724-105">Har du problemer med **tap av datatap (DLP)** fungerer ikke for innhold som inneholder et **amerikansk bank konto nummer** når du bruker en DLP sensitiv informasjons type i O365?</span><span class="sxs-lookup"><span data-stu-id="4c724-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="4c724-106">Hvis det er tilfelle, må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-policyen ser ut når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="4c724-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="4c724-107">For en **amerikansk bank konto nummer** policy, som for eksempel er konfigurert med et konfidenskoeffisienten-nivå på 85%, evalueres følgende og må oppdages for at regelen skal utløse:</span><span class="sxs-lookup"><span data-stu-id="4c724-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="4c724-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 sifre</span><span class="sxs-lookup"><span data-stu-id="4c724-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="4c724-109">**[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 påfølgende sifre.</span><span class="sxs-lookup"><span data-stu-id="4c724-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="4c724-110">**[Kontroll sum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nei, det er ingen kontroll sum</span><span class="sxs-lookup"><span data-stu-id="4c724-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="4c724-111">**[Definisjon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** En DLP-policy er 75% sikker på at den har funnet denne typen sensitiv informasjon hvis, innenfor en nærhet av 300-tegn:</span><span class="sxs-lookup"><span data-stu-id="4c724-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="4c724-112">Det vanlige uttrykket Regex_usa_bank_account_number finner innhold som Sams varer med mønsteret</span><span class="sxs-lookup"><span data-stu-id="4c724-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="4c724-113">Et nøkkel ord fra Keyword_usa_Bank_Account blir funnet.</span><span class="sxs-lookup"><span data-stu-id="4c724-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="4c724-114">Følgende eksempel vil for eksempel utløse den **amerikanske bank konto nummer** policyen: kontrollere konto 78344011</span><span class="sxs-lookup"><span data-stu-id="4c724-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="4c724-115">Hvis du vil ha mer informasjon om hva som kreves for at et **amerikansk bank konto nummer** skal oppdages for innholdet, kan du se følgende avsnitt i denne artikkelen: [hva de sensitive informasjons typene ser ut for amerikansk bank konto nummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="4c724-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="4c724-116">Hvis du bruker en annen innebygd sensitiv informasjons type, kan du se følgende artikkel for informasjon om hva som er nødvendig for andre typer: [hva de sensitive informasjons typene ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="4c724-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  