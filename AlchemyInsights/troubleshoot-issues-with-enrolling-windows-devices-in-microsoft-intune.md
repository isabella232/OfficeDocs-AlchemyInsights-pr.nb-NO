---
title: Feilsøke problemer med å registrere Windows-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665841"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Feilsøke problemer med å registrere Windows-enheter i Microsoft Intune

Se gjennom ressursene som er oppført nedenfor, for å løse problemet nå.
  
Noen vanlige feilmeldinger og løsningstrinn:
  
 **Programvaren kan ikke installeres, 0x80cf4017:** Konto sertifikatet er utløpt. Last ned programvarepakken for PC-klienten på nytt i administrasjonskonsollen for Intune. Se gjennom denne dokumentasjonen for mer informasjon.
  
 **Feilkode 0x801c0003:** Feilen kan oppstå i følgende scenarier:
  
-  Brukeren har flere enheter registrert enn enhetsgrensen. Se gjennom disse dokumentene for å [fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [endre enhetens grense](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Brukere kan bli med enheter til Azure AD" er satt til "ingen". Sett den til alle eller Velg brukere. Se gjennom [denne dokumentasjonen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for mer informasjon.

-  Enheten er allerede registrert av en annen bruker. Hvis dette er tilfelle, fjerner du enheten fra Azure Intune-konsollen eller oppheve registreringen enheten manuelt før du prøver på nytt.

-  Enheten er Windows 10 Home. Bare Windows 10 Pro-, Education-og Enterprise-SKU-er kan bli med i Azure Active Directory.

Flere ressurser som kan hjelpe deg med å løse problemet:
  
-  Bruk [feilsøkings portalen for Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registreringsfeil. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.

-  Se gjennom disse dokumentene for en liste over vanlige feil som forhindrer registrering og løsninger for hver: [feilsøkingsveiledning](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [feilsøking av dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Lær hvordan du registrerer Windows-enheter i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
