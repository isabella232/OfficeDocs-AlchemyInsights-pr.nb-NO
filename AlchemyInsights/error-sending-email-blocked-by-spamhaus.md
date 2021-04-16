---
title: Feil under sending av e-post blokkert av SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813733"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Feil under sending av e-post: Klientvert blokkert ved hjelp av Spamhaus

IP-adressen som sendte meldingen, er på en blokkeringsliste som eies av [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245) Årsaker til å bli blokkert av Spamhaus omfatter kompromitterte kontoer, kompromitterte maskiner som deler en offentlig IP-adresse og Policyer for Internett-leverandør (ISP). Mulige løsninger er:
  
- For blokkerte innkommende meldinger der du kontrollerer kilde-e-postserveren, må du finne årsaken og fjerne blokkeringen fra Spamhaus-nettstedet.

- For blokkerte innkommende meldinger der kilde-IP-adressen tilhører noen andre, må adresseeieren fjerne blokkeringen fra Spamhaus-nettstedet. Hvis IP-adressen er på blokkeringslisten for policy (PBL), kan eieren tilordne en annen statisk IP-adresse eller fjerne adressen fra PBL.

- For blokkerte utgående meldinger fra domenet som er koblet til Microsoft, kan du få denne feilmeldingen hvis meldingene rutes gjennom en tredjepartstjeneste. Du kan bruke et WHOIS-oppslagsverktøy til å finne eieren av den blokkerte IP-adressen.
