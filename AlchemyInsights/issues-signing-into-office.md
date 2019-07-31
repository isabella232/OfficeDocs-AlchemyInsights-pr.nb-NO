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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938286"
---
# <a name="issues-signing-in-to-office-apps"></a>Problemer med pålogging til Office-programmer

Hvis du vil rette påloggingsproblemer med Office-programmer, kan du prøve følgende:

- Fjern alle arbeid-kontoer, bortsett fra den berørte kontoen, ved hjelp av Windows-innstillinger > **Access arbeid eller skole**.
- [Fjern Office legitimasjon](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows-legitimasjoner.<br/>
    **Merk:** Registerbaner for Office-2016 har endret til 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Et Office-program, velger du **fil** > **konto** > **Logg av**. Deretter kan du logge inn med en brukerkonto med en gyldig lisens. Hvis du vil ha mer informasjon, se [kontoer i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- For Mac, kan du se [en Office-2016 for Mac app kan ikke logge på](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Hvis det oppstår en feil under tilkobling til Office 365 ved hjelp av Office-2013, aktivere moderne godkjenning for Office-klient.

Hvis du vil ha mer informasjon, kan du se:
- [Du kan ikke logge på Office 365, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Tilkoblingsproblemer i pålogging etter oppdatering til Office-2016 bygge 16.0.7967 på 10 for Windows](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Beklager, en annen konto fra organisasjonen er allerede logget på denne datamaskinen" i Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Feilsøke påloggingsproblemer med moderne Office-godkjenning når du bruker ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)