---
title: Løse Microsoft 365 apper Beklager, vi har midlertidige serverproblemer
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
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744676"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Løse meldingen Microsoft 365 «Beklager, vi har midlertidige serverproblemer»

Obs! Hvis du bruker en eldre versjon av Windows (for eksempel Windows 7 SP1, Windows Server 2008 [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) R2), bruker du den enkle løsningen for å aktivere TLS 1.2 som standard. Hvis du vil ha mer informasjon, kan du se Oppdatere for å aktivere [TLS 1.1 og TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)som standard sikre protokoller i WinHTTP i Windows .

Hvis du får denne meldingen, kan du prøve følgende:

1. Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Microsoft 365 apper. Se [nettadresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå til **Start**  >  **Kjør**, og skriv deretter **inn services.msc**. Kontroller at følgende tjenester kjører:
    - Automatisk konfigurasjon av nettverkstilkoblingsenheter
    - Nettverkslistetjeneste
    - Nettverksplasseringsbevissthet
    - Windows Hendelseslogg

Hvis en av disse tjenestene ikke kjører, kan du prøve å starte den. Hvis du har problemer med å starte tjenesten, kjører du følgende kommando ved å åpne en ledetekst med utvidede tillatelser:

**sfc /scannow**

Når denne kommandoen er ferdig, starter du datamaskinen på nytt.

Hvis du vil ha detaljert informasjon, kan du se [«Beklager, vi kan ikke koble til kontoen din. Prøv på nytt senere» når du aktiverer](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).