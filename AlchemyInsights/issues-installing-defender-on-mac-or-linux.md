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
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713840"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problemer med å installere Microsoft Defender på Mac eller Linux

**Mac**

- Kontroller at systemkravene er oppfylt før du installerer Microsoft Defender ATP for Mac. Hvis du vil ha mer informasjon, kan du [se Installere Microsoft Defender ATP for Mac.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Se gjennom informasjonen i filen: «/Library/Logs/Microsoft/mdatp/install.log».

**Linux**

- Kontroller at systemkravene er oppfylt før du installerer Microsoft Defender ATP for Linux. Hvis du vil ha mer informasjon, kan du [se Installere Microsoft Defender ATP for Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- Hvis du vil kontrollere at MDATP-tjenesten kjører, kan du se [Installasjonen mislyktes.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Hvis du vil feilsøke og løse problemer hvis tjenesten ikke kjører, kan du se Trinn for å feilsøke hvis [mdatp-tjenesten ikke kjører.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Hvis du vil se hvordan du kontrollerer klientkonfigurasjonen, som bekrefter produktets tilstand og kjører en gjenkjenningstest på EICAR-tekstfilen, kan du se [klientkonfigurasjonen.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)  

    **Obs!** Hvis du vil ha en liste over støttede filsystemer for on-access-aktivitet, kan du se [Microsoft Defender ATP for Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)