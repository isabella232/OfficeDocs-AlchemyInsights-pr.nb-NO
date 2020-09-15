---
title: Problem med utskrifts køen er løst
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801850"
---
# <a name="print-spooler-issue-is-resolved"></a>Problem med utskrifts køen er løst

Hvis enheten ble oppdatert med Windows 10  **OS bygg 19041,329**, kan du ha observert et problem der visse skrivere ikke kunne skrives ut. Utskrifts køen kan kanskje iverksette en feil eller lukkes uventet når du prøver å skrive ut, og ingen utdata kommer fra den berørte skrive ren. Dette problemet er løst i OS Build  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Pågående undersøkelse**

LSASS-filen (Local Security Authority Subsystem Service) (**Isass.exe**) kan mislykkes på enkelte enheter med feil meldingen «en kritisk system prosess, C:\WINDOWS\system32\Isass.exe, mislyktes med status kode c0000008. Maskinen må nå startes på nytt.  **Microsoft arbeider med en løsning og vil gi en oppdatering i en kommende utgivelse.**

Hvis du vil ha mer informasjon, kan du se  [kjente problemer med Windows 10 versjon 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).