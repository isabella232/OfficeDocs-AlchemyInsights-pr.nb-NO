---
title: Enhets beholdning for Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667887"
---
# <a name="intune-device-inventory"></a>Enhets beholdning for Intune

Enheter-bladserveren gir administrator innsikt i enheter under administrasjon i Intune på per enhets basis. Informasjonen som vises, omfatter: maskin vare, oppdagede programmer, enhets Samsvars tilstand og enhets konfigurasjons tilstand.

Lager data for maskin vare og oppdagede programmer samles inn på en sju dagers syklus. Programmer og bestemte elementer med maskin vare som er rapportert, varierer avhengig av enhetens operativ system og om enheten er personlig eller bedrifts eid.

Hvis du vil ha mer informasjon, kan du se [se enhets detaljer i Intune](https://docs.microsoft.com/intune/device-inventory).

**SPØRSMÅL OG SVAR**

Spørsmål: jeg mottar ikke en fullstendig innholds liste over programmer som finnes på Intune-registrerte Windows-enheter. hvorfor ikke?

A: for øyeblikket er det bare moderne apper som er oppført for Windows 10-PC-er som er identifisert som firma enheter. Intune samler ikke inn informasjon om Win32-apper som er installert på disse enhetene.

Spørsmål: Hvorfor blir ikke telefon numre samlet inn fra alle enheter?

A: telefoner som er kategorisert som firma enheter i Intune, er ikke identifisert med sitt fulle telefon nummer når du for eksempel kjører en rapport om en mobil enhets beholdning. Mobil telefon numre for enheter er alltid delvis maskert med stjerner (* * * *), og viser bare de fire siste sifrene.