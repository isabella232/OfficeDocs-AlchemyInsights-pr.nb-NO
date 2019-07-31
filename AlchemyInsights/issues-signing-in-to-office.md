---
title: Problemer med pålogging til Office-programmer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938287"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Tom påloggingsbildet i Office-programmer

Hvis du vil løse dette problemet, kan du prøve følgende:
- Installere de siste oppdateringene for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Tilbakestill Internet Explorer-alternativer: Gå til **Verktøy** > **Alternativer for Internett** > **Avansert** > **Tilbakestill Internet Explorer-innstillinger** (Legg merke til at du mister egendefinerte innstillinger), og prøv deretter logger deg på Office på nytt.
- Deaktiver Windows Defender program Guard (WDAG) eller andre lignende brannmur eller antivirus-programmer:
    1. Gå til **programmer**i Kontrollpanel, og velg deretter **Slå Windows-funksjoner på eller av**.
    2. Hvis Windows Defender program Guard er aktivert, kan du prøve å deaktivere den.<br/>
    **Merk:** Du må kanskje starte datamaskinen på nytt.
- Kontroller at Microsoft.AAD.BrokerPlugin [AAD WAM-plugin-modulen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ikke er blokkert av en hvilken som helst program eller brannmur/anti-virus program.
- [Fjern Office legitimasjon](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows-legitimasjoner.<br/>
    **Merk:** Registerbaner for Office-2016 har endret til 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Hvis du vil ha mer informasjon, kan du se [tilkobling problemer i pålogging etter oppdatering til Office-2016 build 16.0.7967 på 10 for Windows](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).