---
title: Installere office på en Terminal Server - Ulisensiert
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
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508637"
---
# <a name="installing-office-on-a-terminal-server"></a>Installere Office på en Terminal Server

For distribusjon av Microsoft 365 Apps for enterprise på en Windows Server ved hjelp av Remote Desktop Services (RDS), tidligere kalt Terminal Services:
  
- Du må ha et Microsoft 365-abonnement som inkluderer Microsoft 365 Apps for enterprise, for eksempel Office 365 Enterprise E3 eller Enterprise E5. Microsoft 365 Apps for bedrifter og Microsoft 365 Apps for business Premium-abonnementer inkluderer ikke Microsoft 365 Apps for enterprise.

- Du må aktivere aktivering av [delt datamaskin](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Hvis du vil installere Microsoft 365 Apps for enterprise på RDS fra administrasjonssenteret for Microsoft 365, ***som bruker standard installasjonsinnstillinger***, kan du bruke følgende fremgangsmåte.

> [!TIP]
> Du kan også laste ned og kjøre [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) for å installere Microsoft 365 Apps for enterprise i aktiveringsmodus for delt datamaskin.
  
1. Sjekk hva Microsoft 365-abonnementet du har. [Finn ut hvordan](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Bytt om nødvendig til et annet Microsoft 365-abonnement. [Finn ut hvordan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Hvis Office allerede er installert på RDS-serveren ved hjelp av andre Microsoft 365-abonnementer, må du avinstallere den. For eksempel, ved å gå til Kontrollpanel \> Avinstaller et program. Avinstaller ved hjelp av [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du støter på problemer.

4. Logg på administrasjonssenteret for Microsoft 365 med administratorkontoen på RDS-serveren, og [installer Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. Når Office er installert, ***må du ikke åpne eller logge på*** office-programmer.

6. Aktiver aktivering av delt datamaskin på RDS-serveren ved å redigere registret ved å følge disse trinnene:

1. Høyreklikk Windows-knappen nederst til venstre på skjermen, og velg Kjør. Skriv inn **regedit**i Åpne-boksen, og velg deretter OK.

2. Velg Ja når du blir bedt om å tillate at Registerredigering gjør endringer på enheten.

3. I Registerredigering legger du til en strengverdi for **SharedComputerLicensing** med en innstilling på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Logg på som ***sluttbruker*** på RDS-serveren, og kontroller at aktivering av [delt datamaskin er aktivert for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Hvis du vil ha mer informasjon om forutsetninger, installasjonsinstruksjoner og veiledning om tilpassede installasjoner ved hjelp av Office Deployment Tool, kan du se [Distribuere Microsoft 365 Apps for enterprise ved hjelp av Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Hvis du vil rette feil relatert til aktivering av delt datamaskin, kan du se [Feilsøke problemer med aktivering av delt datamaskin for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  