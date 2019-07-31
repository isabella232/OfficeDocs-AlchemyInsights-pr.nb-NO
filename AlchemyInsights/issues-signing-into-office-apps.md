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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938288"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Reparerer Office apps "klarerte plattformmodulen (TPM) på datamaskinen ikke fungerer skikkelig" melding

Hvis du vil løse dette problemet, kan du prøve følgende:

- Installere de siste oppdateringene for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Fjern Office legitimasjon](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows-legitimasjoner.<br/>
    **Merk:** Registerbaner for Office-2016 har endret til 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Prøv [gjenopprettingsprosessen for brukeren](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) for å rette feil for klarert plattformmodul (TPM).
- Angi EnableADAL = 0 ved å gjøre følgende:  
    1. Høyreklikk startknappen i Windows, velg **Kjør**, Skriv inn **regedit**, og velg **OK**.
    2. Velg **Ja** Hvis du vil tillate Registerredigering til å gjøre endringer til enheten.
    3. I Registerredigering, legge til DWORD-verdien **EnableADAL** med innstillingen **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Hvis du vil ha mer informasjon, kan du se [tilkobling problemer i pålogging etter oppdatering til Office-2016 build 16.0.7967 på 10 for Windows](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).