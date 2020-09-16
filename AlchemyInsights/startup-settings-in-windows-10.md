---
title: Oppstarts innstillinger i Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751144"
---
# <a name="startup-settings-in-windows-10"></a>Oppstarts innstillinger i Windows 10

**Endre hvilke apper som kjører automatisk ved oppstart**

1. Gå til [innstillinger > apper > oppstart](ms-settings:startupapps?activationSource=GetHelp).

2. Kontroller at appen du vil kjøre ved oppstart, er slått **på**.

**Legge til en app som skal kjøres automatisk ved oppstart**

1. Klikk eller trykk **Start** , og Finn appen du vil kjøre ved oppstart.

2. Høyre klikk appen, klikk **mer**, og klikk deretter **Åpne fil plassering**. Dette åpner plasseringen der snarveien til appen er lagret. Hvis det ikke er noe alternativ for å åpne fil plasseringen, betyr det at appen ikke kan kjøre ved oppstart.

3. Med fil plasseringen åpen trykker du Windows- **logotasten + R**, skriver inn **Shell: oppstart**, og deretter klikker du **OK**. Dette åpner oppstarts mappen.

4. Kopier og lim inn snarveien til appen fra fil plasseringen til oppstarts mappen.

**Avanserte oppstarts alternativer (inkludert sikker modus, UEFI-innstillinger og oppstart fra en annen enhet)**

1. Lagre arbeidet ditt, og lukk eventuelle åpne dokumenter, siden disse trinnene vil starte data maskinen på nytt.

2. Gå til [innstillinger > oppdater & sikkerhets > gjenoppretting](ms-settings:recovery?activationSource=GetHelp).

3. Klikk **Start på nytt nå**under **Avansert oppstart**. 

4. Når PC-en starter på nytt i Velg et alternativ-skjerm bilde:

    - Hvis du vil starte fra en enhet som en USB-stasjon, klikker du **Bruk en enhet**.

    - Hvis du vil angi UEFI-innstillingene (noen ganger kalt BIOS-konfigurasjon), klikker du **feil søking > avanserte alternativer > innstillinger for UEFI-fastvare**. 

    - Hvis du vil angi sikker modus eller endre avanserte oppstarts innstillinger, klikker du **feilsøk > avanserte alternativer > oppstarts innstillinger**, og deretter klikker du **Start på nytt**. Du kan bli bedt om å angi [gjenopprettings nøkkelen for BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Når PC-en starter på nytt, klikker du på oppstarts innstillingen du vil bruke.