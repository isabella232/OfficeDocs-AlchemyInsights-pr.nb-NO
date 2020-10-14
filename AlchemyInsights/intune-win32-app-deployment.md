---
title: Distribusjon av Intune Win32-apper
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461874"
---
# <a name="intune-win32-app-deployment"></a>Distribusjon av Intune Win32-apper

Microsoft Intune tillater Win32-programmer, inkludert, men ikke begrenset til MSI og. EXE skal distribueres til Windows 10-enheter. Den brukte distribusjons mekanismen krever at Intune Management Extension (IME) er tilgjengelig på målenheten. IME vil bli installert automatisk som et resultat av å identifisere et PowerShell-skript eller en Win32-program distribusjon til en bruker/enhet.

Det finnes også et sett med forhånds krav som må oppfylles for å kunne distribuere Win32-apper som omfatter:

- Støttede plattformer: Windows 10 versjon 1607 eller nyere (Enterprise-, Pro-og Education-versjoner).
- Arkitektur som støttes: x86 og x64.
- Enhets behandling: AAD-koblet og automatisk registrert (inkludert hybrid domene som er sammenføyd og automatisk registrert for gruppe policy).
- Format for program pakke:. **intunewin**  -fil som er klargjort av [verktøyet Microsoft Win32 Content forberedelser](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Sine
    - Maksimums størrelse: 8 GB.
    - Arkitektur som ikke støttes: armer.

Se gjennom dokumentet «[Legg til, tilordne og Overvåk en Win32-app i Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)» for informasjon som er relatert til disse trinnene.

Detaljer om feil søking av program distribusjon på Windows, inkludert Win32-apper kan gjennomgås i følgende dokumenter

- [Feilsøke problemer med installasjon av apper](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Feilsøke Win32-apper](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)