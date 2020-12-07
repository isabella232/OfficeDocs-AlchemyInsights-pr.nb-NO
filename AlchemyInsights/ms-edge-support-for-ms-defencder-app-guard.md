---
title: Microsoft Edges støtte for Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584016"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Microsoft Edges støtte for Microsoft Defender Application Guard

Utformet for Windows 10 og Microsoft Edge bruker Application Guard en metode for maskin vare isolasjon som lar en bruker navigere i et uklarert nettsted fra en isolert, Hyper-V-aktivert beholder, atskilt fra verts operativ systemet.

En organisasjons administrator definerer en liste over klarerte nett steder, Sky ressurser og interne nettverk. Når en bruker besøker et nettsted som ikke er i listen, vil Microsoft Edge åpne området i beholderen. Dette betyr at hvis området blir skadelig, forblir Verts-PCen beskyttet, og angriperen vil ikke få tilgang til virksomhets dataene.

Installasjon av utvidelser i beholderen støttes på Microsoft Edge versjon 81, og den kan kontrolleres via en policy. UpdateURL-adressen som brukes i ExtensionInstallForcelist-policyen, skal legges til som en nøytral ressurs i policyene for nettverks isolasjon som brukes av Application Guard.

Hvis du vil ha mer informasjon, kan du se [Microsoft Edge-støtte for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).
