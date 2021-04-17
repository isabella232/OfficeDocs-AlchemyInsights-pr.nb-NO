---
title: Løse Microsoft 365-apper Beklager, vi har midlertidige serverproblemer
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835280"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Løse meldingen «Beklager, vi har midlertidige serverproblemer» i Microsoft 365-appene

Hvis du mottar denne meldingen, kan du prøve følgende:

1. Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Microsoft 365-apper. Se [nettadresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå til **Start**  >  **Kjør**, og skriv deretter **inn services.msc**. Kontroller at følgende tjenester kjører:
    - Automatisk konfigurasjon av nettverkstilkoblingsenheter
    - Nettverkslistetjeneste
    - Nettverksplasseringsbevissthet
    - Windows-hendelseslogg

Hvis en av disse tjenestene ikke kjører, kan du prøve å starte den. Hvis du har problemer med å starte tjenesten, kjører du følgende kommando ved å åpne en ledetekst med utvidede tillatelser:

**sfc /scannow**

Når denne kommandoen er ferdig, starter du datamaskinen på nytt.

Hvis du vil ha detaljert informasjon, kan du se [«Beklager, vi kan ikke koble til kontoen din. Prøv på nytt senere» når du aktiverer](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).