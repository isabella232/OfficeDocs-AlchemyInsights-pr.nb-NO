---
title: Løse problemer med installasjon av DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744959"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="ea10f-102">Løse problemer med installasjon av DKIM</span><span class="sxs-lookup"><span data-stu-id="ea10f-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="ea10f-103">Hvis du får problemer med å aktivere DKIM for det egen definerte domenet, bruker du følgende Fremgangs måte:</span><span class="sxs-lookup"><span data-stu-id="ea10f-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="ea10f-104">De fleste installasjons problemene for DKIM er relatert til feil DNS-poster.</span><span class="sxs-lookup"><span data-stu-id="ea10f-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="ea10f-105">Kontroller at DKIM CNAME-posten (**ikke** en TXT-post) er riktig formatert.</span><span class="sxs-lookup"><span data-stu-id="ea10f-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="ea10f-106">Hvis du vil ha mer informasjon, kan du se dette [emnet](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="ea10f-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="ea10f-107">Når du har opprettet eller oppdatert DNS-postene for DKIM hos DNS-verten for domenet (vanligvis domene registreren), venter du til DNS-postene skal overføres.</span><span class="sxs-lookup"><span data-stu-id="ea10f-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="ea10f-108">Hvis du ikke kan opprette DKIM DNS-poster i administrasjons senteret, kan du erstatte \<CustomDomain\> med det egen definerte domenet (for eksempel contoso.com) og kjøre denne kommandoen i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="ea10f-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
