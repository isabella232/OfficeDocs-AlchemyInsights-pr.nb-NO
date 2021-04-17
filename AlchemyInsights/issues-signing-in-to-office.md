---
title: Problemer med å logge på Microsoft 365-apper
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
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833048"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tom påloggingsskjerm i Microsoft 365-apper

Prøv følgende for å løse dette problemet:
- Installer de nyeste oppdateringene for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Tilbakestille alternativer for Internet Explorer: Gå til Alternativer for Internett-verktøy Avanserte  >    >    >  **tilbakestillingsinnstillinger** for Internet Explorer (vær oppmerksom på at du mister egendefinerte innstillinger), og prøv deretter å logge på Office på nytt.
- Deaktiver Windows Defender Application Guard (WDAG) eller et lignende brannmur- eller antivirusprogram:
    1. Gå til Programmer i **Kontrollpanel,** og velg deretter **Aktiver eller deaktiver Windows-funksjoner.**
    2. Hvis Windows Defender Application Guard er aktivert, kan du prøve å deaktivere den.<br/>
    **Obs!** Du må kanskje starte datamaskinen på nytt.
- Kontroller at plugin-modulen Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ikke blokkeres av et program eller brannmur/antivirusprogram.
- [Fjern Office-legitimasjon ved hjelp](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) av Windows Legitimasjonsbehandling.<br/>
    **Obs!** Registerbanene for Office 2016 er endret til 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Hvis du vil ha mer informasjon, kan du se Tilkoblingsproblemer ved pålogging etter oppdatering til [Office 2016 bygg 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).