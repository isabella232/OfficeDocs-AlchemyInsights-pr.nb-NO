---
title: Problemet med utskriftskøen er løst
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
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911347"
---
# <a name="print-spooler-issue-is-resolved"></a>Problemet med utskriftskøen er løst

Hvis enheten ble oppdatert med Windows 10 **OS Bygg 19041.329,** kan det hende du har observert et problem der enkelte skrivere ikke kan skrive ut.   Utskriftskøen kan føre til en feil eller lukkes uventet når du prøver å skrive ut, og ingen utdata kommer fra den berørte skriveren. Dette problemet er løst i OS-bygg **19041.331,** [KB4567523.](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)  

**Pågående undersøkelser**

LSASS-filen (Local Security Authority Subsystem Service)**(Isass.exe)** kan mislykkes på enkelte enheter med feilmeldingen «En kritisk systemprosess, C:\WINDOWS\system32\Isass.exe, mislyktes med statuskoden c0000008. Maskinen må nå startes på nytt».  **Microsoft arbeider med en løsning og vil gi en oppdatering i en kommende utgivelse.**

Hvis du vil ha mer informasjon, kan [du Windows 10 kjente problemer med versjon 2004.](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)