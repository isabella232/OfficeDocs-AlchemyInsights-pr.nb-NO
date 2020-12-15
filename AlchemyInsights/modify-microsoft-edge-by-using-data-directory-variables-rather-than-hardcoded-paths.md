---
title: Endre Microsoft Edge ved å bruke data katalog variabler i stedet for hardkodete baner
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679158"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Endre Microsoft Edge ved å bruke data katalog variabler i stedet for hardkodete baner

I Windows kan du for eksempel lagre profil dataene under en brukers lokale program data i stedet for i standard plasseringen, ved å angi **UserDataDir** -policyen til **$ {local_app_data} \Edge\Profile**. 

Hvis du vil ha mer informasjon, kan du se [opprette Microsoft Edge user data Directory-variabler](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).