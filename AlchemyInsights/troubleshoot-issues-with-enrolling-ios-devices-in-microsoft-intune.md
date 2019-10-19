---
title: Feilsøk problemer med registrering av iOS-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507012"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Feilsøk problemer med registrering av iOS-enheter i Microsoft Intune

Se gjennom ressursene som er oppført nedenfor, for å løse problemet nå. 
  
Noen vanlige feilmeldinger og løsningstrinn:
  
- **Enhet cap nådd** Brukeren har flere enheter registrert enn enhetsgrensen. Se gjennom disse dokumentene for å [fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [endre enhetens grense](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Denne tjenesten støttes ikke. Ingen registrerings policy:** Apple Push Notification Service (APNS) må konfigureres eller fornyes. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instruksjoner om hvordan du gjør dette. 
    
- **Brukerlisens type ugyldig eller brukernavn gjenkjennes ikke:** Brukeren må tilordnes en Intune-eller EMS-lisens. Se gjennom disse dokumentene for å tilordne en lisens via: [Office Administrasjonssenter](https://docs.microsoft.com/intune/licenses-assign) eller [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Flere ressurser som kan hjelpe deg med å løse problemet:
  
1. Bruk [feilsøkings portalen for Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registreringsfeil. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon. 
    
2. Se gjennom disse dokumentene for en liste over vanlige feil som forhindrer registrering og løsninger for hver: [feilsøkingsveiledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [feilsøking av dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Finn ut hvordan du registrerer IOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

