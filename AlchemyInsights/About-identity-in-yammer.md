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
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664179"
---
# <a name="about-identity-in-yammer"></a>Om identitet i Yammer

Det anbefales at alle nettverk utfører følgende trinn for å unngå identitets relaterte problemer:

1. Tving Office 365-identitet etter klar gjøring av Microsoft 365-kontoer for brukere i Azure AD for å sikre at alle brukere logger på ved hjelp av den primære Microsoft 365-kontoen. Hvis du vil ha mer informasjon, kan du se [tvinge Office 365-identitet for Yammer-brukere](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolider flere Yammer-nettverk. Eldre Yammer-konfigurasjoner tillater at flere Yammer-nettverk kobles til én Tenant. Hvis du vil ha mer informasjon, kan du se [nettverks overføring – Konsolider flere Yammer-nettverk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Du kan også håndheve lisensiering for Yammer for å blokkere brukere fra Yammer hvis de ikke har en lisens. Hvis du vil ha mer informasjon, kan du se [administrere bruker lisenser for Yammer i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Til slutt kan du overvåke bruker listen for eldre Yammer-nettverk og utsette eldre brukere. Det anbefales at du deaktiverer (deaktiverer) brukere i stedet for å slette dem, for du kan ikke slette. Hvis du vil ha mer informasjon, kan du se [overvåke Yammer-brukere i nettverk som er koblet til Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) og [fjerne brukere](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Ved å konfigurere Yammer ved hjelp av disse trinnene, er du også klar til å konfigurere Yammer-nettverket for opprinnelig modus for Microsoft 365. Hvis du vil ha mer informasjon, kan du se [konfigurere Yammer-nettverket for opprinnelig modus for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).