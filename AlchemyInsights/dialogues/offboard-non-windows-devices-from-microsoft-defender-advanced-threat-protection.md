---
title: Offboard ikke-Windows-enheter fra Microsoft Defender Advanced Threat Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695154"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Offboard ikke-Windows-enheter fra Microsoft Defender Advanced Threat Protection (ATP)

Slik gjør du det:

1. Følg tredjepartsdokumentasjonen for å koble fra tredjepartsløsningen fra Microsoft Defender ATP.
2. Fjern tillatelser for tredjepartsløsningen fra Azure Active Directory-leieren:

    1. Logg på [Azure Portal.](https://go.microsoft.com/fwlink/?linkid=2125612)
    1. Velg **Alle tjenester** for Azure Active  >  **Directory**  >  **Enterprise-programmer.**
    1. Velg programmet du vil sette av.
    1. Velg **Slett.**

Hvis du vil ha mer informasjon, [kan du se Offboard-enheter som](https://go.microsoft.com/fwlink/?linkid=2143630)ikke bruker Windows.
