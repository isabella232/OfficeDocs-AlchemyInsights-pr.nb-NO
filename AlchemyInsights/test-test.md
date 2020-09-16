---
title: Termer mangler i term lageret i SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750460"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivere BitLocker-kryptering med Intune

Policyen for Intune Endpoint Protection kan brukes til å konfigurere Boitlocker krypterings innstillinger for Windows-enheter som beskrevet i: Windows10 (og nyere) innstillinger for å beskytte enheter ved hjelp av Intune

Du bør være klar over at mange nyere enheter som kjører Windows 10 støtter automatisk BitLocker-kryptering som utløses uten program for MDM-policy. Dette kan påvirke bruk av policy hvis det ikke er konfigurerte standard innstillinger. Se vanlige spørsmål for mer informasjon.


Vanlige spørsmål   : hvilke utgaver av Windows støtter enhets kryptering ved hjelp av policyen for ende punkt beskyttelse?
 Svar: innstillingene i policyer for Intune Endpoint Protection implementeres ved hjelp av BitLocker-CSPEN.Ikke alle utgaver eller versjoner av Windows støtter BitLocker-CSPEN. 
      På dette tidspunktet Windows-utgaver: Enterprise; Education, mobil, mobil Enterprise og Professional (fra Bygg 1809 fremover) støttes.




Spørsmål: Hvis en enhet allerede er kryptert med BitLocker ved hjelp av standard innstillingene for OS for krypterings metode og chifferkodestyrke (XTS-AES-128), vil bruk av en policy med ulike innstillinger automatisk utløse rekryptering av stasjonen med de nye innstillingene?

Sv.: Nei. Hvis du vil bruke de nye Cipher innstillingene, må stasjonen først dekrypteres.

Obs! for enheter som blir registrert med automatisk pilot, blir ikke den automatiske krypteringen som ville skje under OOBE, utløst før Intune-policyen blir evaluert, noe som gjør at policy innstillingene kan brukes i stedet for operativ system standardene




Hvis en enhet krypteres som et resultat av appen for Intune-policyen, dekrypteres den når policyen fjernes?

Svar: fjerning av krypterings relatert policy fører ikke til dekryptering av stasjonene som ble konfigurert.




Spørsmål: Hvorfor viser Samsvars policyen for Intune at enheten ikke har BitLocker aktivert, men det er?

A: innstillingen «BitLocker aktivert» i henhold til samsvars policyen for Intune bruker Windows Device Health Attestation-klienten (DHA). Denne klienten måler bare enhets tilstanden ved oppstart. Hvis en enhet ikke har blitt startet på nytt etter at BitLocker-kryptering ble fullført, vil ikke tjeneste tjenesten for DHA rapportere at BitLocker skal være aktiv.