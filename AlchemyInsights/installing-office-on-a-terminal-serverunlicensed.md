---
title: Installere Office på en Terminal Server-ulisensiert
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/15/2019
ms.locfileid: "37205418"
---
# <a name="installing-office-on-a-terminal-server"></a>Installere Office på en terminalserver

For distribusjon av Office 365 ProPlus på en Windows Server ved hjelp av Remote Desktop Services (RDS), tidligere kalt Terminal Services:
  
- Du må ha en plan for Office 365 som inkluderer Office 365 ProPlus, for eksempel Office 365 Enterprise E3 eller Enterprise E5. Office 365 Business og Office 365 Business Premium-abonnementer inkluderer ikke Office 365 ProPlus.

- Du må aktivere [aktivering av delt datamaskin](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Hvis du vil installere Office 365 ProPlus på RDS fra administrasjonssenteret for Microsoft 365, ***som bruker standard installasjonsinnstillinger***, bruker du følgende fremgangsmåte.

> [!TIP]
> Du kan også laste ned og kjøre [Microsoft Kundestøtte og gjenoppretting Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) for å installere Office 365 ProPlus i aktiverings modus for delt datamaskin.
  
1. Sjekk hvilken Office 365 plan du har. [Finn ut hvordan](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Bytt om nødvendig til en annen plan i Office-365. [Finn ut hvordan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Hvis Office allerede er installert på RDS-serveren ved hjelp av andre Office 365-planer, avinstallerer du det. For eksempel ved å gå til kontroll panel \> Avinstaller et program. Avinstaller ved hjelp av [Microsoft Kundestøtte og gjenoppretting Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du kjører i problemer.

4. På RDS-serveren logger du på administrasjonssenteret for Microsoft 365 med administratorkontoen og [installerer Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Når Office er installert, må du ***ikke åpne eller logge på*** noen Office-programmer.

6. Aktiver aktivering av delt datamaskin ved å redigere registret på RDS-serveren ved å følge disse trinnene:

1. Høyreklikk Windows-knappen nederst til venstre på skjermen, og velg Kjør. I åpne-boksen skriver du inn **regedit**, og deretter velger du OK.

2. Velg Ja når du blir bedt om å tillate Registerredigering å gjøre endringer på enheten.

3. I Registerredigering legger du til en strengverdi på **SharedComputerLicensing** med en innstilling på 1 under HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.

7. Logg på RDS-serveren ***som sluttbruker*** , og [Kontroller at aktivering av delt datamaskin er aktivert for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Hvis du vil ha mer informasjon om forutsetninger, installasjonsinstruksjoner og veiledning om tilpassede installasjoner ved hjelp av Office Deployment Tool, kan du se [distribuere Office 365 ProPlus ved hjelp av Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Hvis du vil rette feil relatert til aktivering av delt datamaskin, kan du se [Feilsøke problemer med delt datamaskinaktivering for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  