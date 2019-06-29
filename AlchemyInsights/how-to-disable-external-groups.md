---
title: Slik deaktiverer du eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384834"
---
# <a name="how-to-disable-external-groups"></a>Slik deaktiverer du eksterne grupper

Yammer eksterne meldinger gjelder Exchange Transportregler (ETRs), et sett med proaktiv kontroller for å hindre at selskapet informasjon blir delt. Hvis du vil hindre brukere i å opprette eksterne grupper, må du konfigurere en Exchange transport regel (ETR), og deretter konfigurere Yammer Hvis du vil bruke regelen for Exchange Transport til å blokkere eksternt messaging.
  
Når du har opprettet en regel i Exchange Online administrasjonssenteret, følger du disse trinnene for å angi ETR å bruke i Yammer:
  
- Logger på Yammer som en kontrollert admin, og **Yammer administrasjonssenteret**, går du til C **innhold og sikkerhet \> sikkerhetsinnstillinger.**

- **Eksterne meldinger**, velg **gjennomføre Exchange Online Exchange Transport reglene (ETRs) i Yammer.**

- Velg **Lagre**.

Hvis du vil ha mer informasjon, se [kontrollere eksterne meldinger i Yammer-nettverket med Exchange Transportregler](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)
  