---
title: Feilsøke problemer med å registrere Android-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759629"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Feilsøke problemer med å registrere Android-enheter i Microsoft Intune

Se gjennom ressursene som er oppført nedenfor for å løse problemet nå.
  
Noen vanlige problemer og løsningstrinn:
  
 **Enheten ikke kryptert feil i Firmaportal:** Nyere versjoner av Android, spesielt fra og med v7.0, krever et oppstartspassord for å sikre at enheten din er fullstendig kryptert. Vanlige løsninger er å aktivere en oppstartspinne eller kryptere enheten helt. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) hvis du vil ha mer informasjon.
  
 **Enheter kan ikke sjekke inn med Intune-tjenesten eller vise som "Usunn" i Intune admin-konsollen:** Noen Samsung 4.4- og 5.5-enheter kan ikke sjekke inn i tjenesten. Det finnes 3 mulige løsninger på dette problemet:
  
1. Åpne Intune Company Portal-appen manuelt, som automatisk starter en enhetssynkronisering.

2. Oppdater enheten til Android 6.0 eller nyere.

3. Deaktiver Samsung Smart Manager fra å administrere Intune Company Portal. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for mer informasjon om disse problemene og løsningene.

 **Brukerlisenstype Ugyldig** eller **Brukernavn gjenkjennes ikke feil:** Brukeren må tilordnes en Intune- eller EMS-lisens. Se gjennom disse dokumentene for å tilordne en lisens via: Administrasjonssenter for Office eller Azure-portalen.
  
Flere ressurser som kan løse problemet:
  
1. Bruk [Intune Feilsøking Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registreringsfeil. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) hvis du vil ha mer informasjon.

2. Se gjennom [dette dokumentet](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for en liste over vanlige feil som hindrer registrering og oppløsning er til hver av dem.

3. [Finn ut hvordan du registrerer Android-enheter i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
