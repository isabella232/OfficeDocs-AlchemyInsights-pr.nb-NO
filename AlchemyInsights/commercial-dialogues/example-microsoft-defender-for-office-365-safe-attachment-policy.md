---
title: Eksempel på Microsoft Defender for policy for sikkert vedlegg i Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749202"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Eksempel på Microsoft Defender for policy for sikkert vedlegg i Office 365

Disse innstillingene aktiverer en policy kalt *Ingen forsinkelser* som leverer meldinger umiddelbart, og deretter vedlegg på nytt etter at de er skannet:

- **Navn:** Ingen forsinkelser
- **Beskrivelse:** Leverer meldinger umiddelbart, og vedlegg festes på nytt etter skanning.
- **Svar:** Velg alternativet **Dynamisk** levering. Hvis du vil ha mer informasjon, kan [du se Dynamisk levering i policyer for klarerte vedlegg](https://go.microsoft.com/fwlink/?linkid=2092328).
- **Omdiriger** vedlegg-delen: Velg alternativet for å Aktivere omadressering **,** og skriv deretter inn e-postadressen til den globale microsoft 365-administratoren, sikkerhetsadministratoren eller sikkerhetsanalytikeren som skal undersøke skadelige vedlegg.
- **Bruk på-delen:** **Velg Mottakerdomenet er**, og velg deretter domenet ditt. Velg **Legg til**, og velg deretter **OK**. Når du er ferdig, velger du **Lagre**.

Hvis du vil ha mer informasjon, kan du [se Klarerte vedlegg i Microsoft Defender for Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)
