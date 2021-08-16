---
title: Teams 4c7-feil
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049317"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-feil i Microsoft Teams

Denne feilen oppstår fordi Microsoft Teams krever skjemagodkjenning. Når du distribuerer Active Directory Federation Services (AD FS), er skjemagodkjenning ikke aktivert for intranettet som standard. Hvis Windows integrert godkjenning mislykkes, blir du bedt om å logge på ved hjelp av Skjemagodkjenning.

Du kan løse dette problemet ved å aktivere Skjemagodkjenning ved hjelp av snapin-modulen AD FS Microsoft Management Console (MMC) på datamaskinen som har den lokale kopien av Active Directory. Dette gjør du slik: 

1. Bla til Godkjenningspolicyer i **navigasjonsruten.**
2. Velg **Rediger** global primær godkjenning under Handlinger i **detaljruten.**
3. Velg Skjemagodkjenning på **Intranett-fanen.** 
4. Velg **OK** (eller **Bruk**).