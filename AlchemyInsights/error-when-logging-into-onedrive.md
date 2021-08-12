---
title: 0x8004de40 når du starter OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946588"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 når du starter OneDrive

Hvis du får en feilmelding **0x8004de40** logge på OneDrive, starter du datamaskinen på nytt mens du er koblet til jobb- eller skoledomenet. Hvis du får denne feilen etter omstart, kan du prøve dette mens du er koblet til jobb- eller skoledomenet:

1. Klikk Start, og skriv **inn cmd** eller **ledetekst**  i søkeboksen, høyreklikk på ledetekstappen, og velg  **Kjør som administrator**. Hvis du blir bedt om et administratorpassord eller en bekreftelse, skriver du inn passordet eller klikker **Tillat**.  

2. Skriv inn **dsregcmd /leave**  i ledetekstvinduet, og vent til kommandoen er fullført. Skriv deretter **inn dsregcmd /join,** og vent til kommandoen er fullført.
3. Start datamaskinen på nytt.
