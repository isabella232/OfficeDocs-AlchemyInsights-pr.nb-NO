---
title: DataProtection – Bitlocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118603"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivere Bitlocker-kryptering med Intune

Intune Endpoint Protection policy kan brukes til å konfigurere Bitlocker-krypteringsinnstillinger for Windows enheter. Hvis du vil ha mer [informasjon, Windows 10 (og nyere) innstillinger for å beskytte enheter ved hjelp av Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

I tillegg til Endpoint Protection policyen finnes det også en krypteringsrapport som gir en mer detaljert visning av krypteringsstatusen for enheter. Denne rapporten kan nås fra **MEM-portalen** under Enheter > skjerm , og deretter velger du [Krypteringsrapport](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)under Konfigurasjon. 

Hvis du finner ut at Bitlocker ikke kan aktiveres som forventet, eller at profilen som brukes til å aktivere Bitlocker, er i en feiltilstand, kan du se gjennom krypteringsrapporten for å få en bedre forståelse av hvorfor virkemåten forekommer.

Hvis du vil ha mer informasjon om hvordan du tolker rapporten, inkludert de ulike krypteringsstatusverdiene, kan du se Overvåke enhetskryptering [med Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

Du bør være oppmerksom på at mange nyere enheter som kjører Windows 10 støtter automatisk Bitlocker-kryptering, som utløses uten bruk av MDM-policy. Dette kan påvirke bruken av policyen hvis ikke-standardinnstillinger er konfigurert. Se følgende vanlige spørsmål hvis du vil ha mer informasjon.

Hvis du vil ha informasjon om feilsøking av bitlocker-problemer, kan du se [Feilsøke BitLocker-policyer i Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**SPØRSMÅL OG SVAR**

Spørsmål: Hvilke versjoner av Windows støtter enhetskryptering ved hjelp av Endpoint Protection policyen?<br>
A: Innstillingene i Intune Endpoint Protection policy implementeres ved hjelp av [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Ikke alle versjoner eller bygg av Windows støtter Bitlocker CSP. <br><br>

Spørsmål: Hvordan kan Bitlocker aktiveres på enheter uten å kreve sluttbrukersamhandling?<br>
Sv.: Så lenge de nødvendige forutsetningene er oppfylt, er det mulig å aktivere Bitlocker «Stille kryptering» gjennom Intune. Se detaljene for enhetskravene og eksempelpolicyinnstillingene for å aktivere stille kryptering i følgende dokument: [Aktiver Bitlocker-kryptering stille.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

Sp.: Hvis en enhet allerede er kryptert med Bitlocker ved hjelp av standardinnstillingene for operativsystemet for krypteringsmetode og chiffreringsstyrke (XTS-AES-128), vil bruk av en policy med forskjellige innstillinger automatisk utløse ny kryptering av stasjonen med de nye innstillingene?<br>
Sv.: Nei. Hvis du vil bruke de nye chiffreringsinnstillingene, må stasjonen først dekrypteres.<br><br>
**Obs!** For enheter som registreres med Autopilot, utløses ikke den automatiske krypteringen som ville skje under OOBE før Intune-policyen evalueres, noe som gjør at de policybaserte innstillingene kan brukes i stedet for OS-standardene.
 
Spørsmål: Hvis en enhet krypteres som et resultat av bruken av Intune-policyen, dekrypteres den når policyen fjernes?<br>
A: Fjerning av krypteringsrelatert policy fører IKKE til dekryptering av stasjonene som ble konfigurert.
 
Sp.: Hvorfor viser Intune Compliance Policy at enheten ikke har Bitlocker aktivert, selv om den er det?<br>
Sv.: Innstillingen «Bitlocker aktivert» i Intune Compliance Policy bruker Windows Device Health Attestation (DHA)-klienten. Denne klienten måler bare enhetstilstanden ved oppstart. Så hvis en enhet ikke har blitt startet på nytt siden Bitlocker-krypteringen ble fullført, vil ikke DHA-klienttjenesten rapportere Bitlocker som aktiv.
 
 