---
title: Fikse Office-apper Beklager, vi har midlertidig emisjonsproblemer
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
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764126"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Fikse Office-appene "Beklager, vi har midlertidige serverproblemer" melding

Hvis du mottar denne meldingen, kan du prøve følgende:

1. Kontroller brannmur-, antivirusprogramvaren- og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Office-apper. Se [URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå til **Start** > **Kjør**, og skriv deretter inn **services.msc**. Kontroller at følgende tjenester kjører:
    - Automatisk oppsett av nettverkstilkoblede enheter
    - Nettverkslistetjeneste
    - Bevissthet om nettverksplassering
    - Hendelseslogg for Windows

Hvis en av disse tjenestene ikke kjører, kan du prøve å starte den. Hvis du har problemer med å starte tjenesten, kjører du følgende kommando ved å åpne en ledetekst med forhøyede tillatelser:

**sfc / scannow**

Når denne kommandoen er fullført, starter du datamaskinen på nytt.

Hvis du vil ha detaljert informasjon, kan du se ["Beklager, vi kan ikke koble til kontoen din. Prøv på nytt senere" feil når du aktiverer](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).