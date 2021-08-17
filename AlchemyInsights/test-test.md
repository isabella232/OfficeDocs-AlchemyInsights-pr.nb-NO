---
title: Vilkår som mangler SharePoint Online Term Store
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
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106435"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivere Bitlocker-kryptering med Intune

Intune Endpoint Protection Policy kan brukes til å konfigurere Innstillinger for Boitlocker-kryptering for Windows-enheter som beskrevet i : Windows10-innstillinger (og nyere) for å beskytte enheter ved hjelp av Intune

Du bør være oppmerksom på at mange nyere enheter som kjører Windows 10 støtter automatisk bitlocker-kryptering som utløses uten bruk av MDM-policy. Dette kan påvirke bruken av policyen hvis ikke-standardinnstillinger er konfigurert. Se Vanlige spørsmål for mer informasjon.


Vanlige spørsmål: Hvilke versjoner av Windows støtter enhetskryptering ved hjelp av Endpoint Protection policyen?
A: Innstillingene i Intune Endpoint Protection policy implementeres ved hjelp av Bitlocker CSP.  Ikke alle versjoner eller bygg av Windows støtter Bitlocker CSP. På dette tidspunktet Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise og Professional (fra bygg 1809 og fremover) støttes.




Sp.: Hvis en enhet allerede er kryptert med Bitlocker ved hjelp av standardinnstillingene for operativsystemet for krypteringsmetode og chiffreringsstyrke (XTS-AES-128), vil bruk av en policy med forskjellige innstillinger automatisk utløse ny kryptering av stasjonen med de nye innstillingene?

Sv.: Nei. Hvis du vil bruke de nye chiffreringsinnstillingene, må stasjonen først dekrypteres.

Obs! For enheter som registreres med Autopilot, utløses ikke den automatiske krypteringen som ville skje under OOBE, før Intune-policyen evalueres, noe som gjør at policybaserte innstillinger kan brukes i stedet for OS-standardene




Spørsmål Hvis en enhet krypteres som et resultat av bruken av Intune-policyen, dekrypteres den når policyen fjernes?

A: Fjerning av krypteringsrelatert policy fører IKKE til dekryptering av stasjonene som ble konfigurert.




Sp.: Hvorfor viser policyen for overholdelse av samsvar at enheten ikke har «Bitlocker aktivert», men det er det?

Sv.: Innstillingen «Bitlocker aktivert» i policyen for intune-samsvar bruker Windows Device Health Attestation (DHA)-klienten. Denne klienten måler bare enhetstilstanden ved oppstart. Så hvis en enhet ikke har blitt startet på nytt siden bitlocker-krypteringen ble fullført, vil ikke DHA-klienttjenesten rapportere bitlocker som aktiv.