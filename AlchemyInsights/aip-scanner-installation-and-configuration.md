---
title: 'AIP-skanner: installasjon og konfigurasjon'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358102"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP-skanner: installasjon og konfigurasjon

**Hvis du vil installere AIP-skanneren, følger du de anbefalte retningslinjene:**

1. Hvis du oppgraderer og ikke utfører en ren installasjon, må du kontrollere at du har fulgt retningslinjene for [oppgradering av Azure Information Protection-skanneren](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) og for enhetlig merkingsklient, kan du se oppgradere Azure Information [Protection-skanneren](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Kontroller at du overholder alle [krav til innstillinger for brannmurer og nettverksinfrastruktur](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Kontroller at [policyene](https://docs.microsoft.com/azure/information-protection/configure-policy) dine er satt til automatisk merking eller har en standardetikett i policyen.
4. Kontroller at den relevante filtypen er konfigurert for etikett/beskyttelse som beskrevet i [Filtyper som støttes av Azure Information Protection-klienten](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Hvis du vil endre standardvirkemåten, følger du i tillegg disse retningslinjene: [Endre standard beskyttelsesnivå for filer](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Kontroller at brukerkontoen som er konfigurert til å kjøre skannertjenesten, har tillatelse til å få tilgang til alle de konfigurerte repositoriene.
6. Hvis du fortsatt har problemer, må du eksportere skannerloggene og legge dem til i støttebilletten.

**Eksportere Azure Information Protection Scanner-logger**

1. Gå til %localappdata%\Microsoft\MSIP under brukerkonteksten som kjører skannertjenesten.
2. Zip alt innholdet under MSIP-mappen.
3. Lagre loggene i ditt valg av sted, og legg dem ved serviceforespørselen.
4. Du kan også bruke [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Hvis du vil ha mer informasjon, kan du se**:
- [Distribuere Azure Information Protection-skanneren for å klassifisere og beskytte filer automatisk](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Angi og bruke tokenparameteren for Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Kjøre en oppdagelsessyklus og vise rapporter for skanneren](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Se gjennom dokumentasjonen for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Krav til Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Last ned Azure Information Protection-klienten](https://www.microsoft.com/download/details.aspx?id=53018)
