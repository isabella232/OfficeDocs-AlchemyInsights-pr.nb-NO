---
title: DataProtection-BitLocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768826"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivere BitLocker-kryptering med Intune

 Policyen for Intune Endpoint Protection kan brukes til å konfigurere BitLocker-krypteringsnøkkel for Windows-enheter. Hvis du vil ha mer informasjon, kan du se [Innstillinger for Windows 10 (og nyere) for å beskytte enheter ved hjelp av Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Du bør være klar over at mange nyere enheter som kjører Windows 10 støtter automatisk BitLocker-kryptering, som utløses uten program for MDM-policy. Dette kan påvirke bruk av policy hvis ikke-standard innstillinger er konfigurert. Se følgende vanlige spørsmål for mer informasjon.
 
Hvis du vil ha informasjon om å feilsøke BitLocker-problemer, kan du se [Feilsøke BitLocker-policyer i Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**SPØRSMÅL OG SVAR**

Spørsmål: hvilke utgaver av Windows støtter enhets kryptering ved hjelp av policyen for ende punkt beskyttelse?<br>
Svar: innstillingene i policyer for Intune Endpoint Protection implementeres ved hjelp av [BitLocker-CSPen](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Ikke alle utgaver eller versjoner av Windows støtter BitLocker-CSPEN. <br><br>

Spørsmål: Hvordan kan BitLocker aktiveres på enheter uten å kreve slutt bruker medvirkning?<br>
A: så lenge de nødvendige forhånds kravene er oppfylt, er det mulig å aktivere BitLocker "stille kryptering" gjennom Intune. Se detaljene om enhetens krav og eksempler på policy innstillinger for å aktivere stille kryptering i følgende dokument: [aktivere BitLocker-kryptering stille](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

Spørsmål: Hvis en enhet allerede er kryptert med BitLocker ved hjelp av standard innstillingene for krypterings metode og chifferkodestyrke (XTS-AES-128), vil bruk av en policy med ulike innstillinger automatisk utløse rekryptering av stasjonen med de nye innstillingene?<br>
Sv.: Nei. Hvis du vil bruke de nye Cipher innstillingene, må stasjonen først dekrypteres.<br><br>
**Obs!** For enheter som blir registrert med automatisk pilot, utløses ikke krypteringen som ville oppstå under OOBE, før Intune-policyen evalueres, slik at de policy-baserte innstillingene kan brukes i stedet for OS-standardene.
 
Spørsmål: Hvis en enhet krypteres som et resultat av appen for Intune-policyen, dekrypteres den når policyen fjernes?<br>
Svar: fjerning av krypterings relatert policy fører ikke til dekryptering av stasjonene som ble konfigurert.
 
Spørsmål: Hvorfor viser Samsvars policyen for Intune at enheten ikke har BitLocker aktivert, selv om den er?<br>
A: innstillingen BitLocker Enabled i Intune-overholdelses policyen bruker Windows-klienten tilstands attestering (DHA). Denne klienten måler bare enhets tilstanden ved oppstart. Hvis en enhet ikke har blitt startet på nytt etter at BitLocker-kryptering ble fullført, vil ikke tjeneste tjenesten DHA rapportere at BitLocker blir aktivert.
 
 