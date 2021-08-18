---
title: Identifisere videresending av ekstern e-post på postbokser i overvåkingslogger
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331168"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifisere når videresending av ekstern e-post er konfigurert på postbokser

Når en Microsoft 365 konfigurerer ekstern videresending av e-post på en postboks, overvåkes aktiviteten som en del av **cmdleten Set-Mailbox.** Du kan se aktiviteten ved hjelp av søk i overvåkingsloggen. Slik gjør du det:

1. Gjør ett av følgende:
   - I Samsvarssenter for Microsoft 365 på <https://compliance.microsoft.com> går du til **Løsningsovervåking** \> . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://compliance.microsoft.com/auditlogsearch> .
   - Gå Microsoft 365 Defender til Overvåking i <https://security.microsoft.com> **portalen** på . Du kan også gå direkte til **overvåkingssiden** ved å bruke <https://sip.security.microsoft.com/auditlogsearch> .

2. Kontroller at **Søk-fanen**  er valgt på Overvåking-siden, og konfigurer deretter følgende innstillinger:
   - Velg dato-/klokkeslettområdet i **Start-** og **Slutt-boksene.**
   - Kontroller at **Aktiviteter-boksen** inneholder **Vis resultater for alle aktiviteter**.

3. Når du er ferdig, klikker du **Søk**. Aktivitetene vises på den nye **siden for overvåkingssøk.**

4. Klikk Filtrer resultater **i** resultatene, og skriv inn **Set-Mailbox** i aktivitetsfilterboksen.

5. Velg en overvåkingspost i resultatene. Klikk **Mer** informasjon på **Detaljer-undermenyen.** Du må se på detaljene for hver overvåkingspost for å finne ut om aktiviteten er relatert til videresending av e-post.

   - **ObjectId:** Aliasverdien for postboksen som ble endret.
   - **Parametere:** _ForwardingSmtpAddress_ angir e-postadressen for målet.
   - **UserId:** Brukeren som konfigurerte videresending av e-post på postboksen i **ObjectId-feltet.**

Hvis du vil ha mer informasjon, kan du se [Fastslå hvem som konfigurerte videresending av e-post for en postboks](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
