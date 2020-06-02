---
title: Identifisere ekstern videresending av e-post på postbokser i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508961"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifisere når ekstern videresending av e-post er konfigurert på postbokser

Når en Microsoft 365-bruker konfigurerer ekstern videresending av e-post på en postboks, overvåkes aktiviteten som en del av **cmdleten Set-Postboks.** Du kan se aktiviteten ved hjelp av søk i overvåkingslogg i & samsvarssenter for sikkerhet.

1. Logg på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Gå til søkeloggen for søk i **søkeloggen for søk i søkeloggen for søk**  >  **Audit log search** i søke.

3. Velg datointervallet i feltene **Startdato** og **Sluttdato.** Du trenger ikke å angi et brukernavn. Kontroller at **Aktiviteter-feltet** er satt til **Vis resultater for alle aktiviteter**.

4. Klikk **Søk**.

Klikk **Filtrer resultater** i resultatene, og skriv inn **Set-Mailbox** i aktivitetsfilterboksen. Velg en overvåkingsoppføring i resultatene. Klikk **Mer informasjon**i **undermenyen Detaljer.** Du må se på detaljene for hver overvåkingsoppføring for å finne ut om aktiviteten er relatert til videresending av e-post.

- **ObjectId**: Aliasverdien for postboksen som ble endret.

- **Parametere:** _VideresendingSmtpAddress_ angir mål-e-postadressen.

- **UserId**: Brukeren som konfigurerte videresending av e-post på postboksen i **ObjectId-feltet.**

Hvis du vil ha mer informasjon, kan du se [Finne ut hvem som konfigurerte videresending av e-post for en postboks](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
