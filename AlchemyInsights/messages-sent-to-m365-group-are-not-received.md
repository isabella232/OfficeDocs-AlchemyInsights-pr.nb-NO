---
title: Meldinger som sendes til Microsoft 365-gruppen, mottas ikke av alle medlemmer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/06/2020
ms.locfileid: "45051503"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Meldinger som sendes til en Microsoft 365-gruppe, mottas ikke av alle medlemmer

Sørg for at alle gruppemedlemmene har abonnert på å motta e-postene. Se [Følge en gruppe i Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Hvis du vil kontrollere meldingsstatusen for medlemmer som har abonnert på gruppe-e-post, kjører du følgende kommando på [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`