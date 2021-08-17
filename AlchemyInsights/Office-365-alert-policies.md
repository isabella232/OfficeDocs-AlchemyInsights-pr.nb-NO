---
title: 1385-Office-365-alert-policies
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: f5109445530ec4cc4988fb9c5d37145c45794ced6920607ce6df85c6497c25ec
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891688"
---
# <a name="alert-policies"></a>Varslingspolicyer

Microsoft 365 inneholder standard [](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) varslingspolicyer som utløser varsler for organisasjoner med et Microsoft 365 Enterprise- eller Microsoft 365 E1/G1-, E3/G3- eller E5/G5-abonnement. Administratorer kan derfor motta et varsel på e-post som sendes av Office365Alerts@microsoft.com med en emnelinje, for eksempel «Et varsel med lav alvorlighetsgrad: navnet på *varslingspolicyen».* Varslinger sendes når varsler utløses for vanlige aktiviteter, for eksempel når brukere:

- Opprette innboksregler som videresender e-post.
- Tilordne tillatelser til postboksen.
- Del eller slett et stort antall filer i SharePoint fildeling.
- Opprett eDiscovery-søk og eksporter søkeresultater.

Slik ser du gjennom og handler på et varsel:

1. Gjør ett av følgende:
   - I Samsvarssenter for Microsoft 365 på <https://compliance.microsoft.com> går du til **Varsler**. Du kan også gå direkte til **Varsler-siden** ved å bruke <https://compliance.microsoft.com/compliancealerts> .
   - Gå til Microsoft 365 Defender-varsler i portalen <https://security.microsoft.com> **& på** \> . Du kan også gå direkte til **Varsler-siden** ved å bruke <https://security.microsoft.com/alerts> .
2. Klikk et varsel for å vise en undermenyside med informasjon om varselet.

Du kan gjøre noe med et varsel, for eksempel fjerne [en mistenkelig innboksregel](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account). Du kan også ganske enkelt lukke varselet ved å klikke **Løs** på undermenyen for varselet.

Hvis du vil ha mer informasjon om hvordan du konfigurerer og administrerer varslingspolicyer, kan du  [se denne artikkelen](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).

**Viktig:** Varsler via e-post fra Microsoft vil aldri be deg om å gjøre følgende:

- Angi et passord
- Bekrefte sikkerhetsdetaljene for kontoen din
- Godkjenne deg selv på nytt

Hvis du mottar en e-postmelding med denne typen forespørsler, ble den ikke sendt av Microsoft og bør betraktes som en phishingsvindel. Hvis du mottar en melding med disse typene forespørsler, [rapporterer du meldingen til Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).
