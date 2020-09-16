---
title: Daglig e-postgrense overskredet. Arbeids flyten er suspendert.
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
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731572"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Daglig e-postgrense overskredet. Arbeids flyten er suspendert.

Denne feilen kan bli mottatt i følgende scenarioer:

- Du har en arbeids flyt i SharePoint Online som bruker arbeids flyt plattform typen for SharePoint 2010 eller SharePoint 2013.
- Arbeids flyten er konfigurert til å sende en egen definert e-postmelding til flere enn 200 brukere om gangen, mer enn 10 000 mottakere per dag eller mer enn 30 meldinger per minutt.
- Når du kjører arbeids flyten, sendes ikke e-postmeldingen, og du ser følgende virke måte:
    - For en arbeids flyt som bruker plattform typen for SharePoint 2013, går du til status siden for **arbeids flyten** . På status siden for arbeids flyten er den **interne statusen** satt til **startet**, og informasjons boblen **kan ikke sendes til en mottaker**.

Du kan omgå dette problemet ved å konfigurere arbeids flyten til å sende e-postmeldinger uten å overskride [grensen for Exchange Online-avsenderen](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Bruk for eksempel en pause i arbeids flyten, Send e-post til en Microsoft 365-gruppe, en distribusjons gruppe eller e-postaktivert sikkerhets gruppe, eller send meldingen til færre enn 200 mottakere om gangen.


Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Beslektede emner
- [Opprett flyt](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og flyt](https://flow.microsoft.com/blog/sharepoint-and-flow/) 