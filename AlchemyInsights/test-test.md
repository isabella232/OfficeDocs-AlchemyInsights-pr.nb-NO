---
title: Vilkår mangler fra SharePoint Online term store
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053522"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivere BitLocker-kryptering med Intune

Policyen for beskyttelse mot endepunkter for Intune kan brukes til å konfigurere Boitlocker krypteringsinnstillinger for Windows-enheter som beskrevet i: Windows10 (og senere) innstillinger for å beskytte enheter ved hjelp av Intune

Du bør være oppmerksom på at mange nyere enheter som kjører Windows 10 støtter automatisk BitLocker-kryptering som utløses uten bruk av MDM-policy. Dette kan påvirke bruken av policy hvis ikke standardinnstillingene er konfigurert. Se vanlige spørsmål for flere detaljer.


Vanlige  spørsmål: hvilke versjoner av Windows støtter Enhetskryptering ved å bruke policyen for sluttpunktbeskyttelse?
 A: innstillingene i Intune Endpoint Protection policy implementeres ved hjelp av BitLocker CSP.Ikke alle utgaver eller versjoner av Windows støtter BitLocker CSP. 
      På dette tidspunktet Windows Editions: Enterprise; Utdanning, Mobile, mobile Enterprise og Professional (fra bygge 1809 og framover) støttes.




Q: Hvis en enhet er allerede kryptert med BitLocker bruker OS standardinnstillingene for krypteringsmetode og Cipher styrke (XTS-AES-128) vil bruke en policy med ulike innstillinger automatisk utløse re-kryptering av stasjonen med de nye innstillingene?

A: Nei. For å bruke de nye Cipher innstillingene stasjonen må først dekrypteres.

For enheter som blir registrert med autopilot, utløses automatisk kryptering som vil oppstå under OOBE ikke før Intune-policy evalueres som tillater policy-baserte innstillinger som skal brukes i stedet for OS-standarder




Q hvis en enhet krypteres som et resultat av bruken av Intune-policyen, blir den dekryptert når denne policyen fjernes?

A: fjerning av kryptering relatert policy fører ikke til dekryptering av stasjonene som ble konfigurert.




Spørsmål: Hvorfor viser Intune Compliance policy at enheten ikke har "BitLocker Enabled", men det er?

A: "BitLocker aktivert"-innstillingen i samsvars policyen for Intune bruker Windows Device Health-klienten (DHA). Denne klienten måler bare Enhetsstatus ved oppstart. Så hvis en enhet ikke har blitt startet på nytt siden BitLocker-krypteringen ble fullført, vil ikke DHA-klienttjenesten rapportere BitLocker som aktiv.