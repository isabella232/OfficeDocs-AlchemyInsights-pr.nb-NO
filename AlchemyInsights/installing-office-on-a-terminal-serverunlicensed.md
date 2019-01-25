---
title: Installere office på en Terminal Server - ulisensiert
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29481805"
---
# <a name="installing-office-on-a-terminal-server"></a>Installere Office på en Terminal Server

For distribusjon av Office 365 ProPlus på en Windows-Server ved hjelp av Remote Desktop Services (RDS), tidligere kalt Terminal Services:
  
- Du må ha en Office 365-plan som inkluderer Office 365 ProPlus, for eksempel Office 365 Enterprise E3 eller Enterprise E5. Office 365 Business og Office 365 Business Premium planene inkluderer ikke Office 365 ProPlus.
    
- Du må aktivere [delt datamaskinaktivering](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Hvis du vil installere Office 365 ProPlus på RDS fra Office 365-portalen ** *som bruker standardinnstillingene for installasjonen* **, følger du denne fremgangsmåten: 
  
1. Se hva du har Office 365-planen. [Lære hvordan](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Hvis nødvendig, bytte til en annen Office 365-planer. [Lære hvordan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Hvis Office allerede er installert på RDS-serveren ved hjelp av andre Office 365-planer, kan du avinstallere den. For eksempel ved å gå til Kontrollpanel \> Avinstaller et program. Avinstaller ved hjelp av [Microsoft Kundestøtte og gjenoppretting-hjelperen](https://aka.ms/SARA-OfficeUninstall-Alchemy) Hvis du kjører i problemer. 
    
4. Logg på Office 365-portalen med administrator-kontoen og [installere Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)på RDS-serveren.
    
5. Etter at Office er installert, ** *ikke åpne eller logge deg på* ** til alle Office-programmer. 
    
6. På RDS-server, kan du aktivere delt datamaskinaktivering ved å redigere registret ved å følge disse trinnene:
    
1. Høyreklikk Windows-knappen nederst til venstre på skjermen og velg Kjør. Skriv inn **regedit**i Åpne-boksen, og velg deretter OK. 
    
2. Velg Ja når du blir bedt om å tillate Registerredigering til å gjøre endringer til enheten.
    
3. I Registerredigering, legge til en strengverdi på **SharedComputerLicensing** med innstillingen 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. På RDS-server ** *Logg på som en sluttbruker* ** og [Kontroller at delt datamaskinaktivering er aktivert for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Hvis du vil ha mer informasjon om forutsetninger, installasjonsinstruksjoner og veiledning om tilpassede installasjoner ved hjelp av verktøyet for distribusjon av Office, kan du se [Distribuere Office 365 ProPlus ved hjelp av Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Hvis du vil rette opp feil i forbindelse med aktivering av delt datamaskin, kan du se [Feilsøke problemer med delt datamaskin aktiveringsveiviseren for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

