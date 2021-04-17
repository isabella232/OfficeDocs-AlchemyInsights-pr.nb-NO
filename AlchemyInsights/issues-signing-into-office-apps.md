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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833013"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Retting av Microsoft 365-appene Meldingen «Datamaskinens klarerte plattformmodul fungerer ikke som den skal»

For å løse denne filen kan du prøve følgende:

- Installer de nyeste oppdateringene for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Fjern Office-legitimasjon ved hjelp](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) av Windows Legitimasjonsbehandling.<br/>
    **Obs!** Registerbanene for Office 2016 er endret til 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Prøv [gjenopprettingsprosessen for brukere for](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) å løse TPM-feil (Trusted Platform Module).
- Angi EnableADAL = 0 ved hjelp av følgende fremgangsmåte:  
    1. Høyreklikk Start-knappen i Windows, velg **Kjør,** skriv **inn regedit**, og velg deretter **OK**.
    2. Velg **Ja** for å tillate at Registerredigering kan gjøre endringer på enheten.
    3. Legg til en DWORD-verdi for **EnableADAL** i Registerredigering med innstillingen **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Hvis du vil ha mer informasjon, kan du se Tilkoblingsproblemer ved pålogging etter oppdatering til [Office 2016 bygg 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).