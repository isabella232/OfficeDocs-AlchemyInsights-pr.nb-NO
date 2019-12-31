---
title: Gjenopprettingsnøkler for BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908823"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Tilgang til gjenopprettingsnøkler for BitLocker

Når du konfigurerer BitLocker-innstillinger Intune Endpoint Protection policy, er det mulig å definere om gjenopprettingsinformasjon for BitLocker skal lagres i Azure Active Directory.

Hvis denne innstillingen er konfigurert, skal de lagrede Gjenopprettingsdataene være synlige for en Intune-administrator som en del av enhets oppførings dataene i Intune Devices-blad på to måter:

Enheter-Azure AD-enheter-> "enhet" eller enheter-> alle enheter-> "enhet"-> gjenopprettings taster

Hvis det er administrativ tilgang til selve enheten, kan du eventuelt se gjenopprettingsnøkkelen (Password) ved å kjøre følgende kommando fra en hevet ledetekst:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Hvis enheten ble kryptert før registrering i Intune, kan gjenopprettingsnøkkelen være knyttet til "Microsoft Account" (MSA) som brukes til å logge på enheten under OOBE-prosessen. Hvis det var tilfelle, tilgang https://onedrive.live.com/recoverykey til og logge på med at MSA skal vise enhetene som gjenopprettingsnøkler ble lagret.
 
Hvis enheten ble kryptert som et resultat av konfigurasjon gjennom domenebasert gruppepolicy, kan gjenopprettingsinformasjonen lagres i den lokale Active Directory.
 

