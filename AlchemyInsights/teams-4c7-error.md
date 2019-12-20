---
title: Teams 4c 7-feil
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796264"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c 7 feil i Microsoft Teams

Denne feilen oppstår fordi Microsoft Teams krever skjemagodkjenning. Når du distribuerer Active Directory Federation Services (AD FS), aktiveres ikke skjemagodkjenning for intranettet som standard. Hvis Windows-integrert godkjenning mislykkes, blir du bedt om å logge på ved hjelp av skjemagodkjenning.

Hvis du vil løse dette problemet, kan du aktivere skjemagodkjenning ved hjelp av snapin-modul for AD FS Microsoft Management Console (MMC) på datamaskinen som har den lokale kopien av Active Directory. Hvis du vil gjøre dette, følger du denne fremgangsmåten: 

1. I navigasjonsruten blar du til **godkjennings policyer**.
2. Velg **Rediger global primær godkjenning**under **handlinger** i detaljruten.
3. Velg **skjemagodkjenning**i kategorien **intranett** .
4. Velg **OK** (eller **Bruk**).