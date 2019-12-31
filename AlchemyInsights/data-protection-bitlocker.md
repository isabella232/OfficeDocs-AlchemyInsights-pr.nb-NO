---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908718"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivere BitLocker-kryptering med Intune

 Policyen for sluttpunktbeskyttelse for Intune kan brukes til å konfigurere BitLocker-krypteringsinnstillinger for Windows-enheter. Hvis du vil ha mer informasjon, kan [du se Windows 10 (og senere) innstillinger for å beskytte enheter ved hjelp av Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Du bør være oppmerksom på at mange nyere enheter som kjører Windows 10 støtter automatisk BitLocker-kryptering, som utløses uten bruk av MDM-policy. Dette kan påvirke bruken av policy hvis ikke-standardinnstillinger er konfigurert. Se følgende vanlige spørsmål for flere detaljer.
 
Hvis du vil ha informasjon om feilsøking av BitLocker-problemer, kan du se [Feilsøke BitLocker policyer i Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Vanlige spørsmål**

 Spørsmål: hvilke versjoner av Windows støtter Enhetskryptering ved å bruke policyen for sluttpunktbeskyttelse?<br>
 A: innstillingene i Intune Endpoint Protection policy implementeres ved hjelp av [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Ikke alle utgaver eller versjoner av Windows støtter BitLocker CSP. <br><br>
      På dette tidspunktet støttes følgende Windows-utgaver: Enterprise, Education, Mobile, mobile Enterprise og Professional (Build 1809 og senere).
 
Q: Hvis en enhet er allerede kryptert med BitLocker bruker OS standardinnstillingene for krypteringsmetode og Cipher styrke (XTS-AES-128), vil bruke en policy med ulike innstillinger automatisk utløse re-kryptering av stasjonen med de nye innstillingene?<br>
A: Nei. Hvis du vil bruke de nye Cipher innstillingene, må stasjonen først dekrypteres.<br><br>
**Merk:** For enheter som registreres med autopilot, utløses ikke den automatiske krypteringen som oppstår under OOBE, før Intune-policyen evalueres, noe som gjør at policy-baserte-innstillingene kan brukes i stedet for operativsystem standardene.
 
Spørsmål: Hvis en enhet er kryptert som et resultat av bruken av Intune-policy, vil den bli dekryptert når denne policyen fjernes?<br>
A: fjerning av krypterings relatert policy fører ikke til dekryptering av stasjonene som ble konfigurert.
 
Spørsmål: Hvorfor viser Samsvars policyen for Intune at enheten ikke har BitLocker aktivert, selv om den er det?<br>
A: "BitLocker aktivert"-innstillingen i retningslinjene for overholdelse av Intune bruker Windows Device Health-klienten (DHA). Denne klienten måler bare Enhetsstatus ved oppstart. Så hvis en enhet ikke er startet på nytt siden BitLocker-krypteringen ble fullført, vil ikke DHA-klienttjenesten rapportere BitLocker som aktiv.
 
 