---
title: Problemer med å logge på Microsoft 365-apper
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
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695296"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Blank påloggings skjerm i Microsoft 365-apper

Prøv følgende for å løse problemet:
- Installer de nyeste oppdateringene for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Tilbakestille alternativer for Internet Explorer: gå til **verktøy**  >  **Alternativer for Internet**t  >  **Avansert**  >  **tilbakestille Internet Explorer-innstillinger** (Vær oppmerksom på at du mister egen definerte innstillinger), og prøv deretter å logge på Office på nytt.
- Deaktiver Windows Defender Application Guard (WDAG) eller et lignende brann mur-eller antivirus program:
    1. Gå til **programmer**i kontroll panel, og velg deretter **slå Windows-funksjoner på eller av**.
    2. Hvis Windows Defender Application Guard er aktivert, kan du prøve å deaktivere det.<br/>
    **Obs!** Det kan hende du må starte data maskinen på nytt.
- Kontroller at plugin-modulen Microsoft. AAD. BrokerPlugin [AAD-WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ikke blokkeres av program-eller brann mur-/antivirus program.
- [Fjern Office-legitimasjon](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows-legitimasjons behandling.<br/>
    **Obs!** Register banene for Office 2016 har blitt endret til 16,0. (Eks: \Software\Microsoft\Office\16.0\Common\Identity\)

Hvis du vil ha mer informasjon, kan du se [tilkoblings problemer i pålogging etter oppdatering til Office 2016 Bygg 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).