---
title: Intune-enhet inventar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440483"
---
# <a name="intune-device-inventory"></a>Intune-enhet inventar

Enheter-bladet gir administratorinnsikt i enheter under administrasjon i Intune per enhet. Informasjonen som vises inkluderer: Maskinvare, Oppdagede programmer, Enhetssamsvar-tilstand og Enhetskonfigurasjon.The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.

Lagerdata for maskinvare og oppdagede programmer samles inn på en syv-dagers syklus. Programmene og de spesifikke elementene i maskinvare som rapporteres varierer avhengig av enhetens operativsystem og om enheten er personlig eller bedriftseid.

Hvis du vil ha mer informasjon, kan du se [Se enhetsdetaljer i Intune](https://docs.microsoft.com/intune/device-inventory).

**SPØRSMÅL OG SVAR**

Spørsmål: Jeg mottar ikke en fullstendig lagerliste over programmer som finnes på Intune-registrerte Windows-enheter. hvorfor ikke?

Svar: For øyeblikket er bare moderne apper oppført for Windows 10-PCer som er identifisert som firmaenheter. Intune samler ikke inn informasjon om Win32-apper som er installert på disse enhetene.

Spørsmål: Hvorfor samles ikke telefonnumre fra alle enheter?

Svar: Telefoner kategorisert som firmaenheter i Intune identifiseres ikke med hele telefonnummeret når du for eksempel kjører en lagerrapport for mobilenheter. Bring-you-own-device telefonnumre er alltid delvis maskert med stjerner (****), og viser bare de fire siste sifrene.