---
title: Fikse Microsoft 365-appene Kontoen din er i en ugyldig tilstandsmelding
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
ms.openlocfilehash: 264307f23a349ef4ebf40f48ddbcddd3216a4927
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580126"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Fikse Microsoft 365-appene "Kontoen din er i dårlig tilstand"-feil

Hvis du vil løse denne feilen, kan du prøve følgende alternativer på den berørte datamaskinen:

- Åpne en Office-app, velg **Logg**av  >  **filkonto**  >  **for alle kontoer**. Logg på igjen med en brukerkonto med en gyldig lisens. Hvis du vil ha mer informasjon, se [Kontoer i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Fjern Office-legitimasjon](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows Legitimasjonsbehandling.<br>
  **Merk:** Registerbanene for Office-2016 er endret til 16.0. For eksempel \Software\Microsoft\Office\16.0\Common\Identity\
- Hvis feilen oppstår under tilkobling til Office 365 ved hjelp av Office-2013, [kan du aktivere moderne godkjenning](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for Office-klienten.

Hvis du vil ha mer informasjon, kan du se [Feilsøke apper som ikke kan logge på Microsoft 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

