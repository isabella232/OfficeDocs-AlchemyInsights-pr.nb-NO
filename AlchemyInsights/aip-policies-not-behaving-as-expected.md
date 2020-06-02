---
title: 'AIP: Retningslinjer oppfører seg ikke som forventet'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506567"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Retningslinjer oppfører seg ikke som forventet

Azure Information Protection: Policyer som ikke fungerer som forventet, kan du se følgende for anbefalte retningslinjer for ulike policyproblemer:

1. Hvis du har problemer med visuelle markeringer, kan du se [Når visuelle markeringer brukes](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Hvis du har problemer med automatisk merking, kan du se Slik konfigurerer du [betingelser for automatisk og anbefalt klassifisering for Azure Information Protection og](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) Hva de sensitive [informasjonstypene ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Hvis du har problemer med opprinnelig/pfile beskyttelse, kan du se [fil-API-konfigurasjon](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Kontroller om du bruker policyer for omfang som ikke er riktig konfigurert: Slik konfigurerer du [policyen for Azure information protection for bestemte brukere ved hjelp av policyer for omfang](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Hvis automatisk merking ikke fungerer for Outlook når du legger ved et merket dokument, må du kontrollere at DRMEncryptProperty ikke er definert som beskrevet her: [IRM-registerinnstillinger for sikkerhet](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Hvis du fortsatt har problemer, kan du samle inn Azure Information Protection-klientlogger og legge ved de eksporterte loggene til denne billetten.

1. Åpne et Office-dokument eller opprett en ny e-post i Outlook.
2. Klikk På Hjelp og tilbakemelding **for beskyttelse/følsomhet**  >  **Help and feedback**.
3. Klikk **Eksporter logger**.
4. Lagre loggene til ditt valg av plassering, og legg dem ved denne serviceforespørselen.

Flere ressurser:

- [Slik konfigurerer du en etikett for visuelle markeringer for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Se gjennom dokumentasjonen for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Bruke følsomhetsetiketter i Office-apper](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

