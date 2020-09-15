---
title: Teams 4c7-feil
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700212"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-feil i Microsoft Teams

Denne feilen oppstår fordi Microsoft Teams krever skjema godkjenning. Når du distribuerer Active Directory Federation Services (AD FS), aktiveres ikke skjema godkjenning for intranett som standard. Hvis det oppstår feil i Windows-integrert godkjenning, blir du bedt om å logge på ved hjelp av skjema godkjenning.

Hvis du vil løse dette problemet, kan du aktivere skjema godkjenning ved hjelp av AD FS-snapin-modulen for Microsoft Management Console (MMC) på data maskinen som har den lokale kopien av Active Directory. Dette gjør du slik: 

1. Gå til **godkjennings policyer**i navigasjons ruten.
2. Velg **Rediger global primær godkjenning**under **handlinger** i Detaljer-ruten.
3. Velg **skjema godkjenning**på fanen **intranett** .
4. Velg **OK** (eller **Bruk**).