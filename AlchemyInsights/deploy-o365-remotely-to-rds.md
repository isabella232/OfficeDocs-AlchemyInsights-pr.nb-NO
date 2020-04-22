---
title: Distribuere Microsoft 365-apper for bedrifter for delt bruk på RDS, Terminal Server eller VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: ddd44d40e9430ee31b8b734450dde0defef229d7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704714"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Distribuere Microsoft 365-apper for bedrifter for delt bruk på RDS, Terminal Server eller VDI

Slik distribuerer du Microsoft 365-apper for enterprise ved hjelp av Remote Desktop Services (RDS), tidligere kalt Terminal Services:
- Du må ha en Microsoft 365 For Business-plan eller en Office 365-plan som inkluderer Microsoft 365 Apps for enterprise, for eksempel Office 365 Enterprise E3 eller Enterprise E5.
   > [!NOTE] 
   > Microsoft 365 Apps for bedrifter og Microsoft 365 Business Premium Standard-planer inkluderer ikke Microsoft 365 Apps for enterprise.
- Du må aktivere [aktivisering av delt datamaskin](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Du kan også laste ned og kjøre [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) for å installere Microsoft 365 Apps for enterprise i delt datamaskinaktiveringsmodus.

Hvis du vil ha mer informasjon om forutsetninger, installasjonsinstruksjoner og veiledning om tilpassede installasjoner ved hjelp av Distribusjonsverktøy for Office, kan du se [Distribuere Microsoft 365-apper for bedrifter ved hjelp av Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Slik løser du feil relatert til delt datamaskinaktivering:
- Se [Feilsøke problemer med aktivering av delt datamaskin for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Se [Tilbakestille Microsoft 365 Apps for enterprise for tilstand for organisasjonsaktivering](https://go.microsoft.com/fwlink/?linkid=2109218).

Hvis du vil installere Microsoft 365 Apps for enterprise på RDS fra administrasjonssenteret for Microsoft 365, ***som bruker standard installasjonsinnstillinger***, gjør du følgende:

1.    Sjekk hvilket abonnement du har. [Finn ut hvordan](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    Bytt om nødvendig til et annet abonnement. [Finn ut hvordan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    Hvis Office allerede er installert på RDS-serveren ved hjelp av andre Microsoft-abonnementer, må du avinstallere den. Hvis du for eksempel går til **Kontrollpanel** > **Avinstaller et program**. Avinstaller ved hjelp av [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du støter på problemer.
4.    Logg på administrasjonssenteret for Microsoft 365 med administratorkontoen, og [installer Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx)på RDS-serveren.
5.    Når Office er installert, ***må du ikke åpne eller logge på*** noen Office-programmer.
6.    Aktiver aktivisering av delt datamaskin på RDS-serveren ved å redigere registret ved å følge disse trinnene:
   1. Høyreklikk Windows-knappen nederst til venstre på skjermen, og velg **Kjør**. Skriv inn **regedit**i Åpne-boksen, og velg deretter **OK**.
   2. Velg **Ja** når du blir bedt om å tillate Registerredigering å gjøre endringer på enheten.
   3. Legg til en strengverdi for **SharedComputerLicensing** i Registerredigering med en innstilling på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Logg på som ***sluttbruker på*** RDS-serveren, og kontroller at delt [datamaskinaktivering er aktivert for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

