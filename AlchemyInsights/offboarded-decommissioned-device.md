---
title: Problemer med å fjerne en avbordsenhet eller utgangsenhet fra enhetsbeholdningen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 13865acb75b60a824c1dde9427c11471e980ea9e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324453"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Problemer med å fjerne en avbordsenhet eller utgangsenhet fra enhetsbeholdningen

Microsoft Defender for endepunkt tillater for øyeblikket ikke manuelt fjerning av enhetsposten for en avbords- eller utgangsenhet fra enhetslageret.

Av sikkerhetsgrunner forblir enheten i portalen som en historisk post i opptil 180 dager. Enhetsdataene slettes imidlertid i henhold til den konfigurerte oppbevaringsperioden.

**Obs!** En avbords- eller uttrykket enhet bytter automatisk til **Inaktiv** tilstand etter sju dager. Enheter som ikke er aktive i løpet av de siste 30 dagene, er heller ikke med i dataene som gjenspeiler organisasjonens Håndtering av trusler og sikkerhetsproblemer eksponeringsresultat eller Microsoft Secure Score for Devices.
 
Hvis du fremdeles ikke vil se enkelte enheter i enhetslagervisning, kan du prøve å plassere en enhetskode for å filtrere ut enheten som er utestengt fra Enhetslager-visningen.

Hvis du vil ha mer informasjon, kan du se:

[Eksterne enheter fra Microsoft Defender for endepunkttjenesten](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Eksponeringspoengsum i Håndtering av trusler og sikkerhetsproblemer](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Løse usunne sensorer i Microsoft Defender for endepunkt](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Slik bruker du merking effektivt (del 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Slik bruker du merking effektivt (del 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Slik bruker du merking effektivt (del 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




