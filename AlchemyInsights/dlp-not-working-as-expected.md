---
title: DLP fungerer ikke som forventet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/08/2020
ms.locfileid: "42977447"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="14fdf-102">DLP fungerer ikke som forventet</span><span class="sxs-lookup"><span data-stu-id="14fdf-102">DLP not working as expected</span></span>

<span data-ttu-id="14fdf-103">**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="14fdf-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="14fdf-104">**Sette opp DLP**</span><span class="sxs-lookup"><span data-stu-id="14fdf-104">**Setting up DLP**</span></span>

<span data-ttu-id="14fdf-105">Har du problemer med **at dlp (Data Loss Prevention)** i Office 365 ikke fungerer som forventet?</span><span class="sxs-lookup"><span data-stu-id="14fdf-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="14fdf-106">I så fall må du kontrollere at **DLP-policyen** er riktig konfigurert, og at dataene inneholder hva **DLP-policyen** leter etter når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="14fdf-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="14fdf-107">Med DLP-policyer kan du identifisere og beskytte sensitiv informasjon i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="14fdf-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="14fdf-108">Hvis du vil konfigurere DLP-policyer, bruker du informasjonen [her](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="14fdf-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="14fdf-109">**Hvilke DLP-retningslinjer ser etter**</span><span class="sxs-lookup"><span data-stu-id="14fdf-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="14fdf-110">Når du bruker de **innebygde sensitive informasjonstypene** i Office 365 sikkerhets- og samsvarssenter, ser DLP-policyer etter bestemte mønstre og elementer når du oppdager disse sensitive typene.</span><span class="sxs-lookup"><span data-stu-id="14fdf-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="14fdf-111">**Innebygde sensitive informasjonstyper**</span><span class="sxs-lookup"><span data-stu-id="14fdf-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="14fdf-112">Hvis du vil ha informasjon om de innebygde sensitive typene og hva en DLP-policy ser etter når du oppdager sensitivetypen, kan du se: [Hva de sensitive informasjonstypene ser etter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="14fdf-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="14fdf-113">**Egendefinerte sensitive informasjonstyper**</span><span class="sxs-lookup"><span data-stu-id="14fdf-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="14fdf-114">Hvis du prøver å opprette egendefinerte sensitive informasjonstyper, bruker du følgende artikkel for informasjon om hvordan du oppretter en egendefinert sensitiv type: [Opprette en egendefinert sensitiv informasjonstype](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="14fdf-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="14fdf-115">**Teste en DLP-policy**</span><span class="sxs-lookup"><span data-stu-id="14fdf-115">**Test a DLP policy**</span></span>

<span data-ttu-id="14fdf-116">Hvis du vil teste dataene med en innebygd eller egendefinert sensitiv informasjonstype, bruker du alternativet **Testtype** under **Klassifiseringer** > **Sensitive infotyper**.</span><span class="sxs-lookup"><span data-stu-id="14fdf-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="14fdf-117">Hvis du vil ha mer informasjon, kan du se [Teste egendefinerte sensitive informasjonstyper](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="14fdf-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="14fdf-118">**Rapporter**</span><span class="sxs-lookup"><span data-stu-id="14fdf-118">**Reports**</span></span>
  
- <span data-ttu-id="14fdf-119">Få sensitiv datainnsikt med [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="14fdf-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="14fdf-120">Se bestemte detaljer om hendelsen med en [hendelsesrapport](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="14fdf-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
