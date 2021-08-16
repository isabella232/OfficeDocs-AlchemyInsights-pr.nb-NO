---
title: Slik deaktiverer du eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015629"
---
# <a name="how-to-disable-external-groups"></a>Slik deaktiverer du eksterne grupper

Yammer eksterne meldinger Exchange et sett med proaktive kontroller for å hindre at firmainformasjon deles. Hvis du vil begrense brukere fra å opprette eksterne grupper, må du konfigurere en Exchange-transportregel (ETR), og deretter konfigurere Yammer til å bruke Exchange-transportregelen til å blokkere eksterne meldinger.
  
Når du har opprettet en regel i Exchange Online administrasjonssenteret, følger du disse trinnene for å angi at ETR skal brukes i Yammer:
  
- Logg på Yammer som bekreftet administrator, og gå til C-Yammer i administrasjonssenteret **\> for Innstillinger.**

- Under **Eksterne meldinger** velger du **Fremtving Exchange Online Exchange transportregler (ETR) i Yammer.**

- Velg **Lagre**.

Hvis du vil ha mer informasjon, kan du se Deaktivere [eksterne meldinger i et Yammer nettverk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  