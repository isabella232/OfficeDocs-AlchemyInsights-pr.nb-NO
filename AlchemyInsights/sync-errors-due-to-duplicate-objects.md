---
title: 902 (Synkroniser feil på grunn av dupliserte objekter)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767143"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synkronisere feil på grunn av dupliserte objekter

Du kan få en av følgende feilmeldinger når katalogsynkronisering er ferdig i Microsoft 365:

- Kan ikke oppdatere dette objektet i Microsoft Online Services fordi følgende attributter som er knyttet til dette objektet, har verdier som allerede er knyttet til et annet objekt i den lokale katalogen.

- Det finnes allerede et synkronisert objekt med samme proxy-adresse i Microsoft Online Services-katalogen.

- Kan ikke oppdatere dette objektet fordi følgende attributter som er knyttet til dette objektet, har verdier som allerede er knyttet til et annet objekt i de lokale katalogtjenestene: UserPrincipalName.

Hvis du vil identifisere og løse problemet, laster du ned og kjører [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).

Hvis du vil ha mer informasjon, kan du se [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
