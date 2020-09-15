---
title: Feilsøke problemer med å registrere Windows-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658887"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Feilsøke problemer med å registrere Windows-enheter i Microsoft Intune

Se gjennom ressursene som er oppført nedenfor, for å løse problemet nå.
  
Noen vanlige feil meldinger og løsnings trinn:
  
 **Program varen kan ikke installeres, 0x80cf4017:** Konto sertifikatet er utløpt. Last ned program vare pakken for PC-klienten i administrasjons konsollen for Intune på nytt. Se gjennom denne dokumentasjonen for mer informasjon.
  
 **Feilkode 0x801c0003:** Feilen kan oppstå i følgende scenarioer:
  
-  Brukeren har flere enheter som ble registrert enn enhets grensen. Se gjennom disse dokumentene for å [fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [endre enhets grensen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  «Brukere kan bli med i enheter til Azure AD» er satt til ingen. Angi det til alle eller Velg brukere. Se gjennom [denne dokumentasjonen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for mer informasjon.

-  Enheten er allerede registrert av en annen bruker. Hvis det er tilfelle, fjerner du enheten fra Azure Intune-konsollen eller avregistrerer enheten manuelt før du prøver på nytt.

-  Enheten er Windows 10 Home. Bare Windows 10 Pro, Education og Enterprise SKU-er kan bli med i Azure Active Directory.

Flere ressurser som kan hjelpe deg med å løse problemet:
  
-  Bruk [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registrerings feil. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.

-  Se gjennom disse dokumentene for en liste over vanlige feil som forhindrer registrering og løsninger på hver av dem: [feil søkings veiledning](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [feil søkings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Lær hvordan du registrerer Windows-enheter i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
