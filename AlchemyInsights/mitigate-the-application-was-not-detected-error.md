---
title: Fiks feilen Appen ble ikke funnet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810492"
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
