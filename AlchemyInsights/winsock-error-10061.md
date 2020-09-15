---
title: 1554 Winsock-feil 10061
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
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698871"
---
# <a name="winsock-error-10061"></a>Winsock-feil 10061

Denne feil koden betyr at Microsoft ikke kunne opprette en TCP-socket (tilkobling) med mål verten. Den mest sannsynlige årsaken til denne feilen er et problem med brann mur konfigurasjonen. Du kan løse problemet ved å kontrollere disse innstillingene:

- Bekreft brann mur konfigurasjonen med informasjonen i [URL-adresser og IP-adresseområder for Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Hvis feilen er spesifikk for Exchange Online Protection (EOP), bør du tidligere ha blitt varslet om en endring i [IP-adressene for Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Kontroller at Internett-leverandøren din ikke blokkerer porten.

- Kontroller innstillingene for smart verts-og målserver i koblingene.

Vær oppmerksom på at Microsoft 365 ikke blokkerer *inn kommende* tilkoblinger på denne måten.
