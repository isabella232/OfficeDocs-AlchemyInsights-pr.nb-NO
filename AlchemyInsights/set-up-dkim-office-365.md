---
title: Oppsett av DKIM i Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765275"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="55a04-102">Oppsett av DKIM i Office 365</span><span class="sxs-lookup"><span data-stu-id="55a04-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="55a04-103">Fullstendige instruksjoner for konfigurering av DKIM for egendefinerte domener i Office 365 er [her](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="55a04-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="55a04-104">For **hvert** egendefinert domene må du opprette **to** DKIM CNAME-postene på din domenets DNS-vertstjeneste (vanligvis domeneregistrar).</span><span class="sxs-lookup"><span data-stu-id="55a04-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="55a04-105">Hvis du for eksempel contoso.com og fourthcoffee.com krever fire DKIM CNAME-poster: to for contoso.com og to for fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="55a04-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="55a04-106">DKIM CNAME-postene for **hvert** egendefinert domene bruker følgende formater:</span><span class="sxs-lookup"><span data-stu-id="55a04-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="55a04-107">**Vertsnavn**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="55a04-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="55a04-108">**Peker til adressen eller verdi**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="55a04-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="55a04-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="55a04-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="55a04-110">**Vertsnavn**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="55a04-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="55a04-111">**Peker til adressen eller verdi**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="55a04-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="55a04-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="55a04-112">**TTL**: 3600</span></span>

   <span data-ttu-id="55a04-113">\<DomainGUID\> er teksten til venstre for `.mail.protection.outlook.com` i den tilpassede MX-posten for det egendefinerte domenet (for eksempel `contoso-com` for domenet contoso.com).</span><span class="sxs-lookup"><span data-stu-id="55a04-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="55a04-114">\<InitialDomain\> er domenet du brukte da du registrerte deg for Office 365 (for eksempel contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="55a04-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="55a04-115">Når du har opprettet CNAME-postene for tilpasset domene, fullfører du fremgangsmåten nedenfor:</span><span class="sxs-lookup"><span data-stu-id="55a04-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="55a04-116">en.</span><span class="sxs-lookup"><span data-stu-id="55a04-116">a.</span></span> <span data-ttu-id="55a04-117">[Logg på Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med jobbkonto eller skolekonto.</span><span class="sxs-lookup"><span data-stu-id="55a04-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="55a04-118">b.</span><span class="sxs-lookup"><span data-stu-id="55a04-118">b.</span></span> <span data-ttu-id="55a04-119">Velg ikonet til startprogrammet for apper øverst til venstre, og velg **Administrator**.</span><span class="sxs-lookup"><span data-stu-id="55a04-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="55a04-120">c.</span><span class="sxs-lookup"><span data-stu-id="55a04-120">c.</span></span> <span data-ttu-id="55a04-121">Utvid **Admin** i den nedre, venstre navigasjonen og velge **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="55a04-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="55a04-122">d.</span><span class="sxs-lookup"><span data-stu-id="55a04-122">d.</span></span> <span data-ttu-id="55a04-123">Gå til **beskyttelse mot** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="55a04-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="55a04-124">e.</span><span class="sxs-lookup"><span data-stu-id="55a04-124">e.</span></span> <span data-ttu-id="55a04-125">Velg domenet, og velg deretter **Aktiver** for **Logg meldinger for dette domenet med DKIM-signaturer**.</span><span class="sxs-lookup"><span data-stu-id="55a04-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="55a04-126">Gjenta dette trinnet for hvert egendefinert domene.</span><span class="sxs-lookup"><span data-stu-id="55a04-126">Repeat this step for each custom domain.</span></span>
