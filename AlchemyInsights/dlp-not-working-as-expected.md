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
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679702"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="b80bc-102">DLP fungerer ikke som forventet</span><span class="sxs-lookup"><span data-stu-id="b80bc-102">DLP not working as expected</span></span>

<span data-ttu-id="b80bc-103">**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="b80bc-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="b80bc-104">**Konfigurere DLP**</span><span class="sxs-lookup"><span data-stu-id="b80bc-104">**Setting up DLP**</span></span>

<span data-ttu-id="b80bc-105">Har du problemer med hindring av datatap **(DLP)** i Office 365 fungerer ikke som forventet?</span><span class="sxs-lookup"><span data-stu-id="b80bc-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="b80bc-106">Hvis det er tilfelle, må du kontrollere at **DLP-policyen** er riktig konfigurert, og at dataene inneholder hva **DLP-policyen** ser ut når det evalueres.</span><span class="sxs-lookup"><span data-stu-id="b80bc-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="b80bc-107">Policyer for DLP lar deg identifisere og beskytte sensitiv informasjon i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="b80bc-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="b80bc-108">Hvis du vil konfigurere policyer for hindring av tap, kan du bruke informasjonen [her](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="b80bc-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="b80bc-109">**Hvilke DLP-policyer ser etter**</span><span class="sxs-lookup"><span data-stu-id="b80bc-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="b80bc-110">Når du bruker de **innebygde sensitive informasjons typene** i sikkerhets-og samsvars senteret, ser DLP-policyer for bestemte mønstre og elementer når de oppdager disse sensitive typene.</span><span class="sxs-lookup"><span data-stu-id="b80bc-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="b80bc-111">**Innebygde sensitive informasjons typer**</span><span class="sxs-lookup"><span data-stu-id="b80bc-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="b80bc-112">Hvis du vil ha informasjon om de innebygde sensitive typene og hva en DLP-policy ser etter når du oppdager den sensitive typen, kan du se: [hva de sensitive informasjons typene ser ut for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="b80bc-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="b80bc-113">**Egen definerte sensitive informasjons typer**</span><span class="sxs-lookup"><span data-stu-id="b80bc-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="b80bc-114">Hvis du prøver å opprette egen definerte sensitive informasjons typer, bruker du følgende artikkel for å få informasjon om hvordan du oppretter en egen definert sensitiv type: [opprette en egen definert sensitiv informasjons type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="b80bc-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="b80bc-115">**Teste en DLP-policy**</span><span class="sxs-lookup"><span data-stu-id="b80bc-115">**Test a DLP policy**</span></span>

<span data-ttu-id="b80bc-116">Hvis du vil teste dataene med en innebygd eller egen definert, sensitiv informasjons type, bruker du **test type** alternativet under **klassifiseringer**av  >  **sensitive informasjons typer**.</span><span class="sxs-lookup"><span data-stu-id="b80bc-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="b80bc-117">Hvis du vil ha mer informasjon, kan du se [teste egen definerte sensitive informasjons typer](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="b80bc-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="b80bc-118">**Rapporter**</span><span class="sxs-lookup"><span data-stu-id="b80bc-118">**Reports**</span></span>
  
- <span data-ttu-id="b80bc-119">Få sensitive data innsikt med [DLP-rapporter.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="b80bc-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="b80bc-120">Se bestemte detaljer om hendelsen med en [hendelses rapport](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="b80bc-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
