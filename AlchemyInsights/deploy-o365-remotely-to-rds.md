---
title: Distribuere Microsoft 365-apper for bedrifter for delt bruk på RDS, Terminal Server eller VDI
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
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200682"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Distribuere Microsoft 365-apper for bedrifter for delt bruk på RDS, Terminal Server eller VDI

Slik distribuerer du Microsoft 365-apper for bedrifter ved hjelp av Remote Desktop Services (RDS), tidligere kalt Terminal Services:

- Du må ha et Microsoft 365 For Business-abonnement eller et Office 365-abonnement som inneholder Microsoft 365-apper for bedrifter, for eksempel Office 365 Enterprise E3 eller Enterprise E5.
   > [!NOTE]
   > Microsoft 365-appene for bedrifter og Microsoft 365 Business Standard-abonnementer inkluderer ikke Microsoft 365-apper for bedrifter.
- Du må aktivere [aktivering av delt datamaskin](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Du kan også laste ned og kjøre [Microsofts assistent](https://aka.ms/SaRA_OfficeSCA_M365Portal) for støtte og gjenoppretting for å installere Microsoft 365-apper for bedrifter i modus for aktivering av delt datamaskin.

Hvis du vil ha mer informasjon om forutsetninger, installasjonsinstruksjoner og veiledning om tilpassede installasjoner ved hjelp av distribusjonsverktøyet for Office, kan du se Distribuere [Microsoft 365-apper for bedrifter](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)ved hjelp av Eksterne skrivebordstjenester .

Slik løser du feil relatert til aktivering av delt datamaskin:

- Se [Feilsøke problemer med aktivering av delt datamaskin for Microsoft 365-apper for bedrifter.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Se [Tilbakestille Microsoft 365 Apps for enterprise for tilstand for organisasjonsaktivering](https://go.microsoft.com/fwlink/?linkid=2109218).

Hvis du vil installere Microsoft 365-apper for bedrifter på RDS fra administrasjonssenteret for Microsoft 365, som bruker standard installasjonsinnstillinger, bruker du følgende fremgangsmåte:

1. Kontroller hvilket abonnement du har. [Finn ut hvordan](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Bytt om nødvendig til et annet abonnement. [Finn ut hvordan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Hvis Office allerede er installert på RDS-serveren ved hjelp av andre Microsoft-abonnementer, må du avinstallere det. Du kan for eksempel gå til **Avinstallere** et program i  >  **kontrollpanelet.** Avinstaller ved hjelp [av Microsofts assistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) for støtte og gjenoppretting hvis det er problemer.
4. Logg på administrasjonssenteret for Microsoft 365 med administratorkontoen på RDS-serveren, og installer [Microsoft 365-apper for bedrifter.](https://portal.office.com/OLS/MySoftware.aspx)
5. Når Office er installert, ***må du ikke åpne eller logge på*** noen Office-programmer.
6. Aktiver aktivering av delt datamaskin på RDS-serveren ved å redigere registeret ved å følge disse trinnene:
   1. Høyreklikk Windows-knappen nederst til venstre på skjermen, og velg **Kjør**. Skriv regedit i **Åpne**-boksen, og velg deretter **OK**.
   2. Velg **Ja** når du blir bedt om å tillate at Registerredigering gjør endringer på enheten.
   3. Legg til en strengverdi for **SharedComputerLicensing** i Registerredigering med innstillingen 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Logg på som sluttbruker  på RDS-serveren, og kontroller at aktivering av delt datamaskin er aktivert [for Microsoft 365-apper for bedrifter.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
