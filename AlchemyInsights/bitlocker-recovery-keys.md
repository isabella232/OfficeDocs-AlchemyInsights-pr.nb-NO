---
title: BitLocker-gjenopprettings nøkler
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685895"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Få tilgang til BitLocker-gjenopprettings nøklene

Når du konfigurerer BitLocker-innstillinger Intune Endpoint Protection-policyen, kan du definere om BitLocker-gjenopprettingsinformasjon skal lagres i Azure Active Directory.

Hvis denne innstillingen er konfigurert, skal lagrede gjenopprettings data være synlige for en Intune-administrator som en del av enhets post dataene i Intune-enheter blad på to måter:

Enheter – Azure AD-enheter – > "enhet" eller enheter-> alle enheter-> "enhet" – > gjenopprettings nøkler

Hvis det er administrator tilgang til selve enheten, kan du eventuelt se gjenopprettings nøkkelen (passord) ved å kjøre følgende kommando fra en hevet lede tekst:

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
Hvis enheten ble kryptert før enrolment i Intune, kan gjenopprettings nøkkelen ha blitt tilknyttet "Microsoft-kontoen" (MSA) som brukes til å logge på enheten under OOBE-prosessen. Hvis dette var tilfelle, kan du få tilgang til  https://onedrive.live.com/recoverykey og logge på med denne MSA for å vise enhetene som gjenopprettings nøklene ble lagret i.
 
Hvis enheten ble kryptert som et resultat av konfigurasjon via domene BAS ert gruppe policy, kan gjenopprettings informasjonen være lagret i den lokale Active Directory.
 

