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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695882"
---
# <a name="fix-connection-policy"></a>Løse tilkoblingspolicy

E-postmeldingen ble merket som sikker og levert til brukerens innboks fordi ip-adressen som sendes, ble merket som sikker i policyen for tilkoblingsfilter. Hvis du vil se gjennom policyen, gjør du følgende:

1. Gå til sikkerhetssenteret [for Office 365 &,](https://go.microsoft.com/fwlink/p/?linkid=2077143)og gå deretter **til** beskyttelse mot søppelpost for  >    >  [trusselbehandling.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Velg **policyen** for tilkoblingsfilter på Egendefinert-fanen, og velg deretter **Rediger policy.**
3. Se gjennom **ip-tillatelseslisten.** Se om **klarerte lister** er aktivert.

    > [!NOTE]
    > Microsoft abonnerer på tredjepartskilder for klarerte avsendere. Hvis **listen over klarerte** avsendere er aktivert, blir ikke disse klarerte avsenderne feilaktig merket som søppelpost. Jeg anbefaler å velge dette alternativet fordi det vil redusere antall falske positiver (god e-post som klassifiseres som søppelpost) som du mottar.
