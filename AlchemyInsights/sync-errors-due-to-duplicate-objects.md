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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708071"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synkroniseringsfeil på grunn av dupliserte objekter

Du kan få en av følgende feilmeldinger når katalogsynkroniseringen fullføres i Microsoft 365:

- Kan ikke oppdatere dette objektet i Microsoft Online Services fordi følgende attributter som er knyttet til dette objektet, har verdier som kanskje allerede er knyttet til et annet objekt i den lokale katalogen.

- Et synkronisert objekt med samme proxy-adresse finnes allerede i Microsoft Online Services-katalogen.

- Kan ikke oppdatere dette objektet fordi følgende attributter som er knyttet til dette objektet, har verdier som kanskje allerede er knyttet til et annet objekt i de lokale katalogtjenestene: UserPrincipalName.

Hvis du vil identifisere og løse problemet, kan du laste ned og kjøre [feilutbedringsverktøyet IdFix DirSync.](https://github.com/Microsoft/idfix)

Hvis du vil ha mer informasjon, kan du [se KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
