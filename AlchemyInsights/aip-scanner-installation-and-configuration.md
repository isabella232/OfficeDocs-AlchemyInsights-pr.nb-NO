---
title: 'AIP-skanner: installasjon og konfigurasjon'
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
- "9002278"
- "5119"
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934266"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP-skanner: installasjon og konfigurasjon

Følg de anbefalte retningslinjene for **å installere AIP-skanneren:**

1. Hvis du oppgraderer og ikke utfører en ren installasjon, må du kontrollere at du har fulgt retningslinjene for oppgradering av [Azure Information Protection-skanneren](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) og for enhetlig merkingsklient, se Oppgradere [Azure Information Protection-skanneren](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Kontroller at du overholder alle [krav til brannmurer og innstillinger for nettverksinfrastruktur.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Kontroller at [policyene er satt til](https://docs.microsoft.com/azure/information-protection/configure-policy) automatisk merking eller har en standardetikett i policyen.
4. Kontroller at den relevante filtypen er konfigurert for etikett/beskyttelse som beskrevet i Filtyper som støttes av [Azure Information Protection-klienten.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Hvis du vil endre standard virkemåte, følger du i tillegg disse retningslinjene: Endre standard beskyttelsesnivå [for filer](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Kontroller at brukerkontoen som er konfigurert til å kjøre skannertjenesten, har tillatelse til å få tilgang til alle konfigurerte repositorier.
6. Hvis du fremdeles opplever problemer, kan du eksportere skannerloggene og legge dem til i støtteforespørselen.

**Eksportere Azure Information Protection Scanner-logger**

1. Gå til %localappdata%\Microsoft\MSIP under brukerkonteksten som kjører skannertjenesten.
2. Zip alt innholdet under MSIP-mappen.
3. Lagre alle loggene på valgt plassering, og legg dem ved tjenesteforespørselen.
4. Du kan også bruke [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Hvis du vil ha mer informasjon, kan du se:**
- [Distribuere Azure Information Protection-skanneren for å automatisk klassifisere og beskytte filer](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Angi og bruk Token-parameteren for Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Kjøre en oppdagelsessyklus og vise rapporter for skanneren](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Gå gjennom Azure Information Protection-dokumentasjon](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Krav for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Last ned Azure Information Protection-klient](https://www.microsoft.com/download/details.aspx?id=53018)
