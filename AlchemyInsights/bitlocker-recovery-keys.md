---
title: Bitlocker-gjenopprettingsnøkler
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820295"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Få tilgang til Bitlocker-gjenopprettingsnøkler

Når du konfigurerer Bitlocker-innstillinger Intune Endpoint Protection Policy, er det mulig å definere om Bitlocker-gjenopprettingsinformasjon skal lagres i Azure Active Directory.

Hvis denne innstillingen er konfigurert, skal de lagrede gjenopprettingsdataene være synlige for en Intune-administrator som en del av datainnspillingen for enheten i Intune Devices-bladet på to måter:

Enheter – Azure AD-enheter – > «Enhet» ELLER Enheter – > Alle enheter – > «Enhet» -> Gjenopprettingsnøkler

Hvis det er administrativ tilgang til selve enheten, kan du eventuelt se gjenopprettingsnøkkelen (Passord) ved å kjøre følgende kommando fra en hevet ledetekst:

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
Hvis enheten ble kryptert før registreringen i Intune, kan gjenopprettingsnøkkelen ha blitt knyttet til Microsoft-kontoen (MSA) som ble brukt til å logge på enheten under OOBE-prosessen. Hvis dette var tilfellet, skal tilgang til og pålogging med MSA vise enhetene som  https://onedrive.live.com/recoverykey gjenopprettingsnøklene ble lagret for.
 
Hvis enheten ble kryptert som et resultat av konfigurasjonen via domenebasert gruppepolicy, kan gjenopprettingsinformasjonen lagres i den lokale Active Directory.

Hvis du har konfigurert policyen for endepunktbeskyttelse til å lagre gjenopprettingsnøkkelen i Azure Active Directory, men nøkkelen for en bestemt enhet ikke er lastet opp, kan du utløse opplastingen ved å rotere gjenopprettingsnøkkelen for denne enheten fra MEM-konsollen. Hvis du vil ha mer informasjon, kan du se [Roter BitLocker-gjenopprettingsnøkler](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

