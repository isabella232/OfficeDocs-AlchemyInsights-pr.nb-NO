---
title: Reparere Microsoft 365-appene Kontoen din er i en melding om dårlig tilstand
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
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812545"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Feilmeldingen «Kontoen din er i dårlig tilstand» for å løse Microsoft 365-appene

Hvis du vil løse denne feilen, kan du prøve følgende alternativer på den berørte datamaskinen:

- Åpne en Office-app, og **velg Logg** av  >    >  **filkonto av alle kontoer.** Logg på igjen med en brukerkonto med en gyldig lisens. Hvis du vil ha mer informasjon, se [Kontoer i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Fjern Office-legitimasjon ved hjelp](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) av Windows Legitimasjonsbehandling.<br>
  **Obs!** Registerbanene for Office 2016 er endret til 16.0. Eksempel: \Software\Microsoft\Office\16.0\Common\Identity\
- Hvis feilen oppstår mens du kobler til Office 365 ved hjelp av Office 2013, aktiverer [du moderne godkjenning](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for Office-klienten.

Hvis du vil ha mer informasjon, kan du se Feilsøke apper uten nettlesere som ikke kan logge på [Microsoft 365, Azure eller Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

