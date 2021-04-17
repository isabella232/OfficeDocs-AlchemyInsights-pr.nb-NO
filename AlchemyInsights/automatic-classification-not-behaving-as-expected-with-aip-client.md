---
title: Automatisk klassifisering fungerer ikke som forventet med AIP-klienten
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
- "9002266"
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820907"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatisk klassifisering fungerer ikke som forventet med AIP-klienten

Automatisk klassifisering fungerer ikke som forventet. Bruk følgende anbefalte retningslinjer:

1. Hvis du har problemer med automatisk merking, kan du se [Slik konfigurerer du betingelser for automatisk og anbefalt klassifisering for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) og [Dette ser sensitive informasjonstyper etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Kontroller om du bruker områdepolicyer som ikke er konfigurert på riktig måte: [Slik konfigurerer du Azure Information Protection-policy for bestemte brukere ved hjelp av områdepolicyer](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Hvis automatisk merking ikke fungerer for Outlook når du legger ved et merket dokument, må du kontrollere at `DRMEncryptProperty` ikke er definert som beskrevet her: [IRM-registerinnstillinger for sikkerhet](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Hvis du brukte [innebygde informasjonstyper](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) for Azure Information Protection-policyen, må du kontrollere at innholdet samsvarer med forventet format.
5. Kontroller at merket er riktig konfigurert for **Automatisk** eller **Anbefalt**. (**Automatisk** merking er tilgjengelig for alle Microsoft 365-apper, mens **Anbefalt** er tilgjengelig for alle Microsoft 365-apper, bortsett fra Outlook.)
6. Du kan ikke bruke automatisk klassifisering for dokumenter og e-post som tidligere ble merket manuelt eller merket automatisk med høyere klassifisering.  Hvis du vil ha mer informasjon, kan du se [Slik brukes automatiske eller anbefalte merker](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Hvis du fremdeles opplever problemer, kan du kontakte Azure Information Protection-klientlogger og legge ved de eksporterte loggene i støtteforespørselen. Slik eksporterer du Azure Information Protection-logger:
    - Åpne et Office-dokument eller opprett en ny e-post i Outlook.
    - Klikk på **Beskytt/følsomhet** > **Hjelp og tilbakemelding**.
    - Klikk på **Eksporter logger**.
    - Lagre alle loggene på valgt plassering, og legg dem ved tjenesteforespørselen.

Hvis du vil ha mer informasjon, kan du se:

- [Slik konfigurerer du betingelser for automatisk og anbefalt klassifisering for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Veiledninger for vanlige scenarioer som bruker Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Gå gjennom Azure Information Protection-dokumentasjon](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Gå gjennom abonnementer og funksjoner for Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Krav for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Hurtigstartveiledning for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Last ned Azure Information Protection-klient](https://www.microsoft.com/download/details.aspx?id=53018)
