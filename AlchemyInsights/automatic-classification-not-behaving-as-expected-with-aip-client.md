---
title: Automatisk klassifisering oppfører seg ikke som forventet med AIP-klienten
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
- "4373"
ms.openlocfilehash: 95a994d6a49ee8737a6ebcb196314f92776d8482
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493178"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatisk klassifisering oppfører seg ikke som forventet med AIP-klienten

Automatisk klassifisering som ikke oppfører seg som forventet, bruk følgende anbefalte retningslinjer:

1. Hvis du har problemer med automatisk merking, kan du se [Konfigurere betingelser for automatisk og anbefalt klassifisering for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) og Hva de sensitive [informasjonstypene ser etter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).
2. Kontroller om du bruker policyer for omfang som ikke er riktig konfigurert: Slik konfigurerer du [policyen for Azure information protection for bestemte brukere ved hjelp av policyer for omfang](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Hvis automatisk merking ikke fungerer for Outlook når du legger ved et merket dokument, må du kontrollere at `DRMEncryptProperty` det ikke er definert som beskrevet her: [IRM-registerinnstillinger for sikkerhet](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Hvis du brukte de [innebygde informasjonstypene](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) for azure information protection policy, må du kontrollere at innholdet samsvarer med det forventede formatet.
5. Kontroller at etiketten er riktig konfigurert for **Automatisk** eller **Anbefalt**. **(Automatisk** merking er tilgjengelig for alle Office-apper, mens **Anbefalt** er tilgjengelig for alle Office-apper unntatt Outlook.)
6. Du kan ikke bruke automatisk klassifisering for dokumenter og e-postmeldinger som tidligere ble merket manuelt eller tidligere automatisk merket med en høyere klassifisering.  Hvis du vil ha mer informasjon, kan du se: [Hvordan automatiske eller anbefalte etiketter brukes](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Hvis du fortsatt har problemer, kan du samle inn Azure Information Protection-klientlogger og legge ved de eksporterte loggene i støttebilletten. Slik eksporterer du Azure Information Protection-logger:
    - Åpne et Office-dokument eller opprett en ny e-post i Outlook.
    - Klikk På Hjelp og tilbakemelding **for beskyttelse/følsomhet**  >  **Help and feedback**.
    - Klikk **Eksporter logger**.
    - Lagre loggene i ditt valg av plassering, og legg dem ved i serviceforespørselen.

Hvis du vil ha mer informasjon, kan du se:

- [Slik konfigurerer du betingelser for automatisk og anbefalt klassifisering for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Veiledninger for vanlige scenarier som bruker Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Se gjennom dokumentasjonen for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Se gjennom Azure Information Protection-abonnementer og -funksjoner](https://azure.microsoft.com/pricing/details/information-protection)
- [Krav til Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Hurtigstartveiledning for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Last ned Azure Information Protection-klient](https://www.microsoft.com/download/details.aspx?id=53018)
