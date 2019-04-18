---
title: Løse problemer for levering av e-post til e-post fellesmapper
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910615"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="55f4d-102">Løse problemer for levering av e-post til e-post fellesmapper</span><span class="sxs-lookup"><span data-stu-id="55f4d-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="55f4d-103">Hvis eksterne avsendere ikke kan sende meldinger til din e-post fellesmapper og avsendere får feilmeldingen: **kunne ikke finne (550 5.4.1)**, kontroller e-domenet for fellesmappen er konfigurert som et domene for intern videresending i stedet for en autoritative domenet:</span><span class="sxs-lookup"><span data-stu-id="55f4d-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="55f4d-104">Åpne [administrasjonssenteret for Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="55f4d-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="55f4d-105">Gå til **e-postflyt** \> **godkjente domener**, velg det godtatte domenet, og klikk deretter **Rediger**.</span><span class="sxs-lookup"><span data-stu-id="55f4d-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="55f4d-106">I egenskapene for siden som åpnes, hvis domenetypen er satt til **Authoritative**, endrer du verdien til **intern videresending** , og klikk deretter **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="55f4d-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="55f4d-107">Hvis eksterne avsendere får feil **du ikke har tillatelse (550 5.7.13)**, kan du kjøre følgende kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) for å se hvilke tillatelser for anonyme brukere i fellesmappen:</span><span class="sxs-lookup"><span data-stu-id="55f4d-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="55f4d-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`For eksempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="55f4d-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="55f4d-109">Hvis du vil tillate at eksterne brukere å sende e-post til denne mappen, legge til CreateItems-access høyre bruker anonym.</span><span class="sxs-lookup"><span data-stu-id="55f4d-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="55f4d-110">For eksempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="55f4d-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
