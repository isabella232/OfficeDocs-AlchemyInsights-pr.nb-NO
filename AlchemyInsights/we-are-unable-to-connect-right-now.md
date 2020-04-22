---
title: Aktiveringsproblem - Vi kan ikke koble til akkurat nå
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716181"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Fikse Office-appene «Vi kan ikke koble til akkurat nå»-meldingen

Hvis du mottar denne meldingen, kan du prøve følgende:

1. Kontroller brannmur-, antivirusprogramvaren- og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Office-apper. Se [Microsoft-URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå til **Start** > **Kjør**, og skriv deretter inn **services.msc**. Kontroller at følgende tjenester kjører:
    - Automatisk oppsett av nettverkstilkoblede enheter
    - Nettverkslistetjeneste
    - Bevissthet om nettverksplassering
    - Hendelseslogg for Windows

Hvis en av disse tjenestene ikke kjører, kan du prøve å starte den. Hvis du har problemer med å starte tjenesten, kjører du følgende kommando ved å åpne en ledetekst med forhøyede tillatelser:

**sfc / scannow**

Når denne kommandoen er fullført, starter du datamaskinen på nytt.

Hvis du vil ha detaljert informasjon, kan du se ["Beklager, vi kan ikke koble til kontoen din. Prøv på nytt senere" feil når du aktiverer Office fra Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).