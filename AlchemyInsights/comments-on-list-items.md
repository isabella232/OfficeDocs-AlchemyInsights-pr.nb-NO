---
title: Kommentarer om liste elementer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982487"
---
# <a name="comments-on-list-items"></a>Kommentarer om liste elementer

Brukere vil snart kunne legge til og slette kommentarer i liste elementer. Brukere kan vise alle kommentarer i et liste element og filtrere mellom visninger som viser kommentarer eller aktivitet som er relatert til et element.

**Tids beregning** :

**Målrettet utgivelse** : gradvis Rull ut i midt-oktober og forventet å fullføre med midt-november

**Standard utgivelse** : gradvis innrulling i midt-november og forventet å fullføre innen tidlig desember

**Distribusjon** : målrettet utgivelse for hele organisasjonen

Brukere må merke av nedenfor før de kan legge til og slette kommentarer:

- Kommentarer følger tillatelses innstillingene i SharePoint.
- Klassiske lister som ennå ikke er bygget for å vises i moderne bruker grensesnitt, for eksempel oppgave lister, vil ikke ha denne kommenterings funksjonen.
- Kommentering på lister i Teams er ikke tilgjengelig i denne versjonen.
- Kommentarer er ikke indeksert av søk.

Administratorer kan deaktivere denne funksjonen på organisasjons nivå ved å endre **CommentsOnListItemsDisabled** -parameteren i **Set-SPOTenant PowerShell-** cmdleten.

Det er for øyeblikket ikke mulig å deaktivere kommentering på område-eller liste nivå. Vi håper at du har disse kontrollene i en senere oppdatering, sannsynligvis i den første kvartal 2021.
