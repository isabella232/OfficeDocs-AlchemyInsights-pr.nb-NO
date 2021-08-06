---
title: 902 (Synkroniseringsfeil på grunn av dupliserte objekter)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998803"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synkroniser feil på grunn av dupliserte objekter

Du kan få en av følgende feilmeldinger når katalogsynkroniseringen er ferdig i Microsoft 365:

- Kan ikke oppdatere dette objektet i Microsoft Online Services fordi følgende attributter som er knyttet til dette objektet, har verdier som kanskje allerede er knyttet til et annet objekt i den lokale katalogen.

- Et synkronisert objekt med samme proxy-adresse finnes allerede i Microsoft Online Services-katalogen.

- Kan ikke oppdatere dette objektet fordi følgende attributter som er knyttet til dette objektet, har verdier som kanskje allerede er knyttet til et annet objekt i de lokale katalogtjenestene: UserPrincipalName.

Hvis du vil identifisere og løse problemet, kan du laste ned og kjøre verktøyet for utbedring av [IdFix DirSync-feil.](https://github.com/Microsoft/idfix)

Hvis du vil ha mer informasjon, kan du se [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
