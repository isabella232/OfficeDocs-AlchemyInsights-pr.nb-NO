---
title: Bruke alternativet for fingeravtrykksopplåsing i Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796686"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Bruke alternativet for fingeravtrykksopplåsing i Windows 10

**Aktivere Windows Hello-fingeravtrykk**

Hvis du vil låse opp Windows 10 ved hjelp av fingeravtrykk, må du konfigurere Windows Hello-fingeravtrykk ved å legge til (la Windows lære å gjenkjenne) minst én finger. 

1. Gå til **Innstillinger > kontoer > påloggingsalternativer** (eller klikk [her](ms-settings:signinoptions?activationSource=GetHelp)). Tilgjengelige påloggingsalternativer vises. For eksempel,

    ![Påloggingsalternativer.](media/sign-in-options.png)

2. Klikk eller trykk **Windows Hello Fingeravtrykk**, og klikk deretter **Konfigurer**. Klikk Kom i gang i installasjonsvinduet **for** Windows Hello. Fingeravtrykkssensoren aktiveres, og du blir bedt om å plassere fingeren på sensoren:

   ![Fingeravtrykkssensor.](media/fingerprint-sensor.png)

3. Følg instruksjonene, som vil be deg om å skanne fingeren gjentatte ganger. Når dette er fullført, kan du legge til andre fingre som du kanskje vil bruke til pålogging. Neste gang du logger på Windows 10, kan du bruke fingeravtrykket til å gjøre dette.

**Windows Hello Fingerprint er ikke tilgjengelig som et påloggingsalternativ**

Hvis Windows Hello Fingerprint ikke vises som et alternativ i Påloggingsalternativer , betyr det at Windows ikke er klar over fingeravtrykksleseren/skanneren som er koblet til PC-en, eller at en systempolicy hindrer bruken (hvis for eksempel **PC-en** administreres av arbeidsplassen). Slik feilsøker du: 

1. Velg **Start-knappen** på oppgavelinjen, og søk etter **Enhetsbehandling**.

2. Klikk eller trykk for å åpne **Enhetsbehandling**.

3. Utvid Biometriske enheter i Enhetsbehandling ved å klikke vinkeltegn.

   ![Biometriske enheter.](media/biometric-devices.png)

4. Fingeravtrykksskanneren skal være oppført som en biometrisk enhet, for eksempel Synaptics WBDI-skanner:

   ![Biometriske enheter.](media/biometric-devices-expanded.png)

5. Hvis fingeravtrykksskanneren ikke vises, og skanneren er integrert i PC-en, går du til nettstedet til PC-produsenten. Søk etter en Windows 10-driver for en skanner du kan installere, i delen teknisk støtte for PC-modellen.

6. Hvis skanneren er atskilt fra PC-en (koblet til via USB), kan du gå til nettstedet til skannerprodusenten for å finne og installere enhetsdriverprogramvaren for Windows 10 for skannermodellen du har.
