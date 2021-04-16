---
title: Strøm- eller batteriikon mangler i Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790557"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>Strøm- eller batteriikon mangler i Windows 10

Hvis Windows 10-enheten har et batteri (f.eks. en bærbar datamaskin eller et nettbrett eller en PC som er koblet via USB til en UPS), vises vanligvis et strøm/batteri-ikon på oppgavelinjen nær klokken, for eksempel:

![Batteriikon](media/battery-icon.png)

Hvis du ikke ser dette ikonet, kan det være skjult:

1. Gå til **[Innstillinger > Personalisering > Oppgavelinje](ms-settings:taskbar?activationSource=GetHelp)**.

2. I Systemstatusfeltet klikker du på **Velg hvilke ikoner som skal vises på oppgavelinjen**.

3. Finn deretter **Power**-elementet i listen, og veksle innstillingen til **På**.

    ![Vis strømikonet i oppgavelinjen](media/power-icon-on.png)

**Feilsøking**

Hvis du har fulgt instruksjonene over og **Power**-veksleknappen er nedtonet eller ikke synlig, skriver du inn **Enhetsbehandling** i søkeboksen på oppgavelinjen, og deretter velger du **Enhetsbehandling** i listen over resultater. Under **Batterier** høyreklikker du på batteriet for enheten og klikker på **Deaktivere**, og klikker på **Ja**. Vent noen sekunder og høyreklikk deretter på batteriet og klikk **Aktivere**. Start deretter enheten på nytt.

Hvis du har fulgt instruksjonene over, men batteriikonet ikke vises på oppgavelinjen, skriver du inn **oppgavebehandling** i søkeboksen på oppgavelinjen, og klikker deretter **Oppgavebehandling** i listen over resultater. Gå til **Prosesser** -fanen under **Navn**, høyreklikk på **Explorer**, og klikk deretter på **Start**.
