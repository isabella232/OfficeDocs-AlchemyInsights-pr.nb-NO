---
title: 'INSTALLASJONs vilkår: policyer ikke oppfører seg som forventet'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663198"
---
# <a name="aip-policies-not-behaving-as-expected"></a>INSTALLASJONs vilkår: policyer ikke oppfører seg som forventet

Azure Information Protection: policyer ikke oppfører seg som forventet, kan du se følgende for anbefalte retnings linjer for ulike policy problemer:

1. Hvis du har problemer med visuelle markeringer, kan du se gjennom [når visuelle markeringer brukes](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Hvis du har problemer med automatisk merking, kan du se [hvordan du konfigurerer betingelser for automatisk og anbefalt klassifisering for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) og [hva de sensitive informasjons typene ser ut for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Hvis du har problemer med opprinnelig/Pfile beskyttelse, kan du se [fil-API-konfigurasjonen](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Kontroller om du bruker omfangs policyer som ikke er riktig konfigurert: [Slik konfigurerer du policyen for Azure Information Protection for bestemte brukere ved hjelp av omfangs policyer](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Hvis automatisk merking ikke fungerer for Outlook når du legger ved et merket dokument, må du bekrefte at DRMEncryptProperty ikke er definert som beskrevet her: [IRM-register innstillinger for sikkerhet](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Hvis du fremdeles har problemer, kan du samle inn klient logger for Azure Information Protection og knytte de eksporterte loggene til denne billetten.

1. Åpne et Office-dokument eller opprette en ny e-post i Outlook.
2. Klikk **Beskytt/følsomhet**  >  **Hjelp og tilbake melding**.
3. Klikk **Eksporter logger**.
4. Lagre loggene på valg av sted, og legg dem ved denne service forespørselen.

Flere ressurser:

- [Slik konfigurerer du en etikett for visuelle markeringer for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Gå gjennom dokumentasjon for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Bruk følsomhet-etiketter i Microsoft 365-apper](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

