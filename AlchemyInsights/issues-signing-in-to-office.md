---
title: Problemer med å logge på Microsoft 365 apper
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
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088045"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tom påloggingsskjerm i Microsoft 365 apper

Prøv følgende for å løse dette problemet:
- Installer de nyeste oppdateringene for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Tilbakestille alternativer for Internet Explorer: Gå til Alternativer for Internett-verktøy Avansert tilbakestilling av Internet Explorer Innstillinger (vær oppmerksom på at du mister egendefinerte innstillinger), og prøv deretter å logge på Office  >    >    >   på nytt.
- Deaktiver Windows Defender Application Guard (WDAG) eller et lignende brannmur- eller antivirusprogram:
    1. Gå til Programmer i **Kontrollpanel,** og velg **deretter Windows av eller på**.
    2. Hvis Windows Defender Application Guard er aktivert, kan du prøve å deaktivere den.<br/>
    **Obs!** Du må kanskje starte datamaskinen på nytt.
- Kontroller at plugin-modulen Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ikke blokkeres av et program eller brannmur/antivirusprogram.
- [Fjern Office legitimasjon ved](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) hjelp av Windows Legitimasjonsbehandling.<br/>
    **Obs!** Registerbanene for Office 2016 er endret til 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Hvis du vil ha mer informasjon, kan du se Tilkoblingsproblemer i pålogging etter oppdatering [til Office 2016 bygg 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).