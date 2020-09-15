---
title: Dynamics 365 – feil instrument bord vises i Dynamics 365 Unified Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711284"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Feil instrument bord programmer vises i Dynamics 365 Unified Interface

Det finnes flere årsaker til at du kan se et annet instrument bord enn det du forventer:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Brukeren har angitt et standard instrument bord for bruker 

Du kan vanligvis identifisere et bruker standard instrument bord som er angitt hvis **Angi som standard** -knappen ikke vises på instrument bord kommando linjen. Bruker standard instrument bordet vil overstyre alle andre standard instrument bord, selv om brukerens standard instrument bord ikke er i gjeldende app.

Bruk følgende løsning for å fjerne standard instrument bord.

1. Opprette et nytt personlig instrument bord.

2. Angi at nytt instrument bord skal være standard for brukeren.

3. Slett dette instrument bordet.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Instrument bordet er angitt i Sitemap

Du kan ha angitt et standard instrument bord for organisasjonen ved å velge et instrument bord og velge angi som standard under Tilpass systemet. Instrument bordet som er definert i kart-utforming-verktøyet, vil ha forrang over dette instrument bordet hvis brukeren har tilgang til det.

Hvis du vil at brukere skal se instrument bordet du har angitt som standard for organisasjonen, kan du enten:

* Angi dette instrument bordet i område kart

* Fjerne tilgang til det definerte instrument bord for sitemap for disse brukerne
