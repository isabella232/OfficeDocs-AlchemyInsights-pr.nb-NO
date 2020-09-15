---
title: DLP-regel for amerikansk/britisk Passport-nummer fungerer ikke
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679233"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="c82e9-102">Problemer med DLP-US/Storbritannia Passport-numre</span><span class="sxs-lookup"><span data-stu-id="c82e9-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="c82e9-103">**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="c82e9-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c82e9-104">**DLP-problemer med amerikanske/britiske Passport-numre**</span><span class="sxs-lookup"><span data-stu-id="c82e9-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="c82e9-105">Har du problemer med tap av datatap **(DLP)** fungerer ikke for innhold som inneholder et **amerikansk/britisk Passport-nummer** når du bruker en DLP sensitiv informasjons type i O365?</span><span class="sxs-lookup"><span data-stu-id="c82e9-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="c82e9-106">Hvis det er tilfelle, må du kontrollere at innholdet inneholder den nødvendige informasjonen for hva DLP-policyen ser ut når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="c82e9-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="c82e9-107">Hvis du for eksempel har konfigurert en **US/Storbritannia Passport Number-** policy med et konfidenskoeffisienten-nivå på 75%, evalueres følgende og må oppdages for at regelen skal utløse</span><span class="sxs-lookup"><span data-stu-id="c82e9-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="c82e9-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Ni sifre</span><span class="sxs-lookup"><span data-stu-id="c82e9-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="c82e9-109">**[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Ni påfølgende sifre</span><span class="sxs-lookup"><span data-stu-id="c82e9-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="c82e9-110">**[Kontroll sum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nei, det er ingen kontroll sum</span><span class="sxs-lookup"><span data-stu-id="c82e9-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="c82e9-111">**[Definisjon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** En DLP-policy er 75% sikker på at den har funnet denne typen sensitiv informasjon hvis, innenfor en nærhet av 300-tegn:</span><span class="sxs-lookup"><span data-stu-id="c82e9-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c82e9-112">Funksjonen Func_usa_uk_passport finner innhold som Sams varer med mønsteret.</span><span class="sxs-lookup"><span data-stu-id="c82e9-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="c82e9-113">Et nøkkel ord fra Keyword_passport blir funnet.</span><span class="sxs-lookup"><span data-stu-id="c82e9-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="c82e9-114">Følgende eksempel vil for eksempel utløse den **amerikanske/britiske Passport Number** -policyen: amerikansk pass nummer 123456789</span><span class="sxs-lookup"><span data-stu-id="c82e9-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="c82e9-115">Hvis du vil ha mer informasjon om hva som kreves for at et amerikansk/britisk Passport-nummer skal oppdages for innholdet, kan du se følgende avsnitt i denne artikkelen: [hva de sensitive informasjons typene ser ut for amerikansk/britisk Passport-nummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="c82e9-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="c82e9-116">Hvis du bruker en annen innebygd sensitiv informasjons type, kan du se følgende artikkel for informasjon om hva som er nødvendig for andre typer: [hva de sensitive informasjons typene ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="c82e9-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  