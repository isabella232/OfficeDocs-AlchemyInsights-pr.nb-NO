---
title: Send som Microsoft 365-gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872000"
---
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="c0b63-102">Send som Microsoft 365-gruppe</span><span class="sxs-lookup"><span data-stu-id="c0b63-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="c0b63-103">Du kan tilordne Send som-tillatelser slik at bestemte brukere kan sende meldinger som en Microsoft 365-gruppe:</span><span class="sxs-lookup"><span data-stu-id="c0b63-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="c0b63-104">Koble til Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c0b63-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="c0b63-105">Kjør følgende kommando:</span><span class="sxs-lookup"><span data-stu-id="c0b63-105">Run the following command:</span></span>  

    <span data-ttu-id="c0b63-106">Legg til RecipientPermission- `<GroupName>` trustee `<MailboxName>` -AccessRights SendAs</span><span class="sxs-lookup"><span data-stu-id="c0b63-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="c0b63-107">Hvis du vil ha mer informasjon, kan du se [tillate at medlemmer sender som eller sender på vegne av en gruppe](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="c0b63-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>