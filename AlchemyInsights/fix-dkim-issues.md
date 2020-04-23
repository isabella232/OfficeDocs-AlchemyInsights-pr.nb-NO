---
title: Løse problemer med DKIM-oppsett
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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717571"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="6c973-102">Løse problemer med DKIM-oppsett</span><span class="sxs-lookup"><span data-stu-id="6c973-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="6c973-103">Hvis det oppstår problemer med å aktivere DKIM for det egendefinerte domenet, bruker du følgende trinn:</span><span class="sxs-lookup"><span data-stu-id="6c973-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="6c973-104">De fleste installasjonsproblemer med DKIM er relatert til feil DNS-poster.</span><span class="sxs-lookup"><span data-stu-id="6c973-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="6c973-105">Kontroller at DKIM CNAME-posten (**ikke** en TXT-post) er riktig formatert.</span><span class="sxs-lookup"><span data-stu-id="6c973-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="6c973-106">Hvis du vil ha mer informasjon, kan du se dette [emnet](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="6c973-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="6c973-107">Når du har opprettet eller oppdatert DKIM DNS-postene dine på DNS-vertstjenesten for domenet ditt (vanligvis domeneregistratoren), venter du på at DNS-postene skal overføres.</span><span class="sxs-lookup"><span data-stu-id="6c973-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="6c973-108">Hvis du ikke kan opprette DKIM DNS-postene i \<administrasjonssenteret, kan du erstatte CustomDomain\> med det egendefinerte domenet `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`(for eksempel contoso.com) og kjøre denne kommandoen i Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): .</span><span class="sxs-lookup"><span data-stu-id="6c973-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
