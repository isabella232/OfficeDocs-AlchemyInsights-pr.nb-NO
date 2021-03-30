---
title: Hjelp med skjerminnstillingen for kveldslys
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404667"
---
# <a name="help-with-the-night-light-display-setting"></a>Hjelp med skjerminnstillingen for kveldslys

Hvis du vil lære mer om skjerminnstillinger for kveldstid, kan du se Angi [skjerm for kveldstid i Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).

Hvis alternativene for kveldslys er nedtonet i Innstillinger, kontrollerer du skjermdriveren: 

1. Klikk søkeboksen på oppgavelinjen, og skriv **inn Enhetsbehandling**, og velg deretter **Enhetsbehandling** i søkeresultatene.
1. Utvid **skjermkort**. 

Funksjonen for kveldslys er dessverre ikke tilgjengelig hvis enheten bruker en DisplayLink-driver eller en Grunnleggende skjermdriver.

Funksjonen for kveldslys bruker nylig grafikkteknologi, så du må kanskje oppdatere skjermdriveren:  

- Se etter oppdateringer ved å gå til **Start**  >  **innstillinger**  >  **Oppdater & Sikkerhetsoppdatering** for  >  **Windows Update**  >  **Se etter oppdateringer**.  

ELLER

- Gå til maskinvareprodusentens støttenettsted for å laste ned og installere de nyeste skjermdriverne manuelt.

## <a name="reset-night-light-in-the-registry"></a>Tilbakestille kveldslyset i registeret

Hvis oppdatering av skjermdriveren ikke fungerte, må du kanskje tilbakestille kveldslyset i registeret.  

**Forsiktig:** Dette feilsøkingstrinnet anbefales bare for avanserte brukere. Det kan oppstå alvorlige problemer hvis du endrer registeret feil. For ekstra beskyttelse bør du sikkerhetskopiere registeret før du endrer det, slik at du kan gjenopprette det hvis det oppstår problemer.

1. Skriv inn **regedit** i søkeboksen, og velg deretter **Registerredigering** i søkeresultatene.

1. Gå til følgende registernøkkel: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Eksporter og slett deretter følgende undernøkkel:$$windows.data.bluelightreduction.bluelightreductionstate

1. Eksporter og slett deretter følgende undernøkkel:$$windows.data.bluelightreduction.settings

1. Start Windows på nytt, og kontroller om alternativene for kveldslys er tilgjengelige.


