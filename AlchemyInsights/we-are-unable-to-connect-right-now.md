---
title: Aktiveringsproblem – Vi kan ikke koble til akkurat nå
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
- "3408"
- "9001423"
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998167"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Løse meldingen Microsoft 365 «Vi kan ikke koble til akkurat nå»

Hvis du mottar denne meldingen, kan du prøve følgende:

1. Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Microsoft 365 apper. Se [Microsofts nettadresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå til **Start**  >  **Kjør**, og skriv deretter **inn services.msc**. Kontroller at følgende tjenester kjører:
    - Automatisk konfigurasjon av nettverkstilkoblingsenheter
    - Nettverkslistetjeneste
    - Nettverksplasseringsbevissthet
    - Windows Hendelseslogg

Hvis en av disse tjenestene ikke kjører, kan du prøve å starte den. Hvis du har problemer med å starte tjenesten, kjører du følgende kommando ved å åpne en ledetekst med utvidede tillatelser:

**sfc /scannow**

Når denne kommandoen er ferdig, starter du datamaskinen på nytt.

Hvis du vil ha detaljert informasjon, kan du se [«Beklager, vi kan ikke koble til kontoen din. Prøv på nytt senere» når du aktiverer](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)Office fra Microsoft 365 .