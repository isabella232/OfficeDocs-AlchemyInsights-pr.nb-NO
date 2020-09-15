---
title: DLP kan trenge en egen definert type
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712193"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="d0df2-102">DLP kan trenge en egen definert type</span><span class="sxs-lookup"><span data-stu-id="d0df2-102">DLP might need a custom type</span></span>

<span data-ttu-id="d0df2-103">**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="d0df2-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d0df2-104">**DLP kan kreve en egen definert informasjons type**</span><span class="sxs-lookup"><span data-stu-id="d0df2-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="d0df2-105">Med en policy for hindring av tap av data (HINDRING) kan du identifisere og beskytte sensitive data i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="d0df2-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="d0df2-106">I noen scenarioer kan det hende du må opprette en egen **definert** sensitiv informasjons type for å beskytte organisasjonens data.</span><span class="sxs-lookup"><span data-stu-id="d0df2-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="d0df2-107">Organisasjonen kan for eksempel identifisere og beskytte ansatt-IDer eller andre data i et bestemt format for organisasjonen. Hvis dette er tilfelle, kan du se følgende artikler for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="d0df2-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="d0df2-108">**Tilpasse en innebygd sensitiv informasjons type**</span><span class="sxs-lookup"><span data-stu-id="d0df2-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="d0df2-109">Hvis en innebygd sensitiv informasjons type oppfyller behovene dine med bare noen få tilpasninger, kan du [tilpasse en innebygd sensitiv informasjons type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="d0df2-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="d0df2-110">Du kan for eksempel legge til eller fjerne nøkkel ord, eller legge til eller fjerne støtte bevis som en dato eller adresse.</span><span class="sxs-lookup"><span data-stu-id="d0df2-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="d0df2-111">**Opprette en egen definert sensitiv informasjons type**</span><span class="sxs-lookup"><span data-stu-id="d0df2-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="d0df2-112">Men hvis du trenger å identifisere og beskytte en annen type sensitiv informasjon helt, kan du [opprette en egen definert sensitiv informasjons type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) i bruker grensesnittet til sikkerhets & samsvars senteret.</span><span class="sxs-lookup"><span data-stu-id="d0df2-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="d0df2-113">**Opprette en egen definert sensitiv informasjons type i sikkerhets & overholdelses senteret PowerShell**</span><span class="sxs-lookup"><span data-stu-id="d0df2-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="d0df2-114">Til slutt, hvis bruker grensesnittet ikke gir alle alternativene du trenger, kan du [opprette en egen definert sensitiv informasjons type i sikkerhets & Overholdelses senteret PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="d0df2-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="d0df2-115">Når du starter med en XML-fil, kan du bruke alle alternativene som er tilgjengelige.</span><span class="sxs-lookup"><span data-stu-id="d0df2-115">By starting with an XML file, you can use every option available.</span></span>
