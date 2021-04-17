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
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828161"
---
# <a name="startup-settings-in-windows-10"></a>Oppstartsinnstillinger i Windows 10

**Endre hvilke apper som kjører automatisk ved oppstart**

1. Gå til [Innstillinger > Apper > Oppstart](ms-settings:startupapps?activationSource=GetHelp).

2. Kontroller at alle apper du vil kjøre ved oppstart, er **slått på**.

**Legge til en app som skal kjøres automatisk ved oppstart**

1. Klikk eller trykk **Start,** og finn appen du vil kjøre ved oppstart.

2. Høyreklikk appen, klikk **Mer**, og klikk deretter **Åpne filplassering**. Dette åpner plasseringen der snarveien til appen er lagret. Hvis det ikke er noe alternativ for Åpne filplassering, betyr det at appen ikke kan kjøre ved oppstart.

3. Når filplasseringen er åpen, trykker du **Windows-logotasten + R,** skriver **inn skall:oppstart** og klikker **deretter OK**. Dette åpner Oppstart-mappen.

4. Kopier og lim inn snarveien til appen fra filplasseringen til Oppstart-mappen.

**Avanserte oppstartsalternativer (inkludert sikkermodus, UEFI-innstillinger og oppstart fra en annen enhet)**

1. Lagre arbeidet og lukk alle åpne dokumenter, siden disse trinnene starter PC-en på nytt.

2. Gå til [Innstillinger > Oppdatering & Sikkerhets-> gjenoppretting](ms-settings:recovery?activationSource=GetHelp).

3. Klikk **Start på nytt** nå under Avansert **oppstart**. 

4. Når PC-en har startet på nytt, går du til skjermbildet Velg et alternativ:

    - Hvis du vil starte opp fra en enhet som en USB-stasjon, klikker **du Bruk en enhet**.

    - Hvis du vil angi UEFI-innstillingene (også kalt BIOS-oppsett), klikker du Feilsøk > Avanserte alternativer > **UEFI-fastvareinnstillinger**. 

    - Hvis du vil angi sikkermodus eller endre avanserte oppstartsinnstillinger, klikker du **Feilsøk**> Avanserte alternativer > Oppstartsinnstillinger og deretter Start **på nytt.** Du kan bli bedt om å angi [BitLocker-gjenopprettingsnøkkelen.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Når PC-en starter på nytt, klikker du oppstartsinnstillingen du vil bruke.