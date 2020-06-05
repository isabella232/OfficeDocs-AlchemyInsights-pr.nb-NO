---
title: Daglig e-postgrense overskredet. Arbeidsflyten er suspendert.
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
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580342"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Daglig e-postgrense overskredet. Arbeidsflyten er suspendert.

Denne feilen kan mottas i følgende scenarier:

- Du har en arbeidsflyt i SharePoint Online som bruker sharepoint 2010- eller SharePoint 2013 arbeidsflytplattformtypen.
- Arbeidsflyten er konfigurert til å sende en egendefinert e-postmelding til mer enn 200 brukere om gangen, mer enn 10 000 mottakere per dag eller mer enn 30 meldinger per minutt.
- Når du kjører arbeidsflyten, sendes ikke e-postmeldingen, og du legger merke til følgende virkemåte:
    - For en arbeidsflyt som bruker sharepoint 2013-plattformtypen, går du til siden **Arbeidsflytstatus.** På siden Arbeidsflytstatus er **intern status** satt til **Startet**, og informasjonsboblen viser **Kan ikke sende til en mottaker**.

Du kan omgå dette problemet ved å konfigurere arbeidsflyten til å sende e-postmeldinger uten å overskride [Exchange Online-avsendergrensene](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Bruk for eksempel en pause i arbeidsflyten, send e-posten til en Microsoft 365-gruppe, en distribusjonsgruppe eller en sikkerhetsgruppe som er aktivert for e-post, eller send meldingen til færre enn 200 mottakere om gangen.


Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Beslektede emner
- [Opprett flyt](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 