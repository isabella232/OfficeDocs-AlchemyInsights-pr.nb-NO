---
title: Komme i gang med SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 5e61491b626bfe75fd26a15ee54be82d9efa19a7
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766900"
---
# <a name="workflows-in-sharepoint"></a>Arbeidsflyter i SharePoint

Hvis SharePoint-arbeidsflyter ikke sender e-post, kan organisasjonen har oppdaget grensene for Exchange Online avsender.

Feilmeldingen "arbeidsflyten er suspendert" kan oppstå hvis du har ett av følgende elementer:

- Du har en arbeidsflyt i SharePoint Online som bruker SharePoint 2010 eller SharePoint 2013 arbeidsflyt plattformtype.

- Arbeidsflyten er konfigurert til å sende en egendefinert e-postmelding til mer enn 200 brukere om gangen, mer enn 10 000 mottakere per dag, eller mer enn 30 meldinger per minutt.

Når du kjører arbeidsflyten, e-postmeldingen er ikke sendt, og du legger merke til feilmeldingen, intern status er satt til suspendert eller kan ikke sende til en mottaker vises.

Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).

