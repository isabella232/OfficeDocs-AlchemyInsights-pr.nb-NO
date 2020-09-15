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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695188"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Løse Microsoft 365-appene data maskinens klarerte plattform modul fungerer ikke som den skal: melding

For å løse denne filen kan du prøve følgende:

- Installer de nyeste oppdateringene for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Fjern Office-legitimasjon](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows-legitimasjons behandling.<br/>
    **Obs!** Register banene for Office 2016 har blitt endret til 16,0. (Eks: \Software\Microsoft\Office\16.0\Common\Identity\)
- Prøv [bruker gjenopprettings prosessen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) for å løse problemer med klarert plattform modul (TPM).
- Angi EnableADAL = 0 ved hjelp av følgende trinn:  
    1. Høyre klikk Start knappen i Windows, velg **Kjør**, Skriv inn **regedit**, og velg deretter **OK**.
    2. Velg **Ja** for å tillate register redigering å gjøre endringer på enheten.
    3. I register redigering legger du til en DWORD-verdi på **EnableADAL** med en innstilling på **0** under HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Hvis du vil ha mer informasjon, kan du se [tilkoblings problemer i pålogging etter oppdatering til Office 2016 Bygg 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).