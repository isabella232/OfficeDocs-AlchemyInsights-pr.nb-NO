---
title: Replikasett
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714252"
---
# <a name="replica-set"></a>Replikasett

AADDS kalles også det administrerte domenet. Det er faktisk to domenekontrollere som kjøres og vedlikeholdes av serverserveren. De to DC-ene inkluderer én hoved-DC og én replikerings-DC. Sikkerhetskopier i AADDS (administrert domene) er en automatisert prosess som administreres av Azure-plattformen. Hvis det oppstår et problem med det administrerte domenet, kan Azure-støtte hjelpe deg med å gjenopprette fra sikkerhetskopiering.

Du oppretter hvert replikasett i et virtuelt nettverk. Hvert virtuelle nettverk må nodenett til alle andre virtuelle nettverk som er vert for et administrert domenes replikeringssett. Denne konfigurasjonen oppretter en nettverkstopologi for nett som støtter katalogreplikering. Et virtuelt nettverk kan støtte flere replikasett forutsatt at hvert replikasett er i et annet virtuelt delnett.

Hvis du vil ha mer informasjon om replikasett, kan du [se Concepts Replica sets.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
