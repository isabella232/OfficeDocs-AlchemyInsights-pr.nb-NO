---
title: Frigjør diskplass i Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: c7d29ab718be8dbdcde61a7de2f158fb3bbd722d2964d8b13cde9936dd1e5ee1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928090"
---
# <a name="free-up-drive-space-in-windows-10"></a>Frigjør diskplass i Windows 10

Her er to alternativer for å frigjøre diskplass i Windows:

- Frigjøre diskplass i Windows 10.
- Frigjør plass for oppdateringer for Windows 10 med ekstern lagringsenhet.

Hvis du fremdeles har lite diskplass etter å ha brukt Diskopprydding, er det mulig at den midlertidige mappen raskt fylles opp med programfiler (.appx) som brukes av Microsoft Store. Du kan løse dette problemet ved å tilbakestille Store, tømme hurtigbufferen for Store og deretter kjøre feilsøkingsverktøyet for Windows Update. Kontroller at Microsoft Store er lukket før du fortsetter med disse trinnene.

**Trinn 1: Tilbakestill Microsoft Store**

**Obs!** Dette sletter app-dataene på enheten permanent, inkludert preferanser og påloggingsdetaljer.

1. Velg **Start** > **innstillinger** > **Apper** > **Apper og funksjoner**.

1. Finn og velg Microsoft Store i listen over apper.

1. Velg **Avanserte alternativer**.

1. Rull nedover og velg **Tilbakestill**, og deretter **Bekreft tilbakestilling**.

**Trinn 2: Tøm bufferen for Microsoft Store**

1. Trykk Windows-tasten + R for å åpne dialogboksen Kjør.

1. Skriv inn wsreset.exe, og **OK**.

1. Et tomt ledetekstvindu åpnes. Etter omtrent 10 sekunder lukkes vinduet, og Store åpnes automatisk.

**Trinn 3: Tilbakestill Windows Update**

1. Velg **Start** > **Innstillinger** > **Oppdatering og sikkerhet** > **Feilsøk**.

1. Rull nedover og velg **Windows Update** fra listen, og velg **Kjør feilsøkingsverktøyet**.

1. Start datamaskinen på nytt, og kontroller om du fremdeles har dette problemet.

