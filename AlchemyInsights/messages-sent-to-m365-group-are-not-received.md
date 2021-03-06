---
title: Meldinger som sendes til Microsoft 365-gruppen, blir ikke mottatt av alle medlemmer
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 080c060f5675065704c7209bd15e4cbb1236b8db
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480692"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="2e198-102">Meldinger som sendes til en Microsoft 365-gruppe, blir ikke mottatt av alle medlemmer</span><span class="sxs-lookup"><span data-stu-id="2e198-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="2e198-103">Kontroller at alle medlemmene i gruppen har abonnert på å motta e-postmeldinger.</span><span class="sxs-lookup"><span data-stu-id="2e198-103">Ensure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="2e198-104">Se [Følg en gruppe i Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="2e198-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="2e198-105">Hvis du vil kontrollere meldingsstatusen for medlemmer som abonnerer på e-postmeldinger for gruppen, kjører du følgende kommando på [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span><span class="sxs-lookup"><span data-stu-id="2e198-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

<span data-ttu-id="2e198-106">Bruk følgende EXO PowerShell-kommando for å konfigurere alle gruppemedlemmene til å motta e-postmeldinger, som sendes til Microsoft 365-gruppen i innboksen:</span><span class="sxs-lookup"><span data-stu-id="2e198-106">Use the following EXO PowerShell command to configure all group members to receive emails sent to Microsoft 365 group in their inbox:</span></span>

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

<span data-ttu-id="2e198-107">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="2e198-107">For example:</span></span>

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`