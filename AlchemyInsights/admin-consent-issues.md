---
title: Problemer med administrator samtykke
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901506"
---
# <a name="admin-consent-issues"></a>Problemer med administrator samtykke

1. Aktiver [arbeids flyten for administrator samtykke](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) for å tillate at brukere ber om administrator godkjenning direkte fra skjerm bildet for samtykke.

1. Hvis du eller programmets brukere ser uventede feil under samtykke prosessen, kan du se denne artikkelen for feil søkings trinn: [uventet feil under utføring av samtykke til et program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Lær mer om [administrator samtykke på Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), hvordan [samtykke lede teksten](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) fungerer, og hvordan du [evaluerer en forespørsel om godkjennings samtykke for hele leieren](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Programmer som integreres med Microsoft Identity Platform, følger en Autorisasjons modell som gir brukere og administratorer kontroll over hvordan data kan nås. Implementeringen av Autorisasjons modellen er oppdatert på Microsoft Identity Platform Endpoint, og den endrer hvordan en app må samhandle med Microsoft Identity Platform. Se [tillatelser og samtykke i Microsoft Identity Platform Endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for en oversikt over denne Autorisasjons modellen, inkludert omfang, tillatelser og samtykke.