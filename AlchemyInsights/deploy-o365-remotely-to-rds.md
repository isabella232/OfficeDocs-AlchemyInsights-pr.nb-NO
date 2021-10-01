---
title: Distribuere Microsoft 365 Apps for delt bruk på RDS, Terminal Server eller VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077259"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>Distribuere Microsoft 365 Apps for delt bruk på RDS, Terminal Server eller VDI

Hvis du Microsoft 365 Apps bruke Remote Desktop Services (RDS), tidligere Terminal Services, må du:

- Bruk den enkle løsningen for å aktivere TLS 1.2 som standard hvis du kjører en eldre versjon av Windows (for eksempel Windows 7 SP1, Windows Server 2008 R2). Hvis du vil ha enkel løsning og mer informasjon, kan du se Oppdatere for å aktivere [TLS 1.1 og TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)som standard sikre protokoller i WinHTTP i Windows . 
- Ha en plan som inneholder Microsoft 365 Apps for enterprise (tidligere Office 365 Plus). For eksempel Office 365 E3 eller Microsoft 365 E5, eller en plan som inneholder skrivebordsversjonen av Project eller Visio, for eksempel Project-abonnement 3 eller Visio-abonnement 2, eller Microsoft 365 Business Premium-planen, som også inneholder Microsoft 365 Apps for business.
- Aktiver aktivering av delt datamaskin. Hvis du vil ha mer informasjon, [kan du se Oversikt over aktivering](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)av delt datamaskin for Microsoft 365 Apps .

**Obs!** Hvis du vil Microsoft 365 Apps i modus for aktivering av delt datamaskin, kan du laste ned og [kjøre Microsoft assistent for støtte og gjenoppretting](https://aka.ms/SaRA_OfficeSCA_M365Portal). Hvis du vil ha mer informasjon om forutsetninger, installasjonsinstruksjoner og veiledning for å tilpasse installasjoner ved hjelp av distribusjonsverktøyet Office, kan du se Distribuere Microsoft 365 Apps ved hjelp av [Eksterne skrivebordstjenester](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services).

Hvis du vil løse feil relatert til aktivering av delt datamaskin, kan du se:

- [Feilsøke problemer med aktivering av delt datamaskin for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Tilbakestille Microsoft 365 Apps for enterprise aktiveringstilstand](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Hvis du vil installere Microsoft 365 Apps på RDS fra Administrasjonssenter for Microsoft 365, som bruker standard installasjonsinnstillinger, følger du disse trinnene:

1. Kontroller hva Microsoft 365 planen du har. Hvis du vil ha mer informasjon, [kan du se Hvilket abonnement har jeg?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Bytt om nødvendig til en annen Microsoft 365 plan. Hvis du vil ha mer informasjon, kan [du se Oppgradere til en annen plan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan).

1. Hvis Microsoft 365 Apps allerede er installert på RDS-serveren ved hjelp av andre inkompatible planer, avinstallerer du det ved å gå til Avinstallere et program i   >  **kontrollpanelet.** Hvis det er problemer, avinstallerer du ved å laste [ned Microsoft assistent for støtte og gjenoppretting](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. På RDS-serveren logger du på Administrasjonssenter for Microsoft 365 med administratorkontoen og [installerer Office](https://portal.office.com/OLS/MySoftware.aspx).

   Når Office er installert, må du ikke åpne eller logge på noen Office programmer.

1. Aktiver aktivering av delt datamaskin på RDS-serveren ved å redigere registeret:

   1. Høyreklikk på knappen Windows nederst til venstre på skjermen, og velg **Kjør**. Skriv regedit i **Åpne**-boksen, og velg deretter **OK**.

   1. Når du blir bedt om å tillate at Registerredigering gjør endringer på enheten, velger du **Ja**.

   1. Legg til en strengverdi for **SharedComputerLicensing** med innstillingen **1** under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration i Registerredigering.

1. Logg på som sluttbruker på RDS-serveren, og kontroller at aktivering av delt datamaskin er aktivert for Microsoft 365 Apps. 

   Hvis du vil ha mer informasjon, kan du se Kontrollere at aktivering av delt [datamaskin er aktivert for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps).