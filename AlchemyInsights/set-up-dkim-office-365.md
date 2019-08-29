---
title: Oppsett DKIM i Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666273"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="782b6-102">Oppsett DKIM i Office 365</span><span class="sxs-lookup"><span data-stu-id="782b6-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="782b6-103">De fullstendige instruksjonene for konfigurering av DKIM for egendefinerte domener i Office 365 er [her](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="782b6-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="782b6-104">For **hvert** egendefinerte domene må du opprette **to** DKIM CNAME Records på domenets DNS-vertstjenesten (vanligvis domeneregistratoren).</span><span class="sxs-lookup"><span data-stu-id="782b6-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="782b6-105">Contoso.com og fourthcoffee.com krever for eksempel fire DKIM CNAME-poster: to for contoso.com og to for fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="782b6-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="782b6-106">DKIM CNAME-postene for **hvert** egendefinerte domene bruker følgende formater:</span><span class="sxs-lookup"><span data-stu-id="782b6-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="782b6-107">**Vertsnavn**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="782b6-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="782b6-108">**Peker til adresse eller verdi**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="782b6-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="782b6-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="782b6-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="782b6-110">**Vertsnavn**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="782b6-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="782b6-111">**Peker til adresse eller verdi**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="782b6-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="782b6-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="782b6-112">**TTL**: 3600</span></span>

   <span data-ttu-id="782b6-113">\<DomainGUID\> er teksten til venstre for `.mail.protection.outlook.com` i den tilpassede MX-posten for det egendefinerte domenet (for eksempel `contoso-com` for domenet contoso.com).</span><span class="sxs-lookup"><span data-stu-id="782b6-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="782b6-114">\<InitialDomain\> er domenet du brukte da du registrerte deg for Office 365 (for eksempel contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="782b6-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="782b6-115">Når du har opprettet CNAME-postene for de egendefinerte domenene, fullfører du følgende instruksjoner:</span><span class="sxs-lookup"><span data-stu-id="782b6-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="782b6-116">A.</span><span class="sxs-lookup"><span data-stu-id="782b6-116">a.</span></span> <span data-ttu-id="782b6-117">[Logg på Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med jobbkonto eller skolekonto.</span><span class="sxs-lookup"><span data-stu-id="782b6-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="782b6-118">B.</span><span class="sxs-lookup"><span data-stu-id="782b6-118">b.</span></span> <span data-ttu-id="782b6-119">Velg ikonet til startprogrammet for apper øverst til venstre, og velg **Administrator**.</span><span class="sxs-lookup"><span data-stu-id="782b6-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="782b6-120">C.</span><span class="sxs-lookup"><span data-stu-id="782b6-120">c.</span></span> <span data-ttu-id="782b6-121">Utvid **administrator** i nedre venstre navigasjon, og velg **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="782b6-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="782b6-122">D.</span><span class="sxs-lookup"><span data-stu-id="782b6-122">d.</span></span> <span data-ttu-id="782b6-123">Gå til **Protection** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="782b6-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="782b6-124">E.</span><span class="sxs-lookup"><span data-stu-id="782b6-124">e.</span></span> <span data-ttu-id="782b6-125">Velg domenet, og velg deretter **Aktiver** for **Sign-meldinger for dette domenet med DKIM-signaturer**.</span><span class="sxs-lookup"><span data-stu-id="782b6-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="782b6-126">Gjenta dette trinnet for hvert egendefinerte domene.</span><span class="sxs-lookup"><span data-stu-id="782b6-126">Repeat this step for each custom domain.</span></span>
