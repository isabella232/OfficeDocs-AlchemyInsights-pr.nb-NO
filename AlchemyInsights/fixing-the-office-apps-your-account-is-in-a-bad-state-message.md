---
title: Fikse Office-apper kontoen din er i en feilmelding
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969649"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Fikse Office-appene "Kontoen din er i en dårlig tilstand" feil

Hvis du vil løse denne feilen, kan du prøve følgende alternativer på den berørte datamaskinen:

- Åpne en Office-app, velg Logg**av** **filkonto** > **** > for alle kontoer . Logg på igjen ved hjelp av en brukerkonto med en gyldig lisens. Hvis du vil ha detaljert informasjon, kan du se [Kontoer i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Fjern Office-legitimasjon](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows Credential Manager.<br>
  **Merk:** Registerbanene for Office-2016 er endret til 16.0. For eksempel \Software\Microsoft\Office\16.0\Common\Identity\
- På den berørte datamaskinen angir du EnableADAL = 0 ved hjelp av følgende trinn:  
     1. Høyreklikk Windows-knappen, og velg **Kjør**. Skriv inn **regedit**i **Åpne-boksen,** og velg deretter **OK**.
     2. Velg **Ja** når du blir bedt om å la Registerredigering gjøre endringer på enheten.
    3. I Registerredigering legger du til en DWORD-verdi for EnableADAL med en innstilling på 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.
- Hvis feilen oppstår under tilkobling til Office 365 ved hjelp av Office-2013, [aktiverer du moderne godkjenning](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for Office-klienten.

Hvis du vil ha mer informasjon, kan du se Feilsøke apper som [ikke er i nettleseren, som ikke kan logge på Office 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

