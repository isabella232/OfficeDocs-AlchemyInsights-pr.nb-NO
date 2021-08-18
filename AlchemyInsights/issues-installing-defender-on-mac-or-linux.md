---
title: Problemer med å installere Microsoft Defender på Mac eller Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: ae17caa4be7809b591be9f9c042186f67828aa3c36a3d17332806e4d92545dc6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898617"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problemer med å installere Microsoft Defender på Mac eller Linux

**Mac**

- Kontroller at systemkravene er oppfylt før du installerer Microsoft Defender ATP for Mac. Hvis du vil ha mer informasjon, [kan du se Slik installerer du Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Se gjennom informasjonen i filen: «/Bibliotek/Logger/Microsoft/mdatp/install.log».

**Linux**

- Kontroller at systemkravene er oppfylt før du installerer Microsoft Defender ATP for Linux. Hvis du vil ha mer informasjon, kan du [se Slik installerer du MDATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Hvis du vil bekrefte at MDATP-tjenesten kjører, kan du se [Installasjonen mislyktes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    Hvis du vil feilsøke og løse problemer hvis tjenesten ikke kjører, kan du se Fremgangsmåte for å [feilsøke hvis mdatp-tjenesten ikke kjører](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- Hvis du vil se fremgangsmåten for å kontrollere klientkonfigurasjonen, som bekrefter produktets tilstand og kjører en gjenkjenningstest på EICAR-tekstfilen, kan du se [Klientkonfigurasjon](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Obs!** Hvis du vil ha en liste over støttede filsystemer for tilgangsaktivitet, kan du se [Microsoft Defender ATP for Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)