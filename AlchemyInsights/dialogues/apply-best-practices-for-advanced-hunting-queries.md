---
title: Bruk anbefalte fremgangsmåter for avanserte søk
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696089"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Bruk anbefalte fremgangsmåter for avanserte søk

Bruk disse anbefalte fremgangsmåtene for å få resultater raskere og unngå tidsavbrudd når du kjører komplekse spørringer:

- Når du prøver nye spørringer, bør du alltid bruke en grense for å unngå å få svært store resultatsett. Bruk også denne til å gjøre en innledende vurdering av størrelsen `count` på resultatsettet.
- Bruk tidsfiltre først. Ideelt sett bør du begrense spørringene til sju dager.
- I begynnelsen av en spørring, rett etter tidsfilteret, legger du til filtrene som forventes å fjerne mesteparten av dataene.
- Når du leter etter fullstendige tokener, bruker du `has` operatoren i stedet for `contains` .
- Kjør et søk på en bestemt kolonne i stedet for på tvers av alle kolonner.
- Når du føyer sammen tabeller, må du først angi tabellen med færre rader.
- `project` bare de nødvendige kolonnene fra tabellene du har sammenføyd.

Hvis du vil ha mer informasjon, kan du [se anbefalte fremgangsmåter for avansert søk for søk.](https://go.microsoft.com/fwlink/?linkid=2144812)
