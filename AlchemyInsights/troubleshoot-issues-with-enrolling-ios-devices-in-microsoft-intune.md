---
title: Feilsøke problemer med registrering av iOS-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736167"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Feilsøke problemer med registrering av iOS-enheter i Microsoft Intune

Se gjennom ressursene som er oppført nedenfor for å løse problemet nå. 
  
Noen vanlige feilmeldinger og løsningstrinn:
  
- **Enhetsdeksel nådd** Brukeren har flere enheter som er registrert enn enhetsgrensen. Se gjennom disse dokumentene for å [fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) eller endre [enhetsgrensen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Denne tjenesten støttes ikke. Ingen registreringsregler:** Apple Push Notification Service (APNS) må konfigureres eller fornyes. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instruksjoner om hvordan du gjør det. 
    
- **Brukerlisenstype ugyldig eller brukernavn gjenkjennes ikke:** Brukeren må tilordnes en Intune- eller EMS-lisens. Se gjennom disse dokumentene for å tilordne en lisens via: [Administrasjonssenter for Office](https://docs.microsoft.com/intune/licenses-assign) eller [Azure-portalen](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Flere ressurser som kan løse problemet:
  
1. Bruk [Intune Feilsøking Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registreringsfeil. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) hvis du vil ha mer informasjon. 
    
2. Se gjennom disse dokumentene for en liste over vanlige feil som hindrer registrering og oppløsning til hver: [Feilsøkingsveiledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [feilsøkingsdokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Lær hvordan du registrerer iOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

