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
ms.openlocfilehash: b7146b2b09b6ac1e33b192dcbcbfb72ea2593313
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630258"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifisere når videresending av ekstern e-post er konfigurert på postbokser

Når en Microsoft 365 konfigurerer ekstern videresending av e-post på en postboks, overvåkes aktiviteten som en del av **cmdleten Set-Mailbox.** Du kan se aktiviteten ved hjelp av søk i overvåkingsloggen i sikkerhetssenteret & samsvarssenteret.

1. Logg på Microsoft 365 [Samsvarssenter](https://protection.office.com/).

2. Gå til **søkesiden**  >  **søk i overvåkingsloggen.**

3. Velg datoområdet i **feltene Startdato og** **Sluttdato.** Du trenger ikke å angi et brukernavn. Kontroller at **Aktiviteter-feltet** er satt til **Vis resultater for alle aktiviteter**.

4. Klikk **Søk**.

Klikk Filtrer resultater i **resultatene,** og skriv **inn Angi postboks** i aktivitetsfilterboksen. Velg en overvåkingspost i resultatene. Klikk **Mer** informasjon på **Detaljer-undermenyen.** Du må se på detaljene for hver overvåkingspost for å finne ut om aktiviteten er relatert til videresending av e-post.

- **ObjectId:** Aliasverdien for postboksen som ble endret.

- **Parametere:** _ForwardingSmtpAddress_ angir e-postadressen for målet.

- **UserId:** Brukeren som konfigurerte videresending av e-post på postboksen i **ObjectId-feltet.**

Hvis du vil ha mer informasjon, kan du se [Fastslå hvem som konfigurerte videresending av e-post for en postboks](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
