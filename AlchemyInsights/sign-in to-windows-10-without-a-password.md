---
title: Logg på Windows 10 uten å bruke et passord
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
- "9001690"
- "3766"
ms.openlocfilehash: fbf190d433eabfee5b45348d05d918222a385314a431812aa5f5926aacf11560
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107528"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Logg på Windows 10 uten å bruke et passord

Hvis du vil unngå å måtte skrive inn et passord ved Windows oppstart, anbefaler vi at du bruker et av de Windows Hello sikre påloggingsalternativene, for eksempel en PIN-kode, ansiktsgjenkjenning eller fingeravtrykk, hvis tilgjengelig. Hvis du virkelig vil deaktivere sikker pålogging, kan du se instruksjonene «Logg på Windows 10» nedenfor.

**Sikre Windows Hello alternativer til kontopassordet**

Gå til **Innstillinger > kontoer > påloggingsalternativer** (eller klikk [her](ms-settings:signinoptions?activationSource=GetHelp)). Tilgjengelige påloggingsalternativer vises. For eksempel,

![Påloggingsalternativer.](media/sign-in-options.png)

Klikk eller trykk ett av alternativene for å konfigurere det. Neste gang du starter eller låser Windows, kan du bruke det nye alternativet i stedet for et passord. 

**Logg på automatisk for å Windows 10**

**Obs!** Automatisk pålogging er praktisk, men medfører en sikkerhetsrisiko, spesielt hvis PC-en er tilgjengelig for flere personer. 

1. Klikk eller trykk **Start-knappen** på oppgavelinjen.

2. Skriv **inn netplwiz,** og trykk ENTER for å åpne Brukerkontoer-vinduet.

3. I **Brukerkontoer** klikker du kontoen du vil logge på automatisk når Windows starter.

4. Fjern merket for Brukere må angi brukernavn og passord for å bruke denne datamaskinen.

    ![Brukere må angi et brukernavn- og passordalternativ.](media/users-must-enter-username.png)

5. Klikk **OK**. Du blir bedt om å angi og bekrefte passordet for kontoen du valgte. Klikk **OK for** å fullføre. Neste Windows 10 starter, logges den automatisk på kontoen du valgte.
