---
title: Løse Microsoft 365 appene Kontoen din er i en melding om dårlig tilstand
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
- "2558"
- "9000571"
ms.openlocfilehash: 68c4dfcc0500761f8ce5090fddb9f2ad58af77bc411c9e714b14c383fef177de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068245"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Feilmeldingen Microsoft 365 «Kontoen din er i feil tilstand»

Hvis du vil løse denne feilen, kan du prøve følgende alternativer på den berørte datamaskinen:

- Åpne en Office-app velger du **Logg** av  >  **filkonto**  >  **av alle kontoer**. Logg på igjen ved å bruke en brukerkonto med en gyldig lisens. Hvis du vil ha mer informasjon, se [Kontoer i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Fjern Office legitimasjon ved](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) hjelp av Windows Legitimasjonsbehandling.<br>
  **Obs!** Registerbanene for Office 2016 er endret til 16.0. Eksempel: \Software\Microsoft\Office\16.0\Common\Identity\
- Hvis feilen oppstår når du kobler til Office 365 bruker Office 2013, [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) aktiverer du moderne godkjenning for Office klienten.

Hvis du vil ha mer informasjon, kan du se Feilsøke apper uten nettlesere som ikke kan logge på [Microsoft 365, Azure eller Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

