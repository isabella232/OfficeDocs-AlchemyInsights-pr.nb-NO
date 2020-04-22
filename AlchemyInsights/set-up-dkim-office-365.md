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
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645681"
---
# <a name="setup-dkim"></a><span data-ttu-id="4f8c0-102">Oppsett DKIM</span><span class="sxs-lookup"><span data-stu-id="4f8c0-102">Setup DKIM</span></span>

<span data-ttu-id="4f8c0-103">De fullstendige instruksjonene for å konfigurere DKIM for egendefinerte domener i Microsoft 365 er [her](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="4f8c0-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="4f8c0-104">For **hvert** egendefinerte domene må du opprette **to** DKIM CNAME-poster på domenets DNS-vertstjeneste (vanligvis domeneregistratoren).</span><span class="sxs-lookup"><span data-stu-id="4f8c0-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="4f8c0-105">Contoso.com og fourthcoffee.com krever for eksempel fire DKIM CNAME-poster: to for contoso.com og to for fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="4f8c0-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="4f8c0-106">DKIM CNAME-postene for **hvert** egendefinerte domene bruker følgende formater:</span><span class="sxs-lookup"><span data-stu-id="4f8c0-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="4f8c0-107">**Vertsnavn**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="4f8c0-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="4f8c0-108">**Peker til adresse eller verdi**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="4f8c0-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="4f8c0-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="4f8c0-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="4f8c0-110">**Vertsnavn**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="4f8c0-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="4f8c0-111">**Peker til adresse eller verdi**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="4f8c0-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="4f8c0-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="4f8c0-112">**TTL**: 3600</span></span>

   <span data-ttu-id="4f8c0-113">\<DomainGUID\> er teksten til `.mail.protection.outlook.com` venstre for i den tilpassede MX-posten `contoso-com` for det egendefinerte domenet (for eksempel for domenet contoso.com).</span><span class="sxs-lookup"><span data-stu-id="4f8c0-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="4f8c0-114">\<InitialDomain\> er domenet du brukte da du registrerte deg for Microsoft 365 (for eksempel contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="4f8c0-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="4f8c0-115">Når du har opprettet CNAME-postene for de egendefinerte domenene, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="4f8c0-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="4f8c0-116">A.</span><span class="sxs-lookup"><span data-stu-id="4f8c0-116">a.</span></span> <span data-ttu-id="4f8c0-117">[logg på Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med jobb- eller skolekontoen.</span><span class="sxs-lookup"><span data-stu-id="4f8c0-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="4f8c0-118">B.</span><span class="sxs-lookup"><span data-stu-id="4f8c0-118">b.</span></span> <span data-ttu-id="4f8c0-119">Velg ikonet til startprogrammet for apper øverst til venstre, og velg **Administrator**.</span><span class="sxs-lookup"><span data-stu-id="4f8c0-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="4f8c0-120">C.</span><span class="sxs-lookup"><span data-stu-id="4f8c0-120">c.</span></span> <span data-ttu-id="4f8c0-121">Utvid **Administrator** i navigasjonen nederst til venstre, og velg **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="4f8c0-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="4f8c0-122">D.</span><span class="sxs-lookup"><span data-stu-id="4f8c0-122">d.</span></span> <span data-ttu-id="4f8c0-123">Gå til **Beskyttelse** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="4f8c0-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="4f8c0-124">E.</span><span class="sxs-lookup"><span data-stu-id="4f8c0-124">e.</span></span> <span data-ttu-id="4f8c0-125">Velg domenet, og velg deretter **Aktiver** for **Sign-meldinger for dette domenet med DKIM-signaturer**.</span><span class="sxs-lookup"><span data-stu-id="4f8c0-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="4f8c0-126">Gjenta dette trinnet for hvert egendefinerte domene.</span><span class="sxs-lookup"><span data-stu-id="4f8c0-126">Repeat this step for each custom domain.</span></span>
