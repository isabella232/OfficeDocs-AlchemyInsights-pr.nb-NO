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
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083239"
---
# <a name="winsock-error-10061"></a>Winsock-feil 10061

Denne feilkoden betyr at Microsoft ikke kan etablere en TCP-kontakt (tilkobling) med målverten. Den mest sannsynlige årsaken til denne feilen er et problem med brannmurkonfigurasjonen. Kontroller disse innstillingene for å løse problemet:

- Kontroller brannmurkonfigurasjonen med informasjonen i Microsoft 365 [nettadresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Hvis feilen er spesifikk for Exchange Online Protection (EOP), skal du tidligere ha blitt varslet om en endring i Exchange Online Protection [IP-adressene](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Kontroller at Internett-leverandøren ikke blokkerer porten.

- Kontroller innstillingene for smartverten og målserveren i koblingene.

Vær oppmerksom Microsoft 365 ikke blokkerer *innkommende* tilkoblinger på denne måten.
