---
title: Komme i gang med SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700716"
---
# <a name="workflows-in-sharepoint"></a>Arbeids flyter i SharePoint

Hvis SharePoint-arbeidsflyter ikke sender e-postmeldinger, kan det hende at organisasjonen har funnet grensen for Exchange Online-avsenderen.

Feil meldingen «arbeids flyten er ute stengt» kan oppstå hvis du har ett av følgende elementer:

- Du har en arbeids flyt i SharePoint Online som bruker arbeids flyt plattform typen for SharePoint 2010 eller SharePoint 2013.

- Arbeids flyten er konfigurert til å sende en egen definert e-postmelding til flere enn 200 brukere om gangen, mer enn 10 000 mottakere per dag eller mer enn 30 meldinger per minutt.

Når du kjører arbeids flyten, sendes ikke e-postmeldingen, og du ser feil meldingen, den interne statusen er satt til suspendert eller kan ikke sendes til en mottaker.

Hvis du vil ha mer informasjon, kan du se [artikkelen](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)nedenfor.

