---
title: Port Google Chrome-utvidelser til Microsoft Edge (Chromium)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677875"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Port Google Chrome-utvidelser til Microsoft Edge (Chromium)

Det er enkelt å [havne Google Chrome-utvidelser til Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension). I de fleste tilfeller er det bare nødvendig med minimale endringer for å kjøre disse utvidelsene i Microsoft Edge.

Utvidelses-APIene og manifest nøklene som støttes av Google Chrome, er kode kompatible med Microsoft Edge. Microsoft Edge støtter imidlertid ikke Utvidelses-APIene Chrome. GCM, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken og Chrome. instanceID.