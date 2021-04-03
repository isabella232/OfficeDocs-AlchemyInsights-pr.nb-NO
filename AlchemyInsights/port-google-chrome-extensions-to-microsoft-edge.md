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
- "8297"
- "9004617"
ms.openlocfilehash: 1c71d74d01c1e38e4c7789aea2c0b43701b3a5de
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505293"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Port Google Chrome-utvidelser til Microsoft Edge (Chromium)

Det er enkelt å [portere Google Chrome-utvidelser til Microsoft Edge (Chromium).](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension) I de fleste tilfeller er det bare nødvendig med minimale endringer for å kjøre disse utvidelsene på Microsoft Edge.

Utvidelses-API-ene og manifestnøklene som støttes av Google Chrome, er kodekompatible med Microsoft Edge. Microsoft Edge støtter imidlertid ikke utvidelsen API-er chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken og chrome.instanceID.