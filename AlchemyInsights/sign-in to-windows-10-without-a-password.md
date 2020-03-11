---
title: Logge på Windows 10 uten å bruke et passord
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588289"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Logge på Windows 10 uten å bruke et passord

Hvis du vil unngå å måtte skrive inn et passord ved oppstart av Windows, anbefaler vi at du bruker et av windows Hello-sikre påloggingsalternativene, for eksempel en PIN-kode, ansiktsgjenkjenning eller fingeravtrykk, hvis tilgjengelig. Hvis du virkelig vil deaktivere sikker pålogging, kan du se instruksjonene "Logg på Windows 10 automatisk" nedenfor.

**Sikre Windows Hello-alternativer til kontopassordet**

Gå til **Innstillinger > Kontoer > Påloggingsalternativer** (eller klikk [her).](ms-settings:signinoptions?activationSource=GetHelp) Tilgjengelige påloggingsalternativer vises. Eksempel:

![Påloggingsalternativer.](media/sign-in-options.png)

Klikk eller trykk på ett av alternativene for å konfigurere det. Neste gang du starter eller låser opp Windows, kan du bruke det nye alternativet i stedet for et passord. 

**Logge på Windows 10 automatisk**

**Merk:** Automatisk pålogging er praktisk, men introduserer en sikkerhetsrisiko, spesielt hvis PCen er tilgjengelig av flere personer. 

1. Klikk eller trykk **startknappen** på oppgavelinjen.

2. Skriv inn **netplwiz,** og trykk på Enter-tasten for å åpne Brukerkontoer-vinduet.

3. Klikk kontoen du vil logge på automatisk når Windows starter, i **Brukerkontoer.**

4. Fjern merket for "Brukere må skrive inn et brukernavn og passord for å bruke denne datamaskinen".

    ![Brukere må skrive inn et alternativ for brukernavn og passord.](media/users-must-enter-username.png)

5. Klikk på **OK**. Du vil bli bedt om å skrive inn og bekrefte passordet for kontoen du valgte. Klikk **OK** for å fullføre. Neste gang Windows 10 starter, logger den automatisk på kontoen du valgte.
