---
title: Oppsett DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509393"
---
# <a name="setup-dkim"></a><span data-ttu-id="7e034-102">Oppsett DKIM</span><span class="sxs-lookup"><span data-stu-id="7e034-102">Setup DKIM</span></span>

<span data-ttu-id="7e034-103">De fullstendige instruksjonene for å konfigurere DKIM for egendefinerte domener i Microsoft 365 er [her](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="7e034-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="7e034-104">For **hvert** egendefinerte domene må du opprette **to** DKIM CNAME-poster på domenets DNS-vertstjeneste (vanligvis domeneregistratoren).</span><span class="sxs-lookup"><span data-stu-id="7e034-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="7e034-105">contoso.com og fourthcoffee.com krever for eksempel fire DKIM CNAME-poster: to for contoso.com og to for fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="7e034-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="7e034-106">DKIM CNAME-postene for **hvert** egendefinerte domene bruker følgende formater:</span><span class="sxs-lookup"><span data-stu-id="7e034-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="7e034-107">**Vertsnavn**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="7e034-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="7e034-108">**Peker til adresse eller verdi:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="7e034-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="7e034-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="7e034-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="7e034-110">**Vertsnavn**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="7e034-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="7e034-111">**Peker til adresse eller verdi:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="7e034-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="7e034-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="7e034-112">**TTL**: 3600</span></span>

   <span data-ttu-id="7e034-113">\<DomainGUID\>er teksten til venstre `.mail.protection.outlook.com` for i den tilpassede MX-posten for det egendefinerte domenet (for eksempel for domenet `contoso-com` contoso.com).</span><span class="sxs-lookup"><span data-stu-id="7e034-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="7e034-114">\<InitialDomain\>er domenet du brukte da du registrerte deg for Microsoft 365 (for eksempel contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="7e034-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="7e034-115">Når du har opprettet CNAME-postene for de egendefinerte domenene, fullfører du følgende instruksjoner:</span><span class="sxs-lookup"><span data-stu-id="7e034-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="7e034-116">a.</span><span class="sxs-lookup"><span data-stu-id="7e034-116">a.</span></span> <span data-ttu-id="7e034-117">[logg på Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med jobb- eller skolekontoen.</span><span class="sxs-lookup"><span data-stu-id="7e034-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="7e034-118">b.</span><span class="sxs-lookup"><span data-stu-id="7e034-118">b.</span></span> <span data-ttu-id="7e034-119">Velg ikonet til startprogrammet for apper øverst til venstre, og velg **Administrator**.</span><span class="sxs-lookup"><span data-stu-id="7e034-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="7e034-120">c.</span><span class="sxs-lookup"><span data-stu-id="7e034-120">c.</span></span> <span data-ttu-id="7e034-121">Utvid **Administrator** i navigasjonen nederst til venstre, og velg **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="7e034-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="7e034-122">D.</span><span class="sxs-lookup"><span data-stu-id="7e034-122">d.</span></span> <span data-ttu-id="7e034-123">Gå til **Beskyttelse**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="7e034-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="7e034-124">E.</span><span class="sxs-lookup"><span data-stu-id="7e034-124">e.</span></span> <span data-ttu-id="7e034-125">Velg domenet, og velg deretter **Aktiver** for **Signer-meldinger for dette domenet med DKIM-signaturer**.</span><span class="sxs-lookup"><span data-stu-id="7e034-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="7e034-126">Gjenta dette trinnet for hvert egendefinerte domene.</span><span class="sxs-lookup"><span data-stu-id="7e034-126">Repeat this step for each custom domain.</span></span>
