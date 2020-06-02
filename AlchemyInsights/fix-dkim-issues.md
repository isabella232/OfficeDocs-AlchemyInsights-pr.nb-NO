---
title: Løs problemer med DKIM-oppsett
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506783"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="0ce79-102">Løs problemer med DKIM-oppsett</span><span class="sxs-lookup"><span data-stu-id="0ce79-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="0ce79-103">Hvis det oppstår problemer med å aktivere DKIM for det egendefinerte domenet, bruker du følgende trinn:</span><span class="sxs-lookup"><span data-stu-id="0ce79-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="0ce79-104">De fleste problemer med DKIM-installasjoner er knyttet til feil DNS-poster.</span><span class="sxs-lookup"><span data-stu-id="0ce79-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="0ce79-105">Kontroller at DKIM CNAME-posten **(ikke** en TXT-post) er riktig formatert.</span><span class="sxs-lookup"><span data-stu-id="0ce79-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="0ce79-106">Hvis du vil ha mer informasjon, kan du se dette [emnet](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="0ce79-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="0ce79-107">Når du har opprettet eller oppdatert DKIM DNS-postene på DNS-vertstjenesten for domenet ditt (vanligvis domeneregistratoren), venter du på dns-postene for å overføre.</span><span class="sxs-lookup"><span data-stu-id="0ce79-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="0ce79-108">Hvis du ikke kan opprette DKIM DNS-postene i administrasjonssenteret, kan du erstatte \<CustomDomain\> med det egendefinerte domenet (for eksempel contoso.com) og kjøre denne kommandoen i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="0ce79-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
