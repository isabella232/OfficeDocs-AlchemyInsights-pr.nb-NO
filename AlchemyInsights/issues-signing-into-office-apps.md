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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579874"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Fikse Microsoft 365-appene meldingen "Datamaskinens klarerte plattformmodul fungerer ikke som den skal"

For å løse denne filen kan du prøve følgende:

- Installere de nyeste oppdateringene for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Fjern Office-legitimasjon](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows Legitimasjonsbehandling.<br/>
    **Merk:** Registerbanene for Office-2016 er endret til 16.0. (Eks: \Software\Microsoft\Office\16.0\Common\Identity\)
- Prøv [brukergjenopprettingsprosessen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) for å fikse TPM-feil (Trusted Platform Module).
- Angi EnableADAL = 0 ved hjelp av følgende trinn:  
    1. Høyreklikk Start-knappen i Windows, velg **Kjør**, Skriv inn **regedit**, og velg deretter **OK**.
    2. Velg **Ja** for å tillate at Registerredigering gjør endringer på enheten.
    3. I Registerredigering legger du til en DWORD-verdi for **EnableADAL** med en innstilling **på 0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Hvis du vil ha mer informasjon, kan du se [Tilkoblingsproblemer i pålogging etter oppdatering til Office-2016 bygge 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).