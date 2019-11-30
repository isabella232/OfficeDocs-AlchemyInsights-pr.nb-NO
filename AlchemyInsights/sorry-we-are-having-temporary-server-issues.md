---
title: Reparere Office-apper beklager, vi har midlertidig server problemer melding
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627999"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Fikse Office-programmer "Beklager, vi har midlertidige Server problemer"-melding

Hvis du får denne meldingen, kan du prøve følgende:

1. Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Office-apper. Se [URL-adresser for Office 365 og IP-adresser](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå til **Start** > **Kjør**, og skriv deretter inn **Services. msc**. Kontroller at følgende tjenester kjører:
    - Automatisk installasjon av nettverkstilkoblede enheter
    - Tjeneste for nettverksliste
    - Kunnskap om nettverksplassering
    - Hendelseslogg for Windows

Hvis en av disse tjenestene ikke kjører, kan du prøve å starte den. Hvis du har problemer med å starte tjenesten, kjører du følgende kommando ved å åpne en ledetekstmed forhøyede tillatelser:

**sfc/scannow**

Når denne kommandoen er ferdig, starter du datamaskinen på nytt.

Hvis du vil ha mer informasjon, se ["Beklager, vi kan ikke koble til kontoen din. Vennligst prøv igjen senere "feil når du aktiverer Office fra Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).