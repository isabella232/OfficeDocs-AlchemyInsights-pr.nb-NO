---
title: Problemer med å logge på Office-apper
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
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763010"
---
# <a name="issues-signing-in-to-office-apps"></a>Problemer med å logge på Office-apper

Prøv følgende for å løse påloggingsproblemer med Office-apper:

- Fjern alle arbeidskontoer, unntatt den berørte kontoen, ved hjelp av Windows-innstillinger > **Access-jobb eller skole**.
- [Fjern Office-legitimasjon](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows Credential Manager.<br/>
    **Merk:** Registerbanene for Office-2016 er endret til 16.0. (F.eks. \Software\Microsoft\Office\16.0\Common\Identity\)
- Åpne en Office-app, velg Logg**av** > **filkonto** > . **File** Logg deretter på med en brukerkonto med en gyldig lisens. Hvis du vil ha mer informasjon, se [Kontoer i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Hvis du bruker Mac, kan du ta en titt på [Jeg kan ikke logge på en Office 2016 for Mac-app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Hvis feilene oppstår under tilkobling til Microsoft 365 ved hjelp av Office-2013, aktiverer du moderne godkjenning for Office-klienten.

Hvis du vil ha mer informasjon, kan du se:
- [Du kan ikke logge på Microsoft 365, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Tilkoblingsproblemer i pålogging etter oppdatering til Office-2016 bygge 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Beklager, en annen konto fra organisasjonen er allerede logget på denne datamaskinen" i Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Feilsøke påloggingsproblemer med moderne Office-godkjenning når du bruker ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)