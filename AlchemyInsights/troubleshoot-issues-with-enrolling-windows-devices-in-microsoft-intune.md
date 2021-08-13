---
title: Feilsøke problemer med å registrere Windows enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981050"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Feilsøke problemer med å registrere Windows enheter i Microsoft Intune

Se gjennom ressursene som er oppført nedenfor, for å løse problemet nå.
  
Noen vanlige feilmeldinger og løsningstrinn:
  
 **Programvaren kan ikke installeres, 0x80cf4017:** Kontosertifikatet er utløpt. Last ned PC Client-programvarepakken på nytt i administrasjonskonsollen for Intune. Se gjennom denne dokumentasjonen for mer informasjon.
  
 **Feilkode 0x801c0003:** Feilen kan oppstå i følgende scenarier:
  
-  Brukeren har flere enheter registrert enn enhetsgrensen. Se gjennom disse dokumentene for [å fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) eller endre [enhetsgrensen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  «Brukere kan bli med i enheter til Azure AD» er satt til «ingen». Angi den til alle, eller velg brukere. Se [gjennom denne dokumentasjonen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for mer informasjon.

-  Enheten er allerede registrert av en annen bruker. Hvis det er tilfellet, må du fjerne enheten fra Azure Intune-konsollen eller manuelt oppheve registreringen av enheten før du prøver på nytt.

-  Enheten er Windows 10 Home. Bare Windows 10 Pro, utdanning og enterprise SKUs kan bli med Azure Active Directory.

Flere ressurser for å løse problemet:
  
-  Bruk [Feilsøkingsportalen for Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registreringsfeil. Se [gjennom dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.

-  Se gjennom disse dokumentene for en liste over vanlige feil som hindrer registrering og løsninger for hver av dem: [Feilsøkingsveiledning](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [Feilsøking av dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Lær hvordan du kan registrere Windows enheter i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
