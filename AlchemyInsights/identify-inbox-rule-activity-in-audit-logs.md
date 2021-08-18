---
title: Identifisere innboksregelaktivitet i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331132"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifisere innboksregelaktivitet i overvåkingslogger

Du kan bruke søk i overvåkingsloggen Samsvarssenter for Microsoft 365 vise innboksregelhendelser (opprette, endre og slette innboksregler).

1. Gjør ett av følgende:
   - I Samsvarssenter for Microsoft 365 på <https://compliance.microsoft.com> går du til **Løsningsovervåking** \> . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://compliance.microsoft.com/auditlogsearch> .
   - Gå Microsoft 365 Defender til Overvåking i <https://security.microsoft.com> **portalen** på . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://security.microsoft.com/auditlogsearch> .

2. Konfigurer følgende innstillinger  på **Søk-fanen** på overvåkingssiden:
   - **Dato- og klokkeslettområde:** Velg dato-/klokkeslettområdet i **Start-** og **Slutt-boksene.**
   - **Aktiviteter:** Velg én eller flere av følgende verdier:
     - **Ny innboksRegel Opprett innboksregel fra Outlook Web App**
     - **Set-InboxRule Endre regel fra Outlook Web App**.
     - **Oppdatere innboksregler fra Outlook klient**

3. Når du er ferdig, klikker du **Søk**. Aktivitetene vises på den nye **siden for overvåkingssøk.**

4. Velg en aktivitet i resultatene for å åpne undermenyen for detaljer. Informasjon om innstillingene for innboksregelen vises i **Parametere-feltet.**

Hvis du vil ha mer informasjon, [kan du se Fastslå om en bruker opprettet en innboksregel](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
