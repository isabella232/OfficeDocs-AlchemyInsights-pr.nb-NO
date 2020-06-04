---
title: Feilsøke problemer med registrering av Windows-enheter i Microsoft Intune
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
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665841"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Feilsøke problemer med registrering av Windows-enheter i Microsoft Intune

Se gjennom ressursene som er oppført nedenfor for å løse problemet nå.
  
Noen vanlige feilmeldinger og løsningstrinn:
  
 **Programvaren kan ikke installeres, 0x80cf4017:** Kontosertifikatet er utløpt. Last ned PC-klientprogramvarepakken på nytt i Intune Admin Console. Se gjennom denne dokumentasjonen hvis du vil ha mer informasjon.
  
 **Feilkode 0x801c0003:** Feilen kan oppstå i følgende scenarier:
  
-  Brukeren har flere enheter registrert enn enhetsgrensen. Se gjennom disse dokumentene for å [fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) eller endre [enhetsgrensen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Brukere kan koble enheter til Azure AD" er satt til "ingen". Sett den til alle, eller velg brukere. Se gjennom [denne dokumentasjonen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) hvis du vil ha mer informasjon.

-  Enheten er allerede registrert av en annen bruker. Hvis det er tilfelle, fjerner du enheten fra Azure Intune-konsollen eller manuelt fjerner enheten før du prøver på nytt.

-  Enheten er Windows 10 Home. Bare SKU-er for Windows 10 Pro, Utdanning og Bedrifter kan bli med i Azure Active Directory.

Flere ressurser for å løse problemet:
  
-  Bruk [Intune Feilsøkingsportal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registreringsfeil. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) hvis du vil ha mer informasjon.

-  Se gjennom disse dokumentene for en liste over vanlige feil som hindrer registrering og løsninger på hver: [Feilsøkingsveiledning](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [feilsøkingsdokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Lær hvordan du registrerer Windows-enheter i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
