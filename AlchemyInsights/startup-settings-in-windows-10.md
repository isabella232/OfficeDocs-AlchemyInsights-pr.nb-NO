---
title: Oppstartsinnstillinger i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2020
ms.locfileid: "42409236"
---
# <a name="startup-settings-in-windows-10"></a>Oppstartsinnstillinger i Windows 10

**Endre hvilke apper som kjøres automatisk ved oppstart**

1. Gå til [Innstillinger > Apper > Oppstart](ms-settings:startupapps?activationSource=GetHelp).

2. Kontroller at alle apper du vil kjøre ved oppstart er slått **På**.

**Legge til en app som skal kjøres automatisk ved oppstart**

1. Klikk eller trykk på **Start,** og finn appen du vil kjøre ved oppstart.

2. Høyreklikk appen, klikk **Mer**, og klikk deretter **Åpne filplassering**. Dette åpner plasseringen der snarveien til appen er lagret. Hvis det ikke finnes noe alternativ for Åpne filplassering, betyr det at appen ikke kan kjøre ved oppstart.

3. Når filplasseringen er åpen, trykker du **Windows-logotasten + R**, skriver **inn shell:startup**, og deretter klikker du **OK**. Dette åpner oppstartsmappen.

4. Kopier og lim inn snarveien til appen fra filplasseringen til oppstartsmappen.

**Avanserte oppstartsalternativer (inkludert sikkermodus, UEFI-innstillinger og oppstart fra en annen enhet)**

1. Lagre arbeidet ditt og lukk eventuelle åpne dokumenter, siden disse trinnene starter PCen på nytt.

2. Gå til [Innstillinger > Oppdater & sikkerhet > gjenoppretting](ms-settings:recovery?activationSource=GetHelp).

3. Klikk Start **på nytt nå**under Avansert **oppstart**. 

4. Når PC-en starter på nytt til skjermbildet Velg et alternativ:

    - Hvis du vil starte opp fra en enhet som en USB-stasjon, klikker du **Bruk en enhet**.

    - Hvis du vil angi UEFI-innstillingene (noen ganger kalt BIOS-oppsett), klikker du **Påsøk > Avanserte alternativer > UEFI-fastvareinnstillinger**. 

    - Hvis du vil angi sikkermodus eller endre avanserte oppstartsinnstillinger, klikker du **Feilsøk > Avanserte alternativer > Oppstartsinnstillinger**, og deretter klikker du **Start på nytt**. Du kan bli bedt om å angi [BitLocker-gjenopprettingsnøkkelen](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Når PCen starter på nytt, klikker du oppstartsinnstillingen du vil bruke.