---
title: DLP fungerer ikke som forventet
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707819"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="722e2-102">DLP fungerer ikke som forventet</span><span class="sxs-lookup"><span data-stu-id="722e2-102">DLP not working as expected</span></span>

<span data-ttu-id="722e2-103">**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="722e2-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="722e2-104">**Konfigurere DLP**</span><span class="sxs-lookup"><span data-stu-id="722e2-104">**Setting up DLP**</span></span>

<span data-ttu-id="722e2-105">Har du problemer med hindring av **tap av data (DLP)** i Office 365, fungerer ikke som forventet?</span><span class="sxs-lookup"><span data-stu-id="722e2-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="722e2-106">Hvis det er det, må du kontrollere at **DLP-policyen** er riktig konfigurert, og at dataene inneholder det **DLP-policyen** ser etter når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="722e2-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="722e2-107">Med DLP-policyer kan du identifisere og beskytte sensitiv informasjon i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="722e2-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="722e2-108">Bruk informasjonen her for å [](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)konfigurere DLP-policyer.</span><span class="sxs-lookup"><span data-stu-id="722e2-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="722e2-109">**Hvilke DLP-policyer ser etter**</span><span class="sxs-lookup"><span data-stu-id="722e2-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="722e2-110">Når du bruker de **innebygde sensitive** informasjonstypene i sikkerhets- og samsvarssentrene, ser DLP-policyer etter bestemte mønstre og elementer når disse sensitive typene oppdages.</span><span class="sxs-lookup"><span data-stu-id="722e2-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="722e2-111">**Innebygde typer sensitiv informasjon**</span><span class="sxs-lookup"><span data-stu-id="722e2-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="722e2-112">Hvis du vil ha informasjon om de innebygde sensitive typene og hva en DLP-policy ser etter når du oppdager sensitive typer, kan du se: Hva de [sensitive informasjonstypene ser etter.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="722e2-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="722e2-113">**Egendefinerte sensitive informasjonstyper**</span><span class="sxs-lookup"><span data-stu-id="722e2-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="722e2-114">Hvis du prøver å opprette egendefinerte sensitive informasjonstyper, kan du bruke følgende artikkel for informasjon om hvordan du oppretter en egendefinert sensitiv type: Opprette en egendefinert [sensitiv informasjonstype.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="722e2-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="722e2-115">**Teste en DLP-policy**</span><span class="sxs-lookup"><span data-stu-id="722e2-115">**Test a DLP policy**</span></span>

<span data-ttu-id="722e2-116">Hvis du vil teste dataene med en innebygd eller egendefinert sensitiv informasjonstype, kan du bruke **alternativet Testtype** under **Klassifiseringer,** sensitive  >  **informasjonstyper.**</span><span class="sxs-lookup"><span data-stu-id="722e2-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="722e2-117">Hvis du vil ha mer informasjon, [kan du se Teste egendefinerte sensitive informasjonstyper.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="722e2-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="722e2-118">**Rapporter**</span><span class="sxs-lookup"><span data-stu-id="722e2-118">**Reports**</span></span>
  
- <span data-ttu-id="722e2-119">Få sensitiv datainnsikt med [DLP-rapporter.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="722e2-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="722e2-120">Se spesifikke detaljer om hendelsen med en [hendelsesrapport.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="722e2-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
