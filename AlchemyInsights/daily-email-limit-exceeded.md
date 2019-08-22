---
title: Daglig e-post er oversteget. Arbeidsflyten er avbrutt.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514472"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Daglig e-post grensen overskredet. Arbeidsflyten er avbrutt.

Denne feilen kan mottas i følgende scenarier:

- Du har en arbeidsflyt i SharePoint Online som bruker SharePoint 2010 eller SharePoint 2013 arbeidsflyttypen plattform.
- Arbeidsflyten er konfigurert til å sende en egendefinert e-postmelding til mer enn 200 brukere samtidig, mer enn 10 000 mottakere per dag, eller i mer enn 30 meldinger per minutt.
- Når du starter arbeidsflyten, i e-postmeldingen sendes ikke, og du legge merke til følgende virkemåte:
    - For en arbeidsflyt ved hjelp av SharePoint 2013-plattformtype, bla til siden **Status for arbeidsflyt** . Den **Interne statusen** er satt til **startet**på siden Status for arbeidsflyt, og boblen informasjon viser **kan ikke sende til en mottaker**.

Du kan omgå dette problemet ved å konfigurere arbeidsflyten for å sende e-postmeldinger uten å overskride [grensene for Exchange Online avsender](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Hvis du for eksempel bruke en pause i arbeidsflyten, sende e-postmeldingen til en Office 365-gruppen, en distribusjonsgruppe eller sikkerhetsgruppe for e-post er aktivert eller sende meldingen til færre enn 200 mottakere om gangen.


Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Beslektede emner
- [Opprette flyt](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og flyt](https://flow.microsoft.com/blog/sharepoint-and-flow/) 