---
title: 1065 avskrevet av EOP utgående IP-adresse rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806804"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Avskrevet av utgående IP-adresseområder for EOP

Vi har oppdaget et mulig problem med organisasjonen din som (hvis den ikke er rettet opp av oktober 26th, 2018) kan bryte e-postflyten til de lokale eller eksterne stedene. Som tidligere kommunisert, konsoliderer vi IP-adresseområder for Exchange Online Protection (EOP) som brukes til å sende og motta e-post utenfor Microsoft 365, for å forenkle behandling av IP-adresseområde. Vår analyse indikerer at én eller flere av de eksterne e-postkildene eller-målene som du har konfigurert i e-postflyt-koblinger, ikke godtar tilkoblinger fra IP-adresseområder som vises [her](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Act før oktober 26th for å sikre at disse kildene og målene vil godta tilkoblinger til og fra alle [PUBLISERTE EoP-IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Hvis du vil ha mer informasjon om denne endringen, kan du se meldings senter inn Legg [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Obs**! hvis du tidligere har brukt IP-eller URL-publisering via HTML, XML og RSS for ende punkt oppdateringer, bør du også overføre til de nye nett tjenestene for automatisering av disse typene oppdateringer. Hvis du vil ha mer informasjon, kan du se [microsoft 365 Endpoint Categories og microsoft 365 IP Address og URL-webtjeneste](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
