---
title: Installere Office på en Terminal Server – ulisensiert
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663126"
---
# <a name="installing-office-on-a-terminal-server"></a>Installere Office på en terminalserver

For distribusjon av Microsoft 365-apper for bedrifter på en Windows-Server ved hjelp av Remote Desktop Services (RDS), tidligere kalt Terminal Services:
  
- Du må ha et Microsoft 365-abonnement som inkluderer Microsoft 365-apper for Enterprise, for eksempel Office 365 Enterprise E3 eller Enterprise E5. Microsoft 365-appene for Business-og Microsoft 365-apper for Business Premium-planer inkluderer ikke Microsoft 365-apper for Enterprise.

- Du må aktivere [aktivering av delt data maskin](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Hvis du vil installere Microsoft 365-apper for Enterprise på RDS fra administrasjons senteret for Microsoft 365, ***som bruker standard installasjons innstillinger***, følger du Fremgangs måten nedenfor.

> [!TIP]
> Du kan også laste ned og kjøre [Microsoft-assistenten for støtte og gjenoppretting](https://aka.ms/SaRA_OfficeSCA_M365Portal) for å installere Microsoft 365-apper for Enterprise i den delte data maskinens aktiverings modus.
  
1. Kontroller hvilket Microsoft 365-abonnement du har. [Finn ut hvordan](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Bytt om nødvendig til et annet Microsoft 365-abonnement. [Finn ut hvordan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Hvis Office allerede er installert på RDS-serveren ved hjelp av andre Microsoft 365-abonnementer, må du avinstallere det. Ved å gå til kontroll panel, må du for eksempel \> avinstallere et program. Avinstaller ved hjelp av [Microsoft kunde støtte og gjenopprettings assistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du har problemer.

4. På RDS-serveren logger du deg på administrasjons senteret for Microsoft 365 med administrator kontoen din og [installerer Microsoft 365-apper for Enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. Når Office er installert, kan du ***ikke åpne eller logge på*** noen Office-programmer.

6. Aktiver en delt data maskin aktivering på RDS-serveren ved å redigere registret ved å følge disse trinnene:

1. Høyre klikk Windows-knappen i nedre venstre hjørne av skjermen, og velg Kjør. Skriv inn **regedit**i åpne-boksen, og velg deretter OK.

2. Velg Ja når du blir bedt om å tillate register redigering for å gjøre endringer på enheten.

3. I register redigering legger du til en streng verdi på **SharedComputerLicensing** med en innstilling på 1 under HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.

7. ***Logg på som en slutt bruker*** på RDS-serveren, og [Kontroller at den delte data maskin aktiveringen er aktivert for Microsoft 365-apper for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Hvis du vil ha mer informasjon om forutsetninger, konfigurasjons instruksjoner og veiledning om tilpassede installasjoner ved hjelp av Office Deployment Tool, kan du se [distribuere Microsoft 365-apper for Enterprise ved hjelp av Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Hvis du vil løse feil relatert til aktivering av delt data maskin, kan du se [Feilsøke problemer med aktivering av delt data maskin for Microsoft 365-apper for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  