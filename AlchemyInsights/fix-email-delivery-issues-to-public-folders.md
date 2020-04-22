---
title: Løse problemer med e-postlevering til e-postaktiverte fellesmapper
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716361"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="dc8c3-102">Løse problemer med e-postlevering til e-postaktiverte fellesmapper</span><span class="sxs-lookup"><span data-stu-id="dc8c3-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="dc8c3-103">Hvis eksterne avsendere ikke kan sende meldinger til de e-postaktiverte fellesmappene, og avsenderne får feilmeldingen: **Finner ikke feilen (550 5.4.1),** må du kontrollere at e-postdomenet for fellesmappen er konfigurert som et internt relédomene i stedet for et autoritativt domene:</span><span class="sxs-lookup"><span data-stu-id="dc8c3-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="dc8c3-104">Åpne [administrasjonssenteret for Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="dc8c3-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="dc8c3-105">Gå til **E-postflyt** \> **Godtatt e-postdomener**, velg det godtatte domenet, og klikk deretter **Rediger**.</span><span class="sxs-lookup"><span data-stu-id="dc8c3-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="dc8c3-106">Hvis domenetypen er satt til **Autoritativ**på egenskapssiden som åpnes, endrer du verdien til **Intern relé** på egenskapssiden som åpnes, og deretter klikker du **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="dc8c3-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="dc8c3-107">Hvis eksterne avsendere får feilmeldingen **du ikke har tillatelse (550 5.7.13),** kjører du følgende kommando i Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) for å se tillatelsene for anonyme brukere i fellesmappen:</span><span class="sxs-lookup"><span data-stu-id="dc8c3-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="dc8c3-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`For eksempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`. .</span><span class="sxs-lookup"><span data-stu-id="dc8c3-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="dc8c3-109">Hvis du vil tillate eksterne brukere å sende e-post til denne fellesmappen, legger du til Rettigheten CreateItems-tilgang til brukeren Anonym.</span><span class="sxs-lookup"><span data-stu-id="dc8c3-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="dc8c3-110">For eksempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`. .</span><span class="sxs-lookup"><span data-stu-id="dc8c3-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
