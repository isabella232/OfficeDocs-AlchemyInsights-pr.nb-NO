---
title: Om identitet i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148308"
---
# <a name="about-identity-in-yammer"></a>Om identitet i Yammer

Det anbefales at alle nettverk tar følgende trinn for å unngå identitetsrelaterte problemer:

1. Fremtving Office 365-identitet etter klargjøring av Microsoft 365-kontoer for brukere i Azure AD for å sikre at alle brukere logger på ved hjelp av sin primære Microsoft 365-konto. Hvis du vil ha mer informasjon, kan du se [Fremtving Office 365-identitet for Yammer-brukere](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolidere flere Yammer-nettverk. Eldre Yammer-konfigurasjoner tillater at flere Yammer-nettverk er koblet til én leier. Hvis du vil ha mer informasjon, kan du se [Nettverksoverføring – Konsolidere flere Yammer-nettverk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Du kan eventuelt fremtvinge lisensiering for Yammer for å blokkere brukere fra Yammer hvis de ikke har en lisens. Hvis du vil ha mer informasjon, kan du se [Administrere Yammer-brukerlisenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Til slutt kan du overvåke brukerlisten for eldre Yammer-nettverk og suspendere eldre brukere. Det anbefales at du suspenderer (deaktiverer) brukere i stedet for å slette dem, fordi sletting er irreversibel. Hvis du vil ha mer informasjon, kan du se [Overvåke Yammer-brukere i nettverk som er koblet til Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) og [Fjerne brukere](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Ved å konfigurere Yammer ved hjelp av disse trinnene, er du også klar til å konfigurere Yammer-nettverket for opprinnelig modus for Microsoft 365. Hvis du vil ha mer informasjon, kan du se [Konfigurere Yammer-nettverket for opprinnelig modus for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).