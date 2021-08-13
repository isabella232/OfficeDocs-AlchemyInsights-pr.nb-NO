---
title: Bruk alternativet for fingeravtrykksopplåsing i Windows 10
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
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971944"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Bruk alternativet for fingeravtrykksopplåsing i Windows 10

**Aktivere Windows Hello fingeravtrykk**

Hvis du Windows 10 å bruke fingeravtrykket, må du konfigurere Windows Hello fingeravtrykk ved å legge til (la Windows lære å gjenkjenne) minst én finger. 

1. Gå til **Innstillinger > kontoer > påloggingsalternativer** (eller klikk [her](ms-settings:signinoptions?activationSource=GetHelp)). Tilgjengelige påloggingsalternativer vises. For eksempel,

    ![Påloggingsalternativer.](media/sign-in-options.png)

2. Klikk eller trykk **Windows Hello fingeravtrykk**, og klikk deretter **Konfigurer**. Klikk kom i Windows Hello i **konfigurasjonsvinduet.** Fingeravtrykkssensoren aktiveres, og du blir bedt om å plassere fingeren på sensoren:

   ![Fingeravtrykkssensor.](media/fingerprint-sensor.png)

3. Følg instruksjonene, som vil be deg om å skanne fingeren gjentatte ganger. Når dette er fullført, kan du legge til andre fingre som du kanskje vil bruke til pålogging. Neste gang du logger på Windows 10, kan du bruke fingeravtrykket til å gjøre dette.

**Windows Hello Fingeravtrykk er ikke tilgjengelig som et påloggingsalternativ**

Hvis Windows Hello fingeravtrykk ikke vises som et alternativ i Påloggingsalternativer , betyr det at Windows ikke er klar over fingeravtrykksleser/skanner som er koblet til PC-en, eller at en systempolicy hindrer bruken (hvis for eksempel **PC-en** administreres av arbeidsplassen). Slik feilsøker du: 

1. Velg **Start-knappen** på oppgavelinjen, og søk etter **Enhetsbehandling**.

2. Klikk eller trykk for å åpne **Enhetsbehandling**.

3. Utvid Biometriske enheter i Enhetsbehandling ved å klikke vinkeltegn.

   ![Biometriske enheter.](media/biometric-devices.png)

4. Fingeravtrykksskanneren skal være oppført som en biometrisk enhet, for eksempel Synaptics WBDI-skanner:

   ![Biometriske enheter.](media/biometric-devices-expanded.png)

5. Hvis fingeravtrykksskanneren ikke vises, og skanneren er integrert i PC-en, går du til nettstedet til PC-produsenten. I delen for teknisk støtte for PC-modellen søker du etter en Windows 10 driver etter en skanner som du kan installere.

6. Hvis skanneren er atskilt fra PC-en (koblet til via USB), kan du gå til nettstedet til skannerprodusenten for å finne og installere Windows 10 programvare for enhetsdriveren for skannermodellen du har.
