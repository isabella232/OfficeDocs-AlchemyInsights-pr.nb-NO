---
title: Problemer med å logge på Microsoft 365-apper
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
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579910"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tom påloggingsskjerm i Microsoft 365-apper

Prøv følgende for å løse dette problemet:
- Installere de nyeste oppdateringene for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Tilbakestill Internet Explorer-alternativer: Gå til **Verktøy**  >  **Alternativer for Internett**  >  **Avansert**  >  **tilbakestilling av Internet Explorer-innstillinger** (vær oppmerksom på at du mister egendefinerte innstillinger), og prøv deretter å logge på Office på nytt.
- Deaktiver Windows Defender Application Guard (WDAG) eller lignende brannmur eller antivirusprogram:
    1. Gå til Programmer **i**Kontrollpanel, og velg deretter **Aktiver eller deaktiver Windows-funksjoner**.
    2. Hvis Programbeskyttelse for Windows Defender er aktivert, kan du prøve å deaktivere den.<br/>
    **Merk:** Du må kanskje starte datamaskinen på nytt.
- Kontroller at [Plugin-modulen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft.AAD.BrokerPlugin AAD WAM ikke blokkeres av et program eller et program eller et antivirusprogram.
- [Fjern Office-legitimasjon](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows Legitimasjonsbehandling.<br/>
    **Merk:** Registerbanene for Office-2016 er endret til 16.0. (Eks: \Software\Microsoft\Office\16.0\Common\Identity\)

Hvis du vil ha mer informasjon, kan du se [Tilkoblingsproblemer i pålogging etter oppdatering til Office-2016 bygge 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).