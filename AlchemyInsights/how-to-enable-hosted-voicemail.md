---
title: Slik aktiverer du telefoni, talepost
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679159"
---
# <a name="how-to-enable-hosted-voicemail"></a>Slik aktiverer du telefoni, talepost

Hvis du vil aktivere talepost, må **HostedVoicemail** være satt til $True.

**HostedVoicemail** -egenskapen for brukeren som bruker Remote POWERSHELL (RPS).

Hvis du vil ha mer informasjon om å koble til RPS, kan du se [Microsoft Teams PowerShell-oversikt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for mer informasjon om å koble til RPS.

1. Teams-administratoren bør være logget på Remote PowerShell for Teams.
1. Fra PowerShell-lede tekst team administrator kan kjøre **Set-csuser User@contoso.com-HostedVoiceMail $True** der SIP-URIen er for den aktuelle brukeren.

> [!NOTE]
> Endringer i policyer kan ha opptil 24 timer å replisere.