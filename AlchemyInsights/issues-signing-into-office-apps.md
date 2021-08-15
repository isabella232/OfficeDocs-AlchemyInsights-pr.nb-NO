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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986900"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Melding om Microsoft 365 «Datamaskinens klarerte plattformmodul fungerer ikke som den skal»

For å løse denne filen kan du prøve følgende:

- Installer de nyeste oppdateringene for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Fjern Office legitimasjon ved](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) hjelp av Windows Legitimasjonsbehandling.<br/>
    **Obs!** Registerbanene for Office 2016 er endret til 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Prøv [gjenopprettingsprosessen for brukere for](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) å løse TPM-feil (Trusted Platform Module).
- Angi EnableADAL = 0 ved hjelp av følgende fremgangsmåte:  
    1. Høyreklikk startknappen Windows, velg **Kjør,** skriv **inn regedit**, og velg deretter **OK**.
    2. Velg **Ja** for å tillate at Registerredigering kan gjøre endringer på enheten.
    3. Legg til en DWORD-verdi for **EnableADAL** i Registerredigering med innstillingen **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Hvis du vil ha mer informasjon, kan du se Tilkoblingsproblemer i pålogging etter oppdatering [til Office 2016 bygg 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).