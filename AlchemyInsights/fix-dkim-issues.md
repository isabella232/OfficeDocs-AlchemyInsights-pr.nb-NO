---
title: Løse problemer med installasjonsprogrammet DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765263"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="68b33-102">Løse problemer med installasjonsprogrammet DKIM</span><span class="sxs-lookup"><span data-stu-id="68b33-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="68b33-103">Hvis du opplever problemer med å aktivere DKIM for det tilpassede domenet, kan du bruke følgende fremgangsmåte:</span><span class="sxs-lookup"><span data-stu-id="68b33-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="68b33-104">De fleste DKIM-installasjonsproblemer knyttet til feil DNS-poster.</span><span class="sxs-lookup"><span data-stu-id="68b33-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="68b33-105">Kontroller DKIM CNAME-post (**ikke** en TXT-post) er riktig formatert.</span><span class="sxs-lookup"><span data-stu-id="68b33-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="68b33-106">Hvis du vil ha mer informasjon, se dette [emnet](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="68b33-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="68b33-107">Når du oppretter eller oppdaterer DKIM DNS-postene i DNS-vertstjenesten for domenet (vanligvis domeneregistraren din), venter på DNS-poster å overføre.</span><span class="sxs-lookup"><span data-stu-id="68b33-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="68b33-108">Hvis du ikke kan opprette DKIM DNS oppføringer i administrasjonssenteret, kan du erstatte \<CustomDomain\> med det tilpassede domenet (for eksempel contoso.com) og kjøre denne kommandoen i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="68b33-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
