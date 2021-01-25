---
title: Arkiv post boksen er nesten full
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974409"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Arkiv post boksen er nesten full

Hvis brukeren mottar advarselen, **Arkiv post boksen er nesten full**, eller du må øke størrelsen på arkiv post boksen, her er noen tips:

1. Hvis brukeren er tilordnet en Exchange Online-plan 1, oppgraderer du til **Exchange Online plan 2** -lisensen for å øke størrelsen fra 50 GB til 100 GB.
1. Hvis brukeren allerede er tilordnet ett av følgende: **Exchange Online plan 2** eller en Exchange Online-plan 1 med et Exchange Online arkiverings tillegg, bruker du Fremgangs måten nedenfor for å aktivere automatisk justering av arkivering:.
 
    1. [Koble til Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Kjør følgende unifiedgroup for brukeren:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Kjør følgende unifiedgroup for å bekrefte at den er aktivert for brukeren:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Hvis du vil ha mer informasjon, se:

- [ Aktiver ubegrenset arkivering – hjelp for administratorer – samsvar med Microsoft 365 | Microsoft-dokumenter](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Begrensninger på Exchange Online – tjeneste beskrivelser | Microsoft-dokumenter](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Oppgrader til en annen forretnings plan | Microsoft-dokumenter](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

