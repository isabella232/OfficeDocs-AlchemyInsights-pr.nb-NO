---
title: DLP fungerer ikke som forventet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: efb4a19f345fe6b8a1e8bb72abeba4a923c05777
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704422"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="a2f29-102">DLP fungerer ikke som forventet</span><span class="sxs-lookup"><span data-stu-id="a2f29-102">DLP not working as expected</span></span>

<span data-ttu-id="a2f29-103">**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="a2f29-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="a2f29-104">**Sette opp DLP**</span><span class="sxs-lookup"><span data-stu-id="a2f29-104">**Setting up DLP**</span></span>

<span data-ttu-id="a2f29-105">Har du problemer med **at dlp (Data Loss Prevention)** i Office 365 ikke fungerer som forventet?</span><span class="sxs-lookup"><span data-stu-id="a2f29-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="a2f29-106">I så fall må du kontrollere at **DLP-policyen** er riktig konfigurert, og at dataene inneholder hva **DLP-policyen** leter etter når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="a2f29-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="a2f29-107">Med DLP-policyer kan du identifisere og beskytte sensitiv informasjon i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="a2f29-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="a2f29-108">Hvis du vil konfigurere DLP-policyer, bruker du informasjonen [her](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="a2f29-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="a2f29-109">**Hvilke DLP-retningslinjer ser etter**</span><span class="sxs-lookup"><span data-stu-id="a2f29-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="a2f29-110">Når du bruker de **innebygde sensitive informasjonstypene** i sikkerhets- og samsvarssentrene, ser DLP-policyer etter bestemte mønstre og elementer når du oppdager disse sensitive typene.</span><span class="sxs-lookup"><span data-stu-id="a2f29-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="a2f29-111">**Innebygde sensitive informasjonstyper**</span><span class="sxs-lookup"><span data-stu-id="a2f29-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="a2f29-112">Hvis du vil ha informasjon om de innebygde sensitive typene og hva en DLP-policy ser etter når du oppdager sensitivetypen, kan du se: [Hva de sensitive informasjonstypene ser etter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="a2f29-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="a2f29-113">**Egendefinerte sensitive informasjonstyper**</span><span class="sxs-lookup"><span data-stu-id="a2f29-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="a2f29-114">Hvis du prøver å opprette egendefinerte sensitive informasjonstyper, bruker du følgende artikkel for informasjon om hvordan du oppretter en egendefinert sensitiv type: [Opprette en egendefinert sensitiv informasjonstype](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="a2f29-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="a2f29-115">**Teste en DLP-policy**</span><span class="sxs-lookup"><span data-stu-id="a2f29-115">**Test a DLP policy**</span></span>

<span data-ttu-id="a2f29-116">Hvis du vil teste dataene med en innebygd eller egendefinert sensitiv informasjonstype, bruker du alternativet **Testtype** under **Klassifiseringer** > **Sensitive infotyper**.</span><span class="sxs-lookup"><span data-stu-id="a2f29-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="a2f29-117">Hvis du vil ha mer informasjon, kan du se [Teste egendefinerte sensitive informasjonstyper](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="a2f29-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="a2f29-118">**Rapporter**</span><span class="sxs-lookup"><span data-stu-id="a2f29-118">**Reports**</span></span>
  
- <span data-ttu-id="a2f29-119">Få sensitiv datainnsikt med [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="a2f29-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="a2f29-120">Se bestemte detaljer om hendelsen med en [hendelsesrapport](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="a2f29-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
