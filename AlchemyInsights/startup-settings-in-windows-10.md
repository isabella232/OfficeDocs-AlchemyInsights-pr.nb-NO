---
title: Oppstartsinnstillinger i Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909835"
---
# <a name="startup-settings-in-windows-10"></a>Oppstartsinnstillinger i Windows 10

**Endre hvilke apper som kjører automatisk ved oppstart**

1. Gå til [Innstillinger > Apper > Oppstart](ms-settings:startupapps?activationSource=GetHelp).

2. Kontroller at alle apper du vil kjøre ved oppstart, er **slått på**.

**Legge til en app som skal kjøres automatisk ved oppstart**

1. Klikk eller trykk **Start,** og finn appen du vil kjøre ved oppstart.

2. Høyreklikk appen, klikk **Mer**, og klikk deretter **Åpne filplassering**. Dette åpner plasseringen der snarveien til appen er lagret. Hvis det ikke er noe alternativ for Åpne filplassering, betyr det at appen ikke kan kjøre ved oppstart.

3. Når filplasseringen er åpen, trykker **du på Windows + R,** skriver inn **shell:startup** og klikker **deretter OK**. Dette åpner Oppstart-mappen.

4. Kopier og lim inn snarveien til appen fra filplasseringen til Oppstart-mappen.

**Avanserte oppstartsalternativer (inkludert Safe, UEFI-innstillinger og oppstart fra en annen enhet)**

1. Lagre arbeidet og lukk alle åpne dokumenter, siden disse trinnene starter PC-en på nytt.

2. Gå til [Innstillinger > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).

3. Klikk **Start på nytt** nå under Avansert **oppstart**. 

4. Når PC-en har startet på nytt, går du til skjermbildet Velg et alternativ:

    - Hvis du vil starte opp fra en enhet som en USB-stasjon, klikker **du Bruk en enhet**.

    - Hvis du vil angi UEFI-innstillingene (noen ganger kalt BIOS-oppsett), klikker du Feilsøk > Avanserte alternativer **> UEFI-Innstillinger.** 

    - Hvis du vil Safe eller endre avanserte oppstartsinnstillinger, klikker du Feilsøk > Avanserte alternativer **>** Oppstarts-Innstillinger og deretter Start **på nytt**. Du kan bli bedt om å angi [BitLocker-gjenopprettingsnøkkelen.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Når PC-en starter på nytt, klikker du oppstartsinnstillingen du vil bruke.