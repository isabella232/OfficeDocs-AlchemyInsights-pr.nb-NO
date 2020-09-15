---
title: Løse problemer med levering av e-post til e-postaktiverte felles mapper
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677937"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="7e841-102">Løse problemer med levering av e-post til e-postaktiverte felles mapper</span><span class="sxs-lookup"><span data-stu-id="7e841-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="7e841-103">Hvis eksterne avsendere ikke kan sende meldinger til de e-postaktiverte felles mappene, og avsenderne får feil meldingen: **ble ikke funnet (550 5.4.1)**, må du kontrollere at e-postdomenene for felles mappen er konfigurert som et internt Relay-domene i stedet for et autoritativt domene:</span><span class="sxs-lookup"><span data-stu-id="7e841-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="7e841-104">Åpne [administrasjons senteret for Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="7e841-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="7e841-105">Gå til **e-postflyt** \> **godkjente domener**, Velg godkjent domene, og klikk deretter **Rediger**.</span><span class="sxs-lookup"><span data-stu-id="7e841-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="7e841-106">På Egenskaper-siden som åpnes, hvis domene typen er satt til **autoritativ**, endrer du verdien til **intern videre sending** og klikker deretter **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="7e841-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="7e841-107">Hvis eksterne avsendere får feilen **du ikke har tilgang til (550 5.7.13)**, kjører du følgende kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) for å se tillatelsene for anonyme brukere i felles mappen:</span><span class="sxs-lookup"><span data-stu-id="7e841-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="7e841-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For eksempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="7e841-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="7e841-109">Hvis du vil tillate at eksterne brukere sender e-post til denne felles mappen, kan du legge til CreateItems Access-tilgang direkte i den anonyme brukeren.</span><span class="sxs-lookup"><span data-stu-id="7e841-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="7e841-110">For eksempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="7e841-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
