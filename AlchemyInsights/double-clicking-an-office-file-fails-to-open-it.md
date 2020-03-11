---
title: Dobbeltklikking av en Office-fil kan ikke åpne den
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: cd45d64108bc3d7b8f35b51389294f5b8253ba9c
ms.sourcegitcommit: 6df4460313ca033d18b59669506de1dbb7482ef9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2020
ms.locfileid: "42573592"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Dobbeltklikking av en Office-fil kan ikke åpne den

Når du har dobbeltklikket en Office-fil, kan du se programmet åpent, men selve filen åpnes ikke. Eller du kan få feilmeldingen: "Det oppstod et problem under sending av kommandoen til programmet." Det er mange årsaker til dette, men de to vanligste løsningene er:

- Fra Excel må du kontrollere at DDE-alternativet ikke er merket av for. Alternativet kan bli funnet ved å opprette en ny arbeidsbok og deretter velge **Fil > alternativer > Avansert**. Fjern merket for Ignorer **andre programmer som bruker Dynamisk datautveksling (DDE)** i **Generelt-delen.**

- Kjør en tilkoblet reparasjon for å gjenopprette standardinnstillingene. Klikk startknappen i Windows, og søk etter "Kontrollpanel". Åpne **Kontrollpanel ,** og gå til **Programmer > programmer og funksjoner**. Høyreklikk deretter **Microsoft Office [Versjon]** og velg **Endre > Tilkoblet reparasjon**.

Hvis ingen av disse løsningene fungerer, finner du en mer fullstendig liste over løsninger i støtteartikkelen, hvis du ikke åpner den [for å dobbeltklikke en Office-fil](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).
