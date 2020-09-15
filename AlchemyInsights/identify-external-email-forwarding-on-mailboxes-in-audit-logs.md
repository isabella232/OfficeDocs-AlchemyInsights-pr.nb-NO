---
title: Identifisere eksterne e-postvideresending på post bokser i overvåkings logger
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696306"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifisere når ekstern e-postvideresending konfigureres på post bokser

Når en Microsoft 365-bruker konfigurerer ekstern e-postvideresending på en post boks, overvåkes aktiviteten som en del av cmdleten **Set-post boks** . Du kan se aktiviteten ved hjelp av overvåkings Logg søk i sikkerhets & Samsvars senteret.

1. Logg på [sikkerhets & samsvars senteret til Microsoft 365](https://protection.office.com/).

2. Gå til **Search**  >  **søke siden for overvåkings Logg** for søk.

3. Velg dato området i feltene **Start dato** og **slutt dato** . Du trenger ikke angi et bruker navn. Kontroller at **aktiviteter** -feltet er satt til å **vise resultater for alle aktiviteter**.

4. Klikk **Søk**.

I resultatene klikker du **Filtrer resultater** og skriv inn **Set-postboks** i aktivitets Filter-boksen. Velg en overvåkings post i resultatene. Klikk **mer informasjon**i under menyen **detaljer** . Du må se på detaljene for hver overvåkings post for å avgjøre om aktiviteten er relatert til videre sending av e-post.

- **ObjectID**: alias-verdien til post boksen som ble endret.

- **Parametere**: _ForwardingSmtpAddress_ angir mål-e-postadressen.

- **Userid**: brukeren som konfigurerte e-postvideresending på post boksen i **objectID** -feltet.

Hvis du vil ha mer informasjon, kan du se [finne ut hvem som konfigurerte videre sendingen av e-post](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
