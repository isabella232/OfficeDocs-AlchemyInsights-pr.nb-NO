---
title: Feilsøke problemer med registrering av iOS-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708971"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Feilsøke problemer med registrering av iOS-enheter i Microsoft Intune

Se gjennom ressursene som er oppført nedenfor for å løse problemet nå. 
  
Noen vanlige feilmeldinger og løsningstrinn:
  
- **Enhetsgrense nådd** Brukeren har flere enheter registrert enn enhetsgrensen. Se gjennom disse dokumentene [for å fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) eller endre [enhetsgrensen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Denne tjenesten støttes ikke. Ingen registreringspolicy:** Apple Push Notification Service (APNS) må konfigureres eller fornyes. Se [gjennom dette dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instruksjoner om hvordan du gjør dette. 
    
- **Brukerlisenstype ugyldig eller brukernavn gjenkjennes ikke:** Brukeren må tildeles en Intune- eller EMS-lisens. Se gjennom disse dokumentene for å tilordne en lisens via [administrasjonssenteret for Office eller](https://docs.microsoft.com/intune/licenses-assign) [Azure Portal.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Flere ressurser som kan hjelpe deg med å løse problemet:
  
1. Bruk [feilsøkingsportalen for Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registreringsfeil. Se [gjennom dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon. 
    
2. Se gjennom disse dokumentene for å få en liste over vanlige feil som hindrer registrering og løsninger for hver av [dem:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) Feilsøkingsveiledning og [Feilsøking av dokumenter.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Finn ut hvordan du registrere iOS-enheter i Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

