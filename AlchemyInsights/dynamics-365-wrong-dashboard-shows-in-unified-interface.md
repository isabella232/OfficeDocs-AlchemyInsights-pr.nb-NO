---
title: Dynamics 365 – Feil instrumentbord vises i Dynamics 365 Unified Interface
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
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101491"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Feil instrumentbord vises i Dynamics 365 enhetlig grensesnitt

Det finnes flere årsaker til at du kan se et annet instrumentbord enn det du forventer:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Brukeren har angitt et brukerstandardinstrumentbord 

Vanligvis kan du identifisere en brukers  standard instrumentbord er angitt hvis Angi som standard-knappen ikke vises i kommandolinjen på instrumentbordet. Brukerstandardinstrumentbordet overstyrer alle andre standard instrumentbord, selv om brukerens standardinstrumentbord ikke er i den gjeldende appen.

Bruk følgende løsning for å fjerne standardinstrumentbordet.

1. Opprette et nytt personlig instrumentbord.

2. Angi det nye instrumentbordet som standard for brukeren.

3. Slett instrumentbordet.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Instrumentbordet er angitt i nettstedskartet

Du kan ha angitt et standard instrumentbord for organisasjonen ved å velge et instrumentbord og velge Bruk som standard under Tilpass systemet. Instrumentbordet som er definert i nettstedskartutformingen, vil imidlertid ha forrang over dette instrumentbordet hvis brukeren har tilgang til det.

Hvis du vil at brukerne skal se instrumentbordet du har angitt som standard for organisasjonen, kan du enten:

* Angi instrumentbordet i nettstedskartet

* Fjerne tilgang til det definerte instrumentbordet for nettstedskart for disse brukerne
