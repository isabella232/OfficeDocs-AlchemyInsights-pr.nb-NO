---
title: Daglig e-postgrense overskredet. Arbeidsflyten er deaktivert.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 5a510f1137c7c49cd1de3d3fd2a470759e37ba1e
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908713"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Daglig e-postgrense overskredet. Arbeidsflyten er deaktivert.

Denne feilen kan mottas i følgende scenarier:

- Du har en arbeidsflyt i SharePoint Online som bruker sharepoint 2010 eller SharePoint 2013 arbeidsflyt plattformtype.
- Arbeidsflyten er konfigurert til å sende en egendefinert e-postmelding til mer enn 200 brukere om gangen, mer enn 10 000 mottakere per dag eller mer enn 30 meldinger per minutt.
- Når du kjører arbeidsflyten, sendes ikke e-postmeldingen, og du legger merke til følgende virkemåte:
    - For en arbeidsflyt ved hjelp av sharepoint 2013-plattformtypen, kan du bla til **siden Arbeidsflytstatus.** På siden Arbeidsflytstatus er **den Interne statusen** satt til **Startet**, og informasjonsboblen viser Kan ikke sende til **en mottaker**.

Du kan omgå dette problemet ved å konfigurere arbeidsflyten til å sende e-postmeldinger uten å overskride [avsendergrensene](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)for Exchange Online . Bruk for eksempel en pause i arbeidsflyten, send e-posten til en Microsoft 365-gruppe, en distribusjonsgruppe eller en e-postaktivert sikkerhetsgruppe eller sende meldingen til færre enn 200 mottakere om gangen.


Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Beslektede emner
- [Opprett flyt](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 