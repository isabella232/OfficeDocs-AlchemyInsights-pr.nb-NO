---
title: Om identitet i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918946"
---
# <a name="about-identity-in-yammer"></a>Om identitet i Yammer

Det anbefales at alle nettverk gjør følgende for å unngå identitetsrelaterte problemer:

1. Fremtving Office 365 identitet etter klargjøring Microsoft 365 kontoer for brukere i Azure AD for å sikre at alle brukere logger seg på ved hjelp av den primære Microsoft 365 kontoen. Hvis du vil ha mer informasjon, [kan du se Office 365 identitet for Yammer brukere](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolidere Yammer nettverk. Eldre Yammer konfigurasjoner gjør at flere Yammer nettverk kan kobles til én leier. Hvis du vil ha mer informasjon, kan du se [Nettverksoverføring – Konsolidere Yammer nettverk.](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)
3. Du kan også bruke lisensiering for Yammer å blokkere brukere Yammer hvis de ikke har en lisens. Hvis du vil ha mer informasjon, [kan du se Administrere Yammer brukerlisenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Til slutt kan du overvåke brukerlisten for eldre Yammer nettverk og deaktivere eldre brukere. Det anbefales at du deaktiverer (deaktiverer) brukere i stedet for å slette dem, fordi slettingen er irreversible. Hvis du vil ha mer informasjon, [kan du se Overvåke Yammer brukere i nettverk](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) som er koblet til Office 365 og Fjern [brukere](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Når du konfigurerer Yammer ved hjelp av disse trinnene, er du også klar til å konfigurere Yammer for opprinnelig modus for Microsoft 365. Hvis du vil ha mer informasjon, [kan du se Konfigurere Yammer for opprinnelig modus for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).