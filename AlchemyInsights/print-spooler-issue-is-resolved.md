---
title: Problemet med utskriftskøen er løst
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088402"
---
# <a name="print-spooler-issue-is-resolved"></a>Problemet med utskriftskøen er løst

Hvis enheten ble oppdatert med Windows 10 **OS Build 19041.329**, kan det hende du har observert et problem der enkelte skrivere ikke kan skrive ut. Utskriftskøen kan kaste en feil eller lukke uventet når du prøver å skrive ut, og ingen utskrift kommer fra den berørte skriveren. Dette problemet er løst i OS Build **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Pågående etterforskning**

Den lokale security authority delsystem service (LSASS) filen** (Isass.exe**) kan mislykkes på enkelte enheter med feilmeldingen "En kritisk systemprosess, C:\WINDOWS\system32\Isass.exe, mislyktes med statuskode c0000008. Maskinen må nå startes på nytt".  **Microsoft arbeider med en løsning og vil gi en oppdatering i en kommende utgivelse.**

Hvis du vil ha mer informasjon, kan du sjekke ut [kjente problemer med Windows 10 versjon 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).