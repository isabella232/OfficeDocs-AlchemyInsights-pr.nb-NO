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
- "2574"
ms.openlocfilehash: 1954ceef7454a4bb047d366cc55793dc78a969e375e9eea88d2d0dbe7f4997ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088009"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problemer med å logge på Microsoft 365 Apps

Hvis du vil løse påloggingsproblemer med Microsoft 365 apper, kan du prøve følgende alternativer på den berørte maskinen:  

- Hvis Windows kan du [se Anbefalinger løse vanlige påloggingsproblemer](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- For Mac kan du [se Kan ikke logge på en Office 2016 for Mac-app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Tips** På Windows-maskiner kan vi diagnostisere og ordne flere vanlige problemer med pålogging til Office for deg. Last ned og kjør **[assistent for støtte og gjenoppretting](https://aka.ms/SaRA-OfficeSignInScenario)** for å bruke vårt automatiserte verktøy.

**Obs!** Deaktivering av moderne godkjenning (ADAL) eller administrasjon av nettkontoer (WAM) for å løse påloggings- eller aktiveringsproblemer **anbefales ikke.** Hvis feilene oppstår når du kobler til Microsoft 365 bruker Office 2013, må du kontrollere at du aktiverer moderne [godkjenning](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for Office klient.

Hvis du vil ha spesifikke feilsøkingshandlinger, kan du se:

[Tilkoblingsproblemer i pålogging etter oppdatering til Office-2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Du kan ikke logge på organisasjonskontoen, for eksempel Office 365, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Feilsøke apper uten nettlesere som ikke kan logge på Office 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Gjentatte ganger bedt om legitimasjon i Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)