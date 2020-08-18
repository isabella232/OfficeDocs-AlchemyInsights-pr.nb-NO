---
title: Distribuere Microsoft 365-apper for bedrifter for delt bruk på RDS, Terminal Server eller VDI
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: bd30d99221e3ddd0b07db0db78009f346babd2d0
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786286"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Distribuere Microsoft 365-apper for bedrifter for delt bruk på RDS, Terminal Server eller VDI

Slik distribuerer du Microsoft 365-apper for bedrifter ved hjelp av Remote Desktop Services (RDS), tidligere kalt Terminal Services:
- Du må ha en Microsoft 365 for Business-plan eller en Office 365-plan som inkluderer Microsoft 365-apper for Enterprise, for eksempel Office 365 Enterprise E3 eller Enterprise E5.
   > [!NOTE] 
   > Microsoft 365-appene for Business og Microsoft 365 Business Premium standard plan inkluderer ikke Microsoft 365-apper for Enterprise.
- Du må aktivere [aktivering av delt data maskin](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Du kan også laste ned og kjøre [Microsoft-assistenten for støtte og gjenoppretting](https://aka.ms/SaRA_OfficeSCA_M365Portal) for å installere Microsoft 365-apper for Enterprise i den delte data maskinens aktiverings modus.

Hvis du vil ha mer informasjon om forutsetninger, oppsetts instruksjoner og veiledning for tilpassede installasjoner ved hjelp av distribusjons verktøy for Office, kan du se [distribuere Microsoft 365-apper for Enterprise ved hjelp av Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Slik retter du feil relatert til aktivering av delt data maskin:
- Se [Feilsøke problemer med aktivering av delt data maskin for Microsoft 365-apper for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Se [Tilbakestille Microsoft 365 Apps for enterprise for tilstand for organisasjonsaktivering](https://go.microsoft.com/fwlink/?linkid=2109218).

Hvis du vil installere Microsoft 365-apper for Enterprise på RDS fra administrasjons senteret for Microsoft 365, ***som bruker standard installasjons innstillinger***, bruker du følgende Fremgangs måte:

1.    Kontroller hvilket abonnement du har. [Finn ut hvordan](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Bytt om nødvendig til et annet abonnement. [Finn ut hvordan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Hvis Office allerede er installert på RDS-serveren ved hjelp av andre Microsoft-abonnementer, må du avinstallere det. Ved å gå til **kontroll panel**, må du for eksempel  >  **avinstallere et program**. Avinstaller ved hjelp av [Microsoft kunde støtte og gjenopprettings assistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du har problemer.
4.    På RDS-serveren logger du deg på administrasjons senteret for Microsoft 365 med administrator kontoen din og [installerer Microsoft 365-apper for Enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5.    Når Office er installert, kan du ***ikke åpne eller logge på*** noen Office-programmer.
6.    Aktiver en delt data maskin aktivering på RDS-serveren ved å redigere registret ved å følge disse trinnene:
   1. Høyre klikk Windows-knappen i nedre venstre hjørne av skjermen, og velg **Kjør**. Skriv inn **regedit**i åpne-boksen, og velg deretter **OK**.
   2. Velg **Ja** når du blir bedt om å tillate register redigering for å gjøre endringer på enheten.
   3. I register redigering legger du til en streng verdi på **SharedComputerLicensing** med en innstilling på 1 under HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.
   4. ***Logg på som en slutt bruker*** på RDS-serveren, og [Kontroller at den delte data maskin aktiveringen er aktivert for Microsoft 365-apper for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

