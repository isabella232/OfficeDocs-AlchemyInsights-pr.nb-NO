---
title: Bruke alternativet for å låse opp finger i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795253"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Bruke alternativet for å låse opp finger i Windows 10

**Aktiver finger avtrykk for Windows Hello**

Hvis du vil låse opp Windows 10 ved hjelp av finger avtrykket, må du konfigurere Windows Hello-finger avtrykk ved å legge til (slik at Windows lærer å gjenkjenne) minst én finger. 

1. Gå til **innstillinger > kontoer > påloggings alternativer** (eller klikk [her](ms-settings:signinoptions?activationSource=GetHelp)). Tilgjengelige påloggings alternativer vil være oppført. Eksempel:

    ![Påloggings alternativer.](media/sign-in-options.png)

2. Klikk eller trykk **Windows Hello-fingerprint**, og klikk deretter **Konfigurer**. I vinduet Windows Hello-oppsett klikker du på **kom i gang**. Finger avtrykk sensoren vil aktivere, og du blir bedt om å plassere fingeren på sensoren:

   ![Finger avtrykk sensoren.](media/fingerprint-sensor.png)

3. Følg instruksjonene, noe som vil be deg om å skanne fingeren din gjentatte ganger. Når dette er fullført, har du muligheten til å legge til andre fingre som du kanskje vil bruke til å logge på. Neste gang du logger deg på Windows 10, kan du velge å bruke finger avtrykk til å gjøre det.

**Windows Hello-fingerprint ikke tilgjengelig som et påloggings alternativ**

Hvis Windows Hello-finger avtrykk ikke vises som et alternativ i **påloggings alternativer**, betyr det at Windows ikke er klar over finger avtrykks leser/skanner som er koblet til data maskinen, eller at en system policy hindrer bruk (Hvis for eksempel data maskinen administreres av arbeids plassen din). Slik feil søker du: 

1. Velg **Start** -knappen på oppgave linjen, og søk etter **enhets behandling**.

2. Klikk eller trykk for å åpne **enhets behandling**.

3. Utvid Biometriske enheter i enhets behandling ved å klikke vinkel tegnet.

   ![Biometriske enheter.](media/biometric-devices.png)

4. Finger avtrykks skanneren skal være oppført som en biometrisk enhet, for eksempel Synaptics WBDI-skanneren:

   ![Biometriske enheter.](media/biometric-devices-expanded.png)

5. Hvis finger avtrykks skanneren ikke vises, og skanneren er integrert i PC-en, kan du gå til PC-produsentens nettsted. Søk etter en Windows 10-driver for en skanner du kan installere, i delen teknisk støtte for din PC-modell.

6. Hvis skanneren er atskilt fra PC-en (tilknyttet via USB), kan du gå til skanner produsentens nettsted for å finne og installere Windows 10 enhets driver program vare for skanner modellen du har.
