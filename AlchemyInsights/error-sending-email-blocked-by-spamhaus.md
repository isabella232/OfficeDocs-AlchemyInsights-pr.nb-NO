---
title: Feil under sending av e-post blokkert av SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783812"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Feil under sending av e-post: klient vert blokkert ved hjelp av Spamhaus

IP-adressen som sendte meldingen, er i en blokkerings liste som eies av [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Årsaker til at du blir blokkert av Spamhaus inkluderer kompromitterte kontoer, som har brutte maskiner som deler en offentlig IP-adresse og retnings linjer for Internett-leverandør (ISP). Mulige løsninger er:
  
- For blokkerte inn kommende meldinger der du styrer kilde-e-postserveren, må du finne årsaken og fjerne blokken fra Spamhaus-nettstedet.

- For blokkerte inn kommende meldinger der kilde-IP-adressen tilhører noen andre, må adresse eieren fjerne blokken fra Spamhaus-nettstedet. Hvis IP-adressen er i policyen for policy blokkering (PBL), kan eieren tilordne en annen statisk IP-adresse eller fjerne adressen fra PBL.

- For blokkerte utgående meldinger fra domenet som er koblet til Microsoft, kan du få denne feilen hvis meldingene er rutet gjennom en tredje parts tjeneste. Du kan bruke et WHOIS-oppslags verktøy til å finne den blokkerte IP-adressen som eier.
