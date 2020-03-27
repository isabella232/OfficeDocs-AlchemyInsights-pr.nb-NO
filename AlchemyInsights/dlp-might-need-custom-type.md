---
title: DLP trenger kanskje en egendefinert type
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 87fcb5c3cc9ccd525265097b66d9d9b3a85c5feb
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977279"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="6ebf4-102">DLP trenger kanskje en egendefinert type</span><span class="sxs-lookup"><span data-stu-id="6ebf4-102">DLP might need a custom type</span></span>

<span data-ttu-id="6ebf4-103">**Viktig:** I løpet av disse enestående tider, vi tar skritt for å sikre at SharePoint Online og OneDrive-tjenester forblir svært tilgjengelige - Vennligst besøk [SharePoint Online midlertidige funksjonsjusteringer](https://aka.ms/ODSPAdjustments) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="6ebf4-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="6ebf4-104">**DLP kan kreve en egendefinert informasjonstype**</span><span class="sxs-lookup"><span data-stu-id="6ebf4-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="6ebf4-105">Med en policy for hindring av tap av data (DLP) kan du identifisere og beskytte sensitive data i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="6ebf4-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="6ebf4-106">I noen scenarier må du kanskje opprette din egen **egendefinerte** sensitive informasjonstype for å beskytte organisasjonens data.</span><span class="sxs-lookup"><span data-stu-id="6ebf4-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="6ebf4-107">Organisasjonen må for eksempel kanskje identifisere og beskytte ansatt-IDer eller andre data i et format som er spesifikt for organisasjonen. I så fall kan du se følgende artikler for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="6ebf4-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="6ebf4-108">**Tilpasse en innebygd sensitiv informasjonstype**</span><span class="sxs-lookup"><span data-stu-id="6ebf4-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="6ebf4-109">Hvis en innebygd sensitiv informasjonstype vil møte dine behov med bare noen få tweaks, kan du [tilpasse en innebygd sensitiv informasjonstype](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="6ebf4-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="6ebf4-110">Du kan for eksempel legge til eller fjerne søkeord, eller legge til eller fjerne støttebevis, for eksempel en dato eller adresse.</span><span class="sxs-lookup"><span data-stu-id="6ebf4-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="6ebf4-111">**Opprette en egendefinert sensitiv informasjonstype**</span><span class="sxs-lookup"><span data-stu-id="6ebf4-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="6ebf4-112">Men hvis du trenger å identifisere og beskytte en annen type sensitiv informasjon helt, kan du [opprette en egendefinert sensitiv informasjonstype](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) i brukergrensesnittet i Security & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="6ebf4-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="6ebf4-113">**Opprette en egendefinert sensitiv informasjonstype i Security & Compliance Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="6ebf4-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="6ebf4-114">Til slutt, hvis brukergrensesnittet ikke inneholder alle alternativene du trenger, kan du [opprette en egendefinert sensitiv informasjonstype i Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="6ebf4-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="6ebf4-115">Ved å starte med en XML-fil kan du bruke alle tilgjengelige alternativer.</span><span class="sxs-lookup"><span data-stu-id="6ebf4-115">By starting with an XML file, you can use every option available.</span></span>
