---
title: Vilkår som mangler fra SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766862"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivere Bitlocker-kryptering med Intune

Intune Endpoint Protection Policy kan brukes til å konfigurere Boitlocker krypteringsinnstillinger for Windows-enheter som beskrevet i : Windows10 (og senere) innstillinger for å beskytte enheter som bruker Intune

Du bør være oppmerksom på at mange nyere enheter som kjører Windows 10, støtter automatisk bitlocker-kryptering som utløses uten bruk av MDM-policy. Dette kan påvirke programmet for policy hvis ikke-standardinnstillinger er konfigurert. Se Vanlige spørsmål for mer informasjon.


Vanlige  spørsmål: Hvilke versjoner av Windows støtter enhetskryptering ved hjelp av policyen for beskyttelse av endepunkt?
 Svar: Innstillingene i Intune Endpoint Protection Policy implementeres ved hjelp av Bitlocker CSP.Ikke alle utgaver eller versjoner av Windows støtter Bitlocker CSP. 
      På dette tidspunktet Windows Editions: Enterprise; Utdanning, Mobil, Mobil bedrift og Professional (fra bygge 1809 og utover) støttes.




Spørsmål: Hvis en enhet allerede er kryptert med Bitlocker ved hjelp av OS-standardinnstillingene for krypteringsmetode og chifferstyrke (XTS-AES-128), vil bruk av en policy med forskjellige innstillinger automatisk utløse rekryptering av stasjonen med de nye innstillingene?

A: Nei. For å kunne bruke de nye chifferinnstillingene må stasjonen først dekrypteres.

For enheter som registreres med Autopilot, utløses ikke den automatiske krypteringen som oppstår under OOBE før Intune-policyen evalueres, noe som gjør at policybaserte innstillinger kan brukes i stedet for OS-standardene




Q Hvis en enhet er kryptert som følge av anvendelsen av Intune-policyen, dekrypteres den når denne policyen fjernes?

A: Fjerning av krypteringsrelatert policy resulterer IKKE i dekryptering av stasjonene som ble konfigurert.




Spørsmål: Hvorfor viser intune Compliance policy at enheten min ikke har "Bitlocker Aktivert", men det er det?

Svar: Innstillingen "Bitlocker aktivert" i intune compliance policy bruker Windows Device Health Attestation (DHA)-klienten. Denne klienten måler bare enhetstilstand ved oppstart. Så hvis en enhet ikke har blitt startet på nytt siden bitlocker kryptering ble fullført DHA-klienttjenesten vil ikke rapportere bitlocker som aktiv.