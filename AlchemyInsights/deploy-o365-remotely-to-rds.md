---
title: Distribuere Microsoft 365 Apps for enterprise for delt bruk på RDS, Terminal Server eller VDI
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
ms.openlocfilehash: 55b86557ec205dde2c459d76e8e330d2a8271dbec723f079e119ebe409b41c3f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031487"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Distribuere Microsoft 365 Apps for enterprise for delt bruk på RDS, Terminal Server eller VDI

Slik distribuerer Microsoft 365 Apps for enterprise bruke Remote Desktop Services (RDS), tidligere kalt Terminal Services:

- Du må ha et Microsoft 365 for bedrifter-abonnement eller en Office 365-plan som inneholder Microsoft 365 Apps for enterprise, for eksempel Office 365 Enterprise E3 eller Enterprise E5.
   > [!NOTE]
   > Abonnementene Microsoft 365 Apps for business Microsoft 365 Business Standard inkluderer ikke Microsoft 365 Apps for enterprise.
- Du må aktivere [aktivering av delt datamaskin](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Du kan også laste ned og kjøre [Microsoft assistent for støtte og gjenoppretting](https://aka.ms/SaRA_OfficeSCA_M365Portal) installere Microsoft 365 Apps for enterprise i modus for aktivering av delt datamaskin.

Hvis du vil ha mer informasjon om forutsetninger, installasjonsinstruksjoner og veiledning om tilpassede installasjoner ved hjelp av distribusjonsverktøyet for Office, kan du se Distribuere Microsoft 365 Apps for enterprise ved hjelp av [Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Slik løser du feil relatert til aktivering av delt datamaskin:

- Se [Feilsøke problemer med aktivering av delt datamaskin for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Se [Tilbakestille Microsoft 365 Apps for enterprise for tilstand for organisasjonsaktivering](https://go.microsoft.com/fwlink/?linkid=2109218).

Hvis du vil installere Microsoft 365 Apps for enterprise på RDS fra ***Administrasjonssenter for Microsoft 365,*** som bruker standard installasjonsinnstillinger, bruker du følgende fremgangsmåte:

1. Kontroller hvilket abonnement du har. [Finn ut hvordan](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Bytt om nødvendig til et annet abonnement. [Finn ut hvordan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Hvis Office allerede er installert på RDS-serveren ved hjelp av andre Microsoft-abonnementer, må du avinstallere det. Du kan for eksempel gå til **Avinstallere** et program i  >  **kontrollpanelet.** Avinstaller ved [hjelp av Microsoft assistent for støtte og gjenoppretting](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis det er problemer.
4. Logg på RDS-serveren med administratorkontoen Administrasjonssenter for Microsoft 365 administratorkontoen, og [installer Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5. Når Office er installert, må du ikke åpne eller ***logge*** på noen Office programmer.
6. Aktiver aktivering av delt datamaskin på RDS-serveren ved å redigere registeret ved å følge disse trinnene:
   1. Høyreklikk på Windows nederst til venstre på skjermen, og velg **Kjør**. Skriv regedit i **Åpne**-boksen, og velg deretter **OK**.
   2. Velg **Ja** når du blir bedt om å tillate at Registerredigering gjør endringer på enheten.
   3. Legg til en strengverdi for **SharedComputerLicensing** i Registerredigering med en innstilling på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Logg på som sluttbruker  på RDS-serveren, og kontroller at aktivering av delt datamaskin [er aktivert for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).
