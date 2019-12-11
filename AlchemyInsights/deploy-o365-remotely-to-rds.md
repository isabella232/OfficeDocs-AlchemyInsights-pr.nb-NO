---
title: Distribuere Office 365 ProPlus for delt bruk på RDS, Terminal Server eller VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959468"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Distribuere Office 365 ProPlus for delt bruk på RDS, Terminal Server eller VDI

Slik distribuerer du Office 365 ProPlus ved hjelp av Remote Desktop Services (RDS), tidligere kalt Terminal Services:
- Du må ha en Microsoft 365 for forretningsplan eller en Office 365-plan som inkluderer Office 365 ProPlus, for eksempel Office 365 Enterprise E3 eller Enterprise E5.
   > [!NOTE] 
   > Office 365 Business og Office 365 Business Premium-abonnementer inkluderer ikke Office 365 ProPlus.
- Du må aktivere [aktivering av delt datamaskin](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Du kan også laste ned og kjøre [Microsoft Kundestøtte og gjenoppretting Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) for å installere Office 365 ProPlus i aktiverings modus for delt datamaskin.

Hvis du vil ha mer informasjon om forutsetninger, oppsettsinstruksjoner og veiledning om tilpassede installasjoner ved hjelp av distribusjonsverktøyet for Office, kan du se [distribuere office 365 ProPlus ved hjelp av Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Slik retter du feil relatert til aktivering av delt datamaskin:
- Se [Feilsøke problemer med aktivering av delt datamaskin for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Se [tilbakestille aktiveringsstatusen for Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).

Hvis du vil installere Office 365 ProPlus på RDS fra administrasjonssenteret for Microsoft 365, ***som bruker standard installasjonsinnstillinger***, bruker du følgende fremgangsmåte:

1.  Sjekk hvilken Office 365 plan du har. [Finn ut hvordan](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Bytt om nødvendig til en annen plan i Office-365. [Finn ut hvordan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Hvis Office allerede er installert på RDS-serveren ved hjelp av andre Office 365-planer, avinstallerer du det. For eksempel ved å gå til **kontroll panel** > **avinstallere et program**. Avinstaller ved hjelp av [Microsoft Kundestøtte og gjenoppretting Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du kjører i problemer.
4.  På RDS-serveren logger du på administrasjonssenteret for Microsoft 365 med administratorkontoen og [installerer Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Når Office er installert, må du ***ikke åpne eller logge på*** noen Office-programmer.
6.  Aktiver aktivering av delt datamaskin ved å redigere registret på RDS-serveren ved å følge disse trinnene:
   1. Høyreklikk Windows-knappen nederst til venstre på skjermen, og velg **Kjør**. I åpne-boksen skriver du inn **regedit**, og deretter velger du **OK**.
   2. Velg **Yes (ja** ) når du blir spurt om du vil tillate at Registerredigering gjør endringer på enheten.
   3. I Registerredigering legger du til en strengverdi på **SharedComputerLicensing** med en innstilling på 1 under HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.
   4. Logg på RDS-serveren ***som sluttbruker*** , og [Kontroller at aktivering av delt datamaskin er aktivert for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

