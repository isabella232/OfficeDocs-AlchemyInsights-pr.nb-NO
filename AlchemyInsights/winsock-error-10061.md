---
title: 1554 Winsock-feil 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859149"
---
# <a name="winsock-error-10061"></a>Winsock-feil 10061

Denne koden betyr at Office 365 ikke kan opprette en TCP socket (tilkobling) med verten. Den mest sannsynlige årsaken til denne feilen er et problem med brannmurkonfigurasjonen. Hvis du vil løse problemet, kontrollerer du disse innstillingene:

- Kontroller konfigurasjonen av brannmur med informasjonen i [Office 365 URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Hvis feilen, er spesifikk for Exchange Online Protection (EOP), bør du har blitt tidligere melding til en endring i [Exchange Online beskyttelse IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Kontroller at Internett-leverandøren (ISP) ikke blokkerer porten.

- Kontroller smart verts- og serverinnstillingene i koblingene.

Legg merke til at Office 365 ikke blokkerer *innkommende* tilkoblinger på denne måten.
