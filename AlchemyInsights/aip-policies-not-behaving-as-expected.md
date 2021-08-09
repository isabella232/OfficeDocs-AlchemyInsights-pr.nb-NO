---
title: 'AIP: Policyer oppfører seg ikke som forventet'
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
- "4780"
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934302"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Policyer oppfører seg ikke som forventet

Azure Information Protection: Policyer oppfører seg ikke som forventet, se følgende for anbefalte retningslinjer for ulike policyproblemer:

1. Hvis du har problemer med visuelle markeringer, kan du se [gjennom Når visuelle markeringer brukes](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Hvis du har problemer med automatisk merking, kan du se Slik konfigurerer du betingelser for automatisk og anbefalt klassifisering [for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) og Hva ser de sensitive [informasjonstypene etter.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Hvis du har problemer med opprinnelig/Pfile-beskyttelse, kan du se [Fil-API-konfigurasjonen](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Kontroller om du bruker områdepolicyer som ikke er konfigurert på riktig måte: [Slik konfigurerer du Azure Information Protection-policy for bestemte brukere ved hjelp av områdepolicyer](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Hvis automatisk merking ikke fungerer for Outlook når du legger ved et merket dokument, kontrollerer du at DRMEncryptProperty ikke er definert som beskrevet her: [IRM-registerinnstillinger for sikkerhet](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Hvis du fremdeles har problemer, kan du samle inn Azure Information Protection-klientlogger og legge ved de eksporterte loggene i denne billetten.

1. Åpne et Office-dokument eller opprett en ny e-post i Outlook.
2. Klikk på **Beskytt/følsomhet** > **Hjelp og tilbakemelding**.
3. Klikk på **Eksporter logger**.
4. Lagre loggene på ønsket plassering, og legg dem ved denne serviceforespørselen.

Flere ressurser:

- [Slik konfigurerer du en etikett for visuelle markeringer for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Gå gjennom Azure Information Protection-dokumentasjon](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Bruke følsomhetsetiketter Microsoft 365 apper](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

