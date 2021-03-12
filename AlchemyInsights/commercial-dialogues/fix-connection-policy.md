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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750606"
---
# <a name="fix-connection-policy"></a>Løse tilkoblingspolicy

E-postmeldingen ble merket som sikker og levert til brukerens innboks fordi den sendte IP-adressen ble merket som sikker i policyen for tilkoblingsfilteret. Gjør følgende for å se gjennom policyen:

1. Gå til sikkerhets- og samsvarssenteret [for Office 365 &](https://go.microsoft.com/fwlink/p/?linkid=2077143), og gå deretter til Policy for beskyttelse mot søppelpost for   >    >  [trusler.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Velg Policy **for** tilkoblingsfilter på Egendefinert-fanen, og velg deretter Rediger **policy**.
3. Se gjennom **tillatelseslisten for IP.** Se om **Sikker-listen** er aktivert.

    > [!NOTE]
    > Microsoft abonnerer på tredjepartskilder for klarerte avsendere. Hvis **Sikker-listen** er aktivert, merkes ikke disse klarerte avsenderne feilaktig som søppelpost. Jeg anbefaler å velge dette alternativet, fordi det vil redusere antall falske positiver (god e-post som er klassifisert som søppelpost) som du mottar.
