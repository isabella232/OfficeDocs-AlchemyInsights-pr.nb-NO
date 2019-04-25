---
title: Feilsøke problemer med registrering av iOS enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391016"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Feilsøke problemer med registrering av iOS enheter i Microsoft Intune

Se gjennom ressursene som vises nedenfor for å løse problemet nå. 
  
Noen vanlige feilmeldinger og Løsningstrinn:
  
- **Enheten Cap nådd** Brukeren har flere enheter som er registrert enn enhetsgrensen. Se gjennom disse dokumentene for å [fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) , eller [Endre begrensningen for enheten](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Denne tjenesten støttes ikke. Ingen registreringspolicyen:** Apple Push Notification Service (APNER) må konfigureres eller fornyes. Gå gjennom [dette dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instruksjoner om hvordan du gjør dette. 
    
- **Ugyldig bruker-lisens eller brukernavnet gjenkjennes ikke:** Brukeren må være tilordnet en Intune eller EMS-lisens. Se gjennom disse dokumentene for å tilordne en lisens via: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) eller [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Ytterligere ressurser til å løse problemet:
  
1. Bruke [Intune feilsøking Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registrering-feil. Gå gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon. 
    
2. Se gjennom disse dokumentene for en liste over vanlige feil som hindrer registrering og løsninger for hver: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [feilsøking dok](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Lær hvordan du kan registrere iOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

