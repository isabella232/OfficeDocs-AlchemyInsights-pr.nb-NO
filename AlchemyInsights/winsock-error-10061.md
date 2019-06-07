---
title: 1554 Winsock-feil 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 3fa3b2f2e10d3ebe480861e1f2d7ecaa262afe14
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757110"
---
# <a name="winsock-error-10061"></a>Winsock-feil 10061

Denne koden betyr at Office 365 ikke kan opprette en TCP socket (tilkobling) med verten. Den mest sannsynlige årsaken til denne feilen er et problem med brannmurkonfigurasjonen. Hvis du vil løse problemet, kontrollerer du disse innstillingene:

- Kontroller konfigurasjonen av brannmur med informasjonen i [Office 365 URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Hvis feilen, er spesifikk for Exchange Online Protection (EOP), bør du har blitt tidligere melding til en endring i [Exchange Online beskyttelse IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Kontroller at Internett-leverandøren (ISP) ikke blokkerer porten.

- Kontroller smart verts- og serverinnstillingene i koblingene.

Legg merke til at Office 365 ikke blokkerer *innkommende* tilkoblinger på denne måten.
