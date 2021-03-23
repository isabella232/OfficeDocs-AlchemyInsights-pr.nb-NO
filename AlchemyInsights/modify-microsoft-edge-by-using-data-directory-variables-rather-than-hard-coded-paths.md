---
title: Endre Microsoft Edge ved hjelp av datakatalogvariabler i stedet for hardkodede baner
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035823"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Endre Microsoft Edge ved hjelp av datakatalogvariabler i stedet for hardkodede baner

Hvis du for eksempel vil lagre profildataene under brukerens lokale programdata i stedet for i standardplasseringen, angir du *UserDataDir-policyen* til **${local_app_data}\Edge\Profile** i Windows.

Hvis du vil ha mer informasjon, kan [du se Opprette katalogvariabler for Microsoft Edge-brukerdata](https://docs.microsoft.com/deployedge/microsoft-edge-policies).