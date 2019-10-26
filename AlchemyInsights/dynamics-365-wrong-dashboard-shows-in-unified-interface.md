---
title: Dynamics 365-feil Dashboard viser i Dynamics 365 enhetlig grensesnitt
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/25/2019
ms.locfileid: "36528560"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Feil dashbord vises i Dynamics 365 enhetlig grensesnitt

Det kan være flere grunner til at du ser et annet instrumentbord enn det du forventer:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Brukeren har angitt et standard instrumentbord for bruker 

Vanligvis kan du identifisere en brukers standard instrumentbord er angitt hvis **angitt som standard** -knappen ikke vises i kommandolinjen for instrumentbordet. Bruker standard instrumentbord overstyrer alle andre standard instrumentbord, selv om brukerens standard instrumentbord ikke er i den gjeldende appen.

Bruk følgende løsning for å avbryte Standardinstrumentbordet.

1. Opprett et nytt personlig instrumentbord.

2. Angi det nye instrumentbordet som bruker standard.

3. Slett dette instrumentbordet.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Dashbordet er satt i Sitemap

Du kan ha angitt et standard instrumentbord for organisasjonen ved å velge et instrumentbord og velge angi som standard under Tilpass systemet. Men dashbordet definert i Sitemap designeren vil forrang over dette dashbordet, hvis brukeren har tilgang til den.

Hvis du vil at brukerne skal se instrumentbordet du har angitt som organisasjonsstandard, kan du gjøre ett av følgende:

* Angi dette instrumentbordet i områdekartet

* Fjern tilgangen til sitemap-definerte dashbord for disse brukerne
