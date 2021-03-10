---
title: Eksempel på policy for Klarerte vedlegg for Microsoft Defender for Office 365
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
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695180"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Eksempel på policy for Klarerte vedlegg for Microsoft Defender for Office 365

Disse innstillingene aktiverer en policy *kalt* Ingen forsinkelser som leverer meldinger umiddelbart, og som deretter fester vedlegg på nytt etter at de er skannet:

- **Navn:** Ingen forsinkelser
- **Beskrivelse:** Leverer meldinger umiddelbart og fester vedlegg på nytt etter skanning.
- **Svar:** Velg alternativet **Dynamisk** levering. Hvis du vil ha mer informasjon, kan du se policyer for dynamisk [levering i klarerte vedlegg.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Omdiriger** vedlegg-delen: Velg alternativet for å aktivere omadressering, og skriv deretter inn e-postadressen til den globale Microsoft 365-administratoren, sikkerhetsadministratoren eller sikkerhetsanalytikeren som skal undersøke skadelige vedlegg.
- **Applied To** section: Select **The recipient domain is,** and then select your domain. Velg **Legg til,** og velg deretter **OK.** Når du er ferdig, velger du **Lagre.**

Hvis du vil ha mer informasjon, kan du [se Klarerte vedlegg i Microsoft Defender for Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)
