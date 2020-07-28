---
title: Kontrollere automatiske oppdateringer for Office Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439931"
---
# <a name="control-automatic-updates-for-office-apps"></a>Kontrollere automatiske oppdateringer for Office Apps

Som standard lastes oppdateringer for Office Apps ned automatisk og brukes i bakgrunnen uten brukermedvirkning. Administratorer kan imidlertid kontrollere hvordan oppdateringer brukes ved hjelp av Office Update-innstillinger. Oppdateringsinnstillinger gjør det mulig for administratorer å aktivere eller deaktivere automatiske oppdateringer, vise eller skjule **Oppdater nå-knappen** i Office, angi oppdateringsfrister og mer. Hvis du vil ha detaljert informasjon, kan du se:

- [Konfigurere oppdateringsinnstillinger for Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatisk oppdatering for Office er ikke aktivert](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definere hvordan Office oppdateres etter at det er installert](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Hvis du vil se gjennom de eksisterende oppdateringsinnstillingene som brukes på en klientmaskin, gjør du følgende:

1. Åpne Registerredigering ved å gå til **Start**  >  **Kjør**  >  **regedit**.
2. Bytt til følgende plassering, og se gjennom Office Update-innstillingene:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. KlikkToRun\Konfigurasjon

**Merk at**  Hvis OfficeMgmtCOM-nøkkelen er angitt, kan du se meldingen "Oppdateringer **Office**administreres av systemansvarlig" i  >  **Office-konto**  >  **Office-oppdateringer**. Hvis du vil ha mer informasjon, kan du se [Administrere oppdateringer for Microsoft 365-apper med Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  