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
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669257"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Feilsøke problemer med registrering av iOS-enheter i Microsoft Intune

Se gjennom ressursene som er oppført nedenfor, for å løse problemet nå. 
  
Noen vanlige feil meldinger og løsnings trinn:
  
- **Enhetens ende** punkt er nådd Brukeren har flere enheter som ble registrert enn enhets grensen. Se gjennom disse dokumentene for å [fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [endre enhets grensen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Denne tjenesten støttes ikke. Ingen registrerings policy:** Apple Push Notification-tjeneste (APNS) må konfigureres eller fornyes. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instruksjoner om hvordan du gjør dette. 
    
- **Bruker lisens typen er ugyldig eller bruker navnet gjenkjennes ikke:** Brukeren må være tilordnet en Intune-eller EMS-lisens. Se gjennom disse dokumentene for å tilordne en lisens gjennom: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) eller [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Flere ressurser som kan hjelpe deg med å løse problemet:
  
1. Bruk [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registrerings feil. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon. 
    
2. Se gjennom disse dokumentene for en liste over vanlige feil som forhindrer registrering og løsninger på hver av dem: [feil søkings veiledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [feil søkings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Lær hvordan du registrerer IOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

