---
title: Slik aktiverer du driftet telefonsvarer
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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055563"
---
# <a name="how-to-enable-hosted-voicemail"></a>Slik aktiverer du driftet telefonsvarer

Hvis du vil aktivere Talepost, **må HostedVoicemail** være satt til $true.

**HostedVoicemail-egenskapen** for brukeren som bruker Ekstern PowerShell (RPS).

Hvis du vil ha mer informasjon om hvordan du kobler til RPS, [kan du Microsoft Teams PowerShell-oversikt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) hvis du vil ha mer informasjon om hvordan du kobler til RPS.

1. Administratoren Teams være logget på Ekstern PowerShell for Teams.
1. Fra PowerShell spør Teams administratoren kan kjøre **set-csuser user@contoso.com -HostedVoiceMail $true** der sip uri er av den aktuelle brukeren.

> [!NOTE]
> Endringer i policyer kan ta opptil 24 timer å replikere.