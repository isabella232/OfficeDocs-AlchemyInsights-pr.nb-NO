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
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716469"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifisere når ekstern videresending av e-post er konfigurert på postbokser

Når en Microsoft 365-bruker konfigurerer ekstern videresending av e-post på en postboks, overvåkes aktiviteten som en del av cmdleten **Set-postboks.** Du kan se aktiviteten ved hjelp av overvåkingsloggsøk i Sikkerhets& compliance Center.

1. Logg på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Gå til**søkesiden for søkeloggen for søke etter** søk i **søkesiden for søkeetter søk.** > 

3. Velg datoperioden i feltene **Startdato** og **Sluttdato.** Du trenger ikke å angi et brukernavn. Kontroller **at Aktiviteter-feltet** er satt til **Vis resultater for alle aktiviteter**.

4. Klikk **Søk**.

Klikk **Filtrer resultater** i resultatene, og skriv inn **Set-postboks** i aktivitetsfilterboksen. Velg en overvåkingspost i resultatene. Klikk **Mer informasjon**i undermenyen **Detaljer.** Du må se på detaljene for hver revisjonsoppføring for å finne ut om aktiviteten er relatert til videresending av e-post.

- **ObjectId**: Aliasverdien for postboksen som ble endret.

- **Parametere**: _ForwardingSmtpAddress_ angir mål-e-postadressen.

- **UserId**: Brukeren som konfigurerte videresending av e-post på postboksen i **ObjectId-feltet.**

Hvis du vil ha mer informasjon, kan du se [Finne ut hvem som konfigurerer videresending av e-post for en postboks](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
