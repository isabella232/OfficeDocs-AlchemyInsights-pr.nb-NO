---
title: 902 (synkroniserings feil på grunn av dupliserte objekter)
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
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737350"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synkroniserings feil på grunn av dupliserte objekter

Du kan få en av følgende feil meldinger når katalog synkronisering er fullført i Microsoft 365:

- Kan ikke oppdatere dette objektet i Microsoft Online Services fordi følgende attributter som er knyttet til dette objektet, har verdier som allerede kan være knyttet til et annet objekt i den lokale katalogen.

- Det finnes allerede et synkronisert objekt med samme proxy-adresse i Microsoft Online Services-katalogen.

- Kan ikke oppdatere dette objektet fordi følgende attributter som er knyttet til dette objektet, har verdier som allerede kan være knyttet til et annet objekt i den lokale katalog tjenesten: UserPrincipalName.

Hvis du vil identifisere og løse problemet, kan du laste ned og kjøre [verktøyet for utbedring av IdFix DirSync-feil](https://www.microsoft.com/download/details.aspx?id=36832).

Hvis du vil ha mer informasjon, kan du se [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
