---
title: Løse tilkoblingspolicy
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988128"
---
# <a name="fix-connection-policy"></a>Løse tilkoblingspolicy

E-postmeldingen ble merket som sikker og levert til brukerens innboks fordi den sendte IP-adressen ble merket som sikker i policyen for tilkoblingsfilteret. Gjør følgende for å se gjennom policyen:

1. Gå til Office 365 [Sikkerhets- & samsvarssenter](https://go.microsoft.com/fwlink/p/?linkid=2077143), og gå deretter til **Policy** for trusselbehandling  >    >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Velg Policy **for** tilkoblingsfilter på Egendefinert-fanen, og velg deretter Rediger **policy**.
3. Se gjennom **tillatelseslisten for IP.** Se om **Safe er** aktivert.

    > [!NOTE]
    > Microsoft abonnerer på tredjepartskilder for klarerte avsendere. Hvis **Safe er** aktivert, blir ikke disse klarerte avsenderne feilaktig merket som søppelpost. Jeg anbefaler å velge dette alternativet, fordi det vil redusere antall falske positiver (god e-post som er klassifisert som søppelpost) som du mottar.
