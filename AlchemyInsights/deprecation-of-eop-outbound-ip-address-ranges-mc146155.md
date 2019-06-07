---
title: 1065 nedgraderingen EOP utgående IP-adresse rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 9860845dea444847833d4c5cd01d49ea93473778
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752964"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Nedgraderingen av EOP utgående IP-adresseområder

Vi har oppdaget et mulig problem med organisasjonen som (Hvis ikke korrigert av oktober 26th, 2018) kan bryte e-postflyt til lokale eller eksterne mål. Som tidligere formidlet for å forenkle behandling av IP-adressen området konsoliderer vi Exchange Online Protection (EOP) IP-adresseområder som brukes til å sende og motta e-post utenfor Office 365. Vår analyse viser at ett eller flere av e-post for eksterne kilder eller mål du har konfigurert i e-post flyt koblinger ikke godtar tilkoblinger fra de IP-adresse områdene vist [her](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Utføre en handling før oktober 26th å sikre disse kilder og mål skal godta tilkoblinger til og fra alle [publiserte EOP IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Hvis du vil ha mer informasjon om denne endringen, kan du se Meldingssentral innlegg [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Merk**: Hvis du tidligere brukte URL-adresse eller IP-publisering via HTML, XML og RSS-oppdateringer for sluttpunktet, også bør du oppdatere til de nye web-tjenestene for å automatisere disse typene oppdateringer. Hvis du vil ha mer informasjon, kan du se [Office 365 endepunktet kategorier og Office 365-IP-adresse og URL-adressen for webtjenesten](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
