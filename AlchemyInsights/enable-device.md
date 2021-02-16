---
title: Aktiver enhet
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256874"
---
# <a name="enable-device"></a>Aktiver enhet

**Slik aktiverer du enheten ved hjelp av PowerShell-kommandoen**

Kjør følgende kommandoer:

- Slik skaffer du deg enhetsobjektet: `Get-MsolDevice -Name <Name>`
- Slik aktiverer du enheten: `Enable-MsolDevice -DeviceId <DeviceId>`

Hvis du vil ha mer informasjon om hvordan du konfigurerer hybrid sammenføyning på administrerte domener, kan du se [Konfigurere hybrid sammenføyning.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
