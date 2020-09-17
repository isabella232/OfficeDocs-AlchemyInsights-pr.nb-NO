---
title: Oppsett-DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808716"
---
# <a name="setup-dkim"></a><span data-ttu-id="93050-102">Oppsett-DKIM</span><span class="sxs-lookup"><span data-stu-id="93050-102">Setup DKIM</span></span>

<span data-ttu-id="93050-103">De fullstendige instruksjonene for å konfigurere DKIM for egen definerte domener i Microsoft 365 er [her](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="93050-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="93050-104">For **hvert** egen definert domene må du opprette **to** DKIM CNAME-poster hos DNS-verten for domenet (vanligvis domene registreren).</span><span class="sxs-lookup"><span data-stu-id="93050-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="93050-105">Contoso.com og fourthcoffee.com krever for eksempel fire DKIM CNAME-poster: to for contoso.com og to for fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="93050-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="93050-106">DKIM CNAME-poster for **hvert** egen definert domene bruker følgende formater:</span><span class="sxs-lookup"><span data-stu-id="93050-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="93050-107">**Verts navn**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="93050-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="93050-108">**Peker til adresse eller verdi**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="93050-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="93050-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="93050-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="93050-110">**Verts navn**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="93050-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="93050-111">**Peker til adresse eller verdi**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="93050-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="93050-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="93050-112">**TTL**: 3600</span></span>

   <span data-ttu-id="93050-113">\<DomainGUID\> er teksten til venstre for den `.mail.protection.outlook.com` tilpassede MX-posten for det egen definerte domenet (for eksempel `contoso-com` for domenet contoso.com).</span><span class="sxs-lookup"><span data-stu-id="93050-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="93050-114">\<InitialDomain\> er domenet du brukte da du registrerte deg for Microsoft 365 (for eksempel contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="93050-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="93050-115">Når du har opprettet CNAME-postene for de egen definerte domenene, må du fullføre følgende instruksjoner:</span><span class="sxs-lookup"><span data-stu-id="93050-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="93050-116">a.</span><span class="sxs-lookup"><span data-stu-id="93050-116">a.</span></span> <span data-ttu-id="93050-117">[Logg på Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med jobb-eller skole kontoen.</span><span class="sxs-lookup"><span data-stu-id="93050-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="93050-118">b.</span><span class="sxs-lookup"><span data-stu-id="93050-118">b.</span></span> <span data-ttu-id="93050-119">Velg ikonet til startprogrammet for apper øverst til venstre, og velg **Administrator**.</span><span class="sxs-lookup"><span data-stu-id="93050-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="93050-120">c.</span><span class="sxs-lookup"><span data-stu-id="93050-120">c.</span></span> <span data-ttu-id="93050-121">Utvid **administrator** i nedre venstre navigasjon, og velg **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="93050-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="93050-122">d.</span><span class="sxs-lookup"><span data-stu-id="93050-122">d.</span></span> <span data-ttu-id="93050-123">Gå til **beskyttelses**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="93050-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="93050-124">e.</span><span class="sxs-lookup"><span data-stu-id="93050-124">e.</span></span> <span data-ttu-id="93050-125">Velg domenet, og velg deretter **Aktiver** for **signerings meldinger for dette domenet med DKIM-signaturer**.</span><span class="sxs-lookup"><span data-stu-id="93050-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="93050-126">Gjenta dette trinnet for hvert egen definert domene.</span><span class="sxs-lookup"><span data-stu-id="93050-126">Repeat this step for each custom domain.</span></span>
