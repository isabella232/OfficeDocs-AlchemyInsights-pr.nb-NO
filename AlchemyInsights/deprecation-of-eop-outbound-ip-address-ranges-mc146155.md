---
title: 1065 Nedgradering av EOP utgående IP-adresseområderMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704606"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Nedgradering av EOP utgående IP-adresseområder

Vi har oppdaget et potensielt problem med organisasjonen din som (hvis ikke korrigert innen 26. oktober 2018) kan bryte e-postflyten til lokale eller eksterne destinasjoner. Som tidligere kommunisert, for å forenkle administrasjon av IP-adresseområde, konsoliderer vi IP-adresseområdene Exchange Online Protection (EOP) som brukes til å sende og motta e-post utenfor Microsoft 365. Vår analyse indikerer at én eller flere av de eksterne e-postkildene eller målene du har konfigurert i e-postflytkoblinger, ikke godtar tilkoblinger fra IP-adresseområdene som vises [her](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Handle før 26 oktober for å sikre at disse kildene og destinasjonene vil akseptere tilkoblinger til og fra alle [publiserte EOP IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Hvis du vil ha mer informasjon om denne endringen, kan du se Message Center innlegg [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Merk:** Hvis du tidligere har brukt IP- eller URL-publisering via HTML-, XML- og RSS-adresse for endepunktoppdateringer, bør du også overføre til de nye webtjenestene for å automatisere denne typen oppdateringer. Hvis du vil ha mer informasjon, kan du se [Microsoft 365 endepunktkategorier og Microsoft 365 IP-adresse og URL-webtjeneste](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
