---
title: Arkivpostboksen er nesten full
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046761"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Arkivpostboksen er nesten full

Hvis brukeren mottar advarselen; **Arkivpostboksen er nesten full,** eller du må øke størrelsen på arkivpostboksen, her er noen tips:

1. Hvis brukeren er tilordnet en Exchange Online Plan 1, oppgraderer du til Exchange Online **Plan 2-lisensen** for å øke størrelsen fra 50 GB til 100 GB.
1. Hvis brukeren allerede er tilordnet ett av følgende: **Exchange Online Plan 2** eller en Exchange Online Plan 1 med et Exchange Online Archiving-tillegg, bruker du fremgangsmåten nedenfor for å aktivere arkivering av automatisk utvidelse:.
 
    1. [Koble til å Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Kjør følgende kommandolet for brukeren:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Kjør følgende kommandolet for å bekrefte at den er aktivert for brukeren:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Hvis du vil ha mer informasjon, kan du se:

- [Aktivere ubegrenset arkivering – hjelp for administratorer – Microsoft 365 samsvars | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online grenser – Tjenestebeskrivelser | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Oppgrader til en annen forretningsplan | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

