---
title: Daglig e-postgrense overskredet. Arbeidsflyten er deaktivert.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914660"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Daglig e-postgrense overskredet. Arbeidsflyten er deaktivert.

Denne feilen kan bli mottatt i følgende scenarier:

- Du har en arbeidsflyt i SharePoint Online som bruker arbeidsflytplattformtypen SharePoint 2010 eller SharePoint 2013.
- Arbeidsflyten er konfigurert til å sende en egendefinert e-postmelding til mer enn 200 brukere om gangen, mer enn 10 000 mottakere per dag eller mer enn 30 meldinger per minutt.
- Når du kjører arbeidsflyten, sendes ikke e-postmeldingen, og du legger merke til følgende virkemåte:
    - For en arbeidsflyt som bruker SharePoint 2013-plattformtypen, blar du til **arbeidsflytstatussiden.** Den interne statusen er  satt til Startet på Arbeidsflytstatus-siden, og informasjonsboblen viser **Kan ikke sende til en mottaker**.

Du kan omgå dette problemet ved å konfigurere arbeidsflyten til å sende e-postmeldinger uten å overskride Exchange Online [avsendergrenser](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Bruk for eksempel en pause i arbeidsflyten, send e-postmeldingen til en Microsoft 365-gruppe, en distribusjonsgruppe eller e-postaktivert sikkerhetsgruppe, eller send meldingen til færre enn 200 mottakere om gangen.


Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Beslektede emner
- [Opprette Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 