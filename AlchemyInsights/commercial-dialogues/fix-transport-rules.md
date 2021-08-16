---
title: Løse transportregler
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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034763"
---
# <a name="fix-transport-rules"></a>Løse transportregler

En egendefinert e-postflytregel påvirket denne meldingen. Hvis du vil se gjennom den nøyaktige regelen, gjør du følgende:

1. Legg merke til GUID-en eller  policynavnet under **Tilleggsinformasjon** i **innsendingsresultatene.**
2. Start Exchange administrasjonsskall. Hvis du vil ha mer informasjon, [kan du se Åpne Exchange Administrasjonsskall](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Kjør denne kommandoen (ved hjelp av GUID fra innsendingen):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Se gjennom beskrivelsen for å se de konfigurerte betingelsene som påvirket meldingen.

Hvis du vil ha mer informasjon, [kan du se Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
