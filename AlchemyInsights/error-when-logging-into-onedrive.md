---
title: 0x8004de40-feil når du starter OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823112"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40-feil når du starter OneDrive

Hvis du får en feil melding **0x8004de40** når du logger deg på OneDrive, må du starte data maskinen på nytt mens du er koblet til jobb-eller skole domenet. Hvis du får denne feil meldingen når du starter på nytt, kan du prøve dette mens du er koblet til jobb-eller skole domenet:

1. Klikk Start, **og skriv inn** kommando **linje**  eller lede tekst i søke boksen, høyre klikk på lede tekst appen, og velg  **Kjør som administrator** . Hvis du blir bedt om å oppgi et administrator passord eller en bekreftelse, skriver du inn passordet eller klikker **Tillat** .  

2. Skriv inn **dsregcmd/Leave**  i lede tekst vinduet, og vent til kommandoen er fullført. Skriv deretter inn **dsregcmd/JOIN** , og vent til kommandoen er fullført.
3. Start data maskinen på nytt.
