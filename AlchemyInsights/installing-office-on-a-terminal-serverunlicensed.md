---
title: Installere office på en terminalserver – ulisensiert
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
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322008"
---
# <a name="installing-office-on-a-terminal-server"></a>Installere Office på en Terminal Server

For distribuering Microsoft 365 Apps for enterprise på en Windows server ved hjelp av Remote Desktop Services (RDS), tidligere kalt Terminal Services:
  
- Du må ha et Microsoft 365 abonnement som inneholder Microsoft 365 Apps for enterprise, for eksempel Office 365 Enterprise E3 eller Enterprise E5. Planene Microsoft 365 Apps for business og Microsoft 365 Apps for business Premium inkluderer ikke Microsoft 365 Apps for enterprise.

- Du må aktivere [aktivering av delt datamaskin](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Hvis du vil installere Microsoft 365 Apps for enterprise på RDS fra ***Administrasjonssenter for Microsoft 365,*** som bruker standard installasjonsinnstillinger, bruker du fremgangsmåten nedenfor.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Se hva Microsoft 365 abonnementet du har. [Finn ut hvordan](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Bytt om nødvendig til et annet Microsoft 365 abonnement. [Finn ut hvordan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Hvis Office allerede er installert på RDS-serveren ved hjelp av andre Microsoft 365 abonnementer, må du avinstallere det. Du kan for eksempel gå til Avinstallere et program i \> kontrollpanelet. Avinstaller ved [hjelp av Microsoft assistent for støtte og gjenoppretting](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis det er problemer.

4. På RDS-serveren logger du på Administrasjonssenter for Microsoft 365 med administratorkontoen og [installerer Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. Når Office er installert, må du ikke åpne eller ***logge*** på noen Office programmer.

6. Aktiver aktivering av delt datamaskin på RDS-serveren ved å redigere registeret ved å følge disse trinnene:

1. Høyreklikk på Windows nederst til venstre på skjermen, og velg Kjør. Skriv inn regedit i **Åpne-boksen,** og velg deretter OK.

2. Velg Ja når du blir bedt om å tillate at Registerredigering gjør endringer på enheten.

3. Legg til en strengverdi for **SharedComputerLicensing** i Registerredigering med innstillingen 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Logg på som sluttbruker  på RDS-serveren, og kontroller at aktivering av delt datamaskin [er aktivert for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Hvis du vil ha mer informasjon om forutsetninger, installasjonsinstruksjoner og veiledning om tilpassede installasjoner ved hjelp av Office-distribusjonsverktøyet, kan du se Distribuere Microsoft 365 Apps for enterprise ved hjelp av [Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Hvis du vil løse feil relatert til aktivering av delt datamaskin, kan du se Feilsøke problemer med aktivering av delt [datamaskin for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  