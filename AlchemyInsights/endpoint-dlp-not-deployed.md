---
title: Endepunkt-DLP ikke distribuert til brukerens enhet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731590"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>Endepunkt-DLP ikke distribuert til brukerens enhet

Hvis DLP-innstillingen (Endpoint Data Loss Prevention) ikke er brukt på en brukers enhet, må du bekrefte at du oppfyller disse kravene:

- Windows 10 x64 bygg 1809 eller nyere er installert på enheten.
- Klientversjon 4.18.2009.7 eller nyere for skadelig programvare er installert.
- Enheten er **en av** disse:
    
    - Azure Active Directory (Azure AD) ble med
    - Hybrid Azure AD ble med
    - AAD registrert

- Hvis du vil gjennomføre policyhandlinger, må du kontrollere at Microsoft Chromium Edge-nettleseren er installert på endepunktenheten.

Hvis du vil ha flere krav til distribusjon av endepunkt-DLP, kan du se Komme i gang med hindring av tap [av endepunktdata.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)