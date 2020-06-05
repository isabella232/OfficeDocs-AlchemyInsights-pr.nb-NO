---
title: Løse Microsoft 365 apps Beklager, vi har midlertidig server problemer melding
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582712"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Løse meldingen "Beklager, vi har midlertidige serverproblemer"

Hvis du får denne meldingen, kan du prøve følgende:

1. Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Microsoft 365-apper. Se [URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå til **Start**  >  **Kjør**, og skriv deretter inn **services.msc**. Kontroller at følgende tjenester kjører:
    - Automatisk oppsett av nettverkstilkoblede enheter
    - Tjeneste for nettverksliste
    - Bevissthet om nettverksplassering
    - Hendelseslogg for Windows

Hvis en av disse tjenestene ikke kjører, kan du prøve å starte den. Hvis du har problemer med å starte tjenesten, kjører du følgende kommando ved å åpne en ledetekst med forhøyede tillatelser:

**sfc /scannow (SFC/scannow)**

Når denne kommandoen er fullført, starter du datamaskinen på nytt.

Hvis du vil ha detaljert informasjon, kan du se [«Beklager, vi kan ikke koble til kontoen din. Prøv på nytt senere" feil når du aktiverer](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).