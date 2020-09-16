---
title: Fikse Microsoft 365-appene kontoen din er i en ugyldig status melding
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744554"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Løse Microsoft 365-appene kontoen din er i en feil melding om ugyldig tilstand

Hvis du vil rette denne feilen, kan du prøve følgende alternativer på den berørte data maskinen:

- Åpne en Office-app, og velg **fil**  >  **konto**  >  **Logg av alle kontoer**. Logg på igjen med en bruker konto med en gyldig lisens. Hvis du vil ha mer informasjon, se [Kontoer i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Fjern Office-legitimasjon](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows-legitimasjons behandling.<br>
  **Obs!** Register banene for Office 2016 har blitt endret til 16,0. For eksempel \Software\Microsoft\Office\16.0\Common\Identity\
- Hvis feilen oppstår mens du kobler til Office 365 ved hjelp av Office 2013, [kan du aktivere moderne godkjenning](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for Office-klienten.

Hvis du vil ha mer informasjon, kan du se [feilsøke programmer som ikke er nett lesere som ikke kan logge på Microsoft 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

