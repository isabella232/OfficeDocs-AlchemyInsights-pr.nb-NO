---
title: Dynamics 365 - feil instrumentbord viser i Dynamics 365 enhetlig grensesnitt
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528560"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Viser feil instrumentbord i Dynamics 365 enhetlig grensesnitt

Det er flere grunner til hvorfor du kanskje se en annen instrumentbord enn den du forventer:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Brukeren har angitt en bruker standard instrumentbord 

Vanligvis kan du identifisere en bruker standard instrumentbord er angitt Hvis knappen **Angi som standard** ikke vises i kommandolinjen for instrumentbordet. Bruker standard instrumentbord overstyrer alle andre instrumentbord for standard selv om brukerens standard instrumentbord ikke er i gjeldende program.

Bruk følgende løsning å Fjern deres standard instrumentbord.

1. Opprett et nytt personlig instrumentbord.

2. Angi det nye instrumentbordet som Brukerstandard.

3. Slett dette instrumentbordet.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Instrumentbordet er satt i områdekartet

Du har angitt en standard instrumentbord for organisasjonen ved å velge et instrumentbord og velge "Angi som standard, under Tilpass i systemet. Men instrumentbord som er definert i sitemap designer skal prioriteres foran dette instrumentbordet Hvis brukeren har tilgang til den.

Hvis du vil at brukere kan vise instrumentbordet du har angitt som Organisasjonsstandard, kan du:

* Angi dette instrumentbordet i områdekartet

* Fjern tilgang til instrumentbordet sitemap som er definert for disse brukerne
