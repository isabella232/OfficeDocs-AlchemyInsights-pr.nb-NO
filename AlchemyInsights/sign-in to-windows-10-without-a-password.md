---
title: Logge på Windows 10 uten å bruke et passord
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
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830555"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Logge på Windows 10 uten å bruke et passord

Hvis du vil unngå å måtte skrive inn et passord ved oppstart av Windows, anbefaler vi at du bruker et av de sikre påloggingsalternativene for Windows Hello, for eksempel en PIN-kode, ansiktsgjenkjenning eller fingeravtrykk, hvis tilgjengelig. Hvis du virkelig vil deaktivere sikker pålogging, kan du se instruksjonene «Logg på Windows 10 automatisk» nedenfor.

**Sikre Windows Hello-alternativer til kontopassordet**

Gå til **Innstillinger > kontoer > påloggingsalternativer** (eller klikk [her](ms-settings:signinoptions?activationSource=GetHelp)). Tilgjengelige påloggingsalternativer vises. For eksempel,

![Påloggingsalternativer.](media/sign-in-options.png)

Klikk eller trykk ett av alternativene for å konfigurere det. Neste gang du starter eller låser opp Windows, kan du bruke det nye alternativet i stedet for et passord. 

**Logge på Windows 10 automatisk**

**Obs!** Automatisk pålogging er praktisk, men medfører en sikkerhetsrisiko, spesielt hvis PC-en er tilgjengelig for flere personer. 

1. Klikk eller trykk **Start-knappen** på oppgavelinjen.

2. Skriv **inn netplwiz,** og trykk ENTER for å åpne Brukerkontoer-vinduet.

3. Klikk **kontoen du** vil logge på automatisk når Windows starter, i Brukerkontoer.

4. Fjern merket for Brukere må angi brukernavn og passord for å bruke denne datamaskinen.

    ![Brukere må angi et brukernavn- og passordalternativ.](media/users-must-enter-username.png)

5. Klikk **OK**. Du blir bedt om å angi og bekrefte passordet for kontoen du valgte. Klikk **OK for** å fullføre. Neste gang Windows 10 starter, logges den automatisk på kontoen du valgte.
