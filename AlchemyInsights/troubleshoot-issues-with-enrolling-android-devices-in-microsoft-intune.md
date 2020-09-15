---
title: Feilsøke problemer med registrering av Android-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689963"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Feilsøke problemer med registrering av Android-enheter i Microsoft Intune

Se gjennom ressursene som er oppført nedenfor, for å løse problemet nå.
  
Noen vanlige problemer og løsnings trinn:
  
 **Enhet ikke kryptert-feil i firma portalen:** Nyere versjoner av Android, spesielt fra og med v 7.0, krever et oppstarts passord for å sikre at enheten er helt kryptert. Vanlige løsninger er å aktivere en oppstarts-PIN-kode eller kryptere enheten fullstendig. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for mer informasjon.
  
 **Enheter kan ikke sjekke inn med Intune-tjenesten eller vise som "inhealth" i administrasjons konsollen for Intune:** Enkelte Samsung 4,4-og 5,5-enheter kan kanskje ikke sjekke inn tjenesten. Det er tre mulige løsninger på dette problemet:
  
1. Åpne Intune Company Portal-appen manuelt, som automatisk vil starte en enhets synkronisering.

2. Oppdater enheten til Android 6,0 eller nyere.

3. Deaktivere Samsung smart Manager fra administrasjon av Intune Company Portal. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for mer informasjon om disse problemene og løsningene.

 **Bruker lisens typen er ugyldig** eller **bruker navnet er ukjent feil:** brukeren må tilordnes en Intune-eller EMS-lisens. Se gjennom disse dokumentene for å tilordne en lisens gjennom: Office Admin Center eller Azure Portal.
  
Flere ressurser som kan hjelpe deg med å løse problemet:
  
1. Bruk [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registrerings feil. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.

2. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for en liste over vanlige feil som forhindrer registrering og løsninger på hver av dem.

3. [Lær hvordan du registrerer Android-enheter i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
