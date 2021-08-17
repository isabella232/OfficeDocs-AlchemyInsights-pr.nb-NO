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
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110689"
---
# <a name="replica-set"></a>Replikasett

AADDS kalles også som det administrerte domenet. Det er faktisk to domenekontrollere som kjøres og vedlikeholdes av backend. De to DCene inkluderer én hoved-DC og én replikerings-DC. Sikkerhetskopier i AADDS (administrert domene) er en automatisert prosess som administreres av Azure-plattformen. Hvis det oppstår et problem med det administrerte domenet, kan Azure-støtte hjelpe deg med å gjenopprette fra sikkerhetskopieringen.

Du oppretter hvert replikasett i et virtuelt nettverk. Hvert virtuelle nettverk må nodes til alle andre virtuelle nettverk som er vert for replikasettet til et administrert domene. Denne konfigurasjonen oppretter en nettverkstopologi for nett som støtter katalogreplikering. Et virtuelt nettverk kan støtte flere replikasett, forutsatt at hvert replikasett er i et annet virtuelt delnett.

Hvis du vil ha mer informasjon om replikasett, kan du [se Konsepter replikasett](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
