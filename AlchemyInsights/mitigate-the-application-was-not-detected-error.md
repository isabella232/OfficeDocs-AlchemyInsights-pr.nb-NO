---
title: Fiks feilen Appen ble ikke funnet
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 34b2024257c88512db170cbb0e672c1628ad8e3935342f87c5032492e1ad0259
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026123"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Fiks feilen «Appen ble ikke funnet»

Appinstallasjonsfeilen «Appen ble ikke funnet etter fullført installasjon», rapportert av Intune, kan oppstå på alle de store OS-plattformene (Windows, iOS og Android).

De vanligste scenarioene som genererer denne feilen inkluderer:

- Appen er oppdatert utenfor Intune (fra en tredjeparts appbutikk) etter den første distribusjonen. Noen apper, for eksempel Google Chrome, kan utføre automatiske oppdateringer.
- En bruker har avinstallert appen etter den første installasjonen.

Løs dette problemet ved å først uføre en gjennomgang av enhetene som er påvirket for å fastslå scenarioet der problemet oppstår.

- Hvis appen har blitt oppdatert utenfor Intune, kan du angi at appdistribusjonen skal ignorere appversjonen. Dette gjør du ved å gå til **Appkonfigurasjon > Appinformasjon** og angi **Ignorer app**-versjon til **Ja**.
- Når du angir klienten, kan det være hensiktsmessig å distribuere appen som «obligatorisk» samt sikre at det er den nyeste versjonen som distribueres.
- Eventuelt kan du, på iOS-plattformen, bruke funksjonaliteten **automatisk oppdatering** som er tilknyttet Apple Volume Purchaase Program som kan konfigureres til å oppdatere seg automatisk til nye appversjoner når de blir tilgjengelige.

Hvis du vil ha mer informasjon om feilsøking av appinstallasjonsproblemer, kan du ta en titt på [Feilsøke problemer med appinstallasjoner](https://docs.microsoft.com/intune/troubleshoot-app-install).
