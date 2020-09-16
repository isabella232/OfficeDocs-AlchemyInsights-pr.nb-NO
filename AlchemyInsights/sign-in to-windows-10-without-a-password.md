---
title: Logge på Windows 10 uten å bruke et passord
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719962"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Logge på Windows 10 uten å bruke et passord

Vi anbefaler at du bruker et av alternativene for sikker pålogging for Windows Hello, for eksempel en PIN-kode, et ansikts gjenkjenning eller finger avtrykk, hvis det er tilgjengelig for å unngå å måtte skrive inn et passord på Windows-oppstart. Hvis du virkelig vil deaktivere sikker pålogging, kan du se instruksjonene automatisk Logg på Windows 10 nedenfor.

**Sikre Windows Hello-alternativer til konto passordet**

Gå til **innstillinger > kontoer > påloggings alternativer** (eller klikk [her](ms-settings:signinoptions?activationSource=GetHelp)). Tilgjengelige påloggings alternativer vil være oppført. Eksempel:

![Påloggings alternativer.](media/sign-in-options.png)

Klikk eller trykk et av alternativene for å konfigurere det. Neste gang du starter eller låser opp Windows, vil du kunne bruke det nye alternativet i stedet for et passord. 

**Logge på Windows 10 automatisk**

**Obs**! automatisk pålogging er praktisk, men introduserer en sikkerhets risiko, spesielt hvis PC-en er tilgjengelig for flere personer. 

1. Klikk eller trykk **Start** -knappen på oppgave linjen.

2. Skriv inn **NETPLWIZ** , og trykk Enter-tasten for å åpne Brukerkontoer-vinduet.

3. Klikk kontoen du vil logge på automatisk når Windows starter, i **bruker kontoer**.

4. Fjern merket i avmerkings boksen brukere må angi et bruker navn og passord for å bruke denne data maskinen.

    ![Brukere må angi et bruker navn og et passord alternativ.](media/users-must-enter-username.png)

5. Klikk **OK**. Du blir bedt om å skrive inn og bekrefte passordet for kontoen du valgte. Klikk **OK** for å fullføre. Neste gang Windows 10 starter, vil den automatisk logge på kontoen du valgte.
