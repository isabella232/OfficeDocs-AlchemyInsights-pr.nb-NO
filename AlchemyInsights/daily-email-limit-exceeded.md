---
title: Den daglige grensen for e-post overskrides. Arbeidsflyten er suspendert.
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
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053126"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Daglig e-grensen er overskredet. Arbeidsflyten er suspendert.

Denne feilen kan mottas i følgende scenarier:

- Du har en arbeidsflyt i SharePoint Online som bruker SharePoint 2010 eller SharePoint 2013 arbeidsflyt plattformtype.
- Arbeidsflyten er konfigurert til å sende en egendefinert e-postmelding til mer enn 200 brukere om gangen, mer enn 10 000 mottakere per dag, eller mer enn 30 meldinger per minutt.
- Når du kjører arbeidsflyten, e-postmeldingen er ikke sendt, og du legger merke til følgende virkemåte:
    - Du går til siden **status for arbeidsflyt** for en arbeidsflyt ved hjelp av plattform typen for SharePoint 2013. Den **interne statusen** er satt til **startet**på siden status for arbeidsflyt, og informasjonsboblen viser **kan ikke sende til en mottaker**.

Du kan omgå dette problemet ved å konfigurere arbeidsflyten til å sende e-postmeldinger uten å overskride [grensene for Exchange Online-avsender](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Du kan for eksempel bruke en pause i arbeidsflyten, sende e-postmeldingen til en Office 365-gruppe, en distribusjonsgruppe eller en sikkerhetsgruppe som er aktivert for e-post, eller sende meldingen til færre enn 200 mottakere om gangen.


Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Beslektede emner
- [Opprett flyt](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 