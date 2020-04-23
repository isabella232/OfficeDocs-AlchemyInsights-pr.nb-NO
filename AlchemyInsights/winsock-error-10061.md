---
title: 1554 Winsock-feil 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766178"
---
# <a name="winsock-error-10061"></a>Winsock-feil 10061

Denne feilkoden betyr at Microsoft ikke kan opprette en TCP-socket (tilkobling) med målverten. Den mest sannsynlige årsaken til denne feilen er et problem med brannmurkonfigurasjonen. Hvis du vil løse problemet, kontrollerer du disse innstillingene:

- Kontrollere brannmurkonfigurasjonen med informasjonen i [URL-adresser og IP-adresseområder for Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Hvis feilen er spesifikk for Exchange Online Protection (EOP), burde du tidligere ha blitt varslet om en endring i [IP-adressene](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)for Exchange Online Protection .

- Kontroller at Internett-leverandøren (ISP) ikke blokkerer porten.

- Kontroller innstillingene for smart verts- og målserver i kontaktene.

Vær oppmerksom på at Microsoft 365 ikke blokkerer *innkommende* tilkoblinger på denne måten.
