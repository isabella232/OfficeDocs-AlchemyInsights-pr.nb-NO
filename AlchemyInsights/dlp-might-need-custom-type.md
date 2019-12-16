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
ms.openlocfilehash: 872fca326065ada002300061c951620b3d9a8d0e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052910"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="67a4a-102">DLP trenger kanskje en egendefinert type</span><span class="sxs-lookup"><span data-stu-id="67a4a-102">DLP might need a custom type</span></span>

<span data-ttu-id="67a4a-103">Med en policy for hindring av tap av data (DLP) kan du identifisere og beskytte sensitive data i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="67a4a-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="67a4a-104">I noen scenarioer kan det hende du må opprette en egen **definert** sensitiv informasjonstype for å beskytte organisasjonens data.</span><span class="sxs-lookup"><span data-stu-id="67a4a-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="67a4a-105">Det kan for eksempel hende at organisasjonen må identifisere og beskytte ansatt-IDer eller andre data i noe format som er spesifikt for organisasjonen. I så fall kan du se følgende artikler for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="67a4a-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="67a4a-106">**Tilpasse en innebygd sensitiv informasjonstype**</span><span class="sxs-lookup"><span data-stu-id="67a4a-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="67a4a-107">Hvis en innebygd sensitiv informasjonstype dekker dine behov med bare noen få tilpasninger, kan du [tilpasse en innebygd sensitiv informasjonstype](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="67a4a-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="67a4a-108">Du kan for eksempel legge til eller fjerne nøkkelord, eller legge til eller fjerne støtte bevis, for eksempel en dato eller en adresse.</span><span class="sxs-lookup"><span data-stu-id="67a4a-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="67a4a-109">**Opprette en egendefinert sensitiv informasjonstype**</span><span class="sxs-lookup"><span data-stu-id="67a4a-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="67a4a-110">Men hvis du må identifisere og beskytte en annen type sensitiv informasjon helt, kan du [opprette en egendefinert sensitiv informasjonstype](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) i brukergrensesnittet for sikkerhets & samsvarssenter.</span><span class="sxs-lookup"><span data-stu-id="67a4a-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="67a4a-111">**Opprette en egendefinert sensitiv informasjonstype i sikkerhet & Compliance Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="67a4a-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="67a4a-112">Hvis BRUKERGRENSESNITTET ikke inneholder alle alternativene du trenger, kan du [opprette en egendefinert sensitiv informasjonstype i sikkerhet & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="67a4a-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="67a4a-113">Ved å starte med en XML-fil, kan du bruke alle tilgjengelige alternativer.</span><span class="sxs-lookup"><span data-stu-id="67a4a-113">By starting with an XML file, you can use every option available.</span></span>
