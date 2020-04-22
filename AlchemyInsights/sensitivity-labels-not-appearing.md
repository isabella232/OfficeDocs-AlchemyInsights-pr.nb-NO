---
title: Følsomhetsetiketter vises ikke
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 72dc88a55b55954f34c95fa5b5038f472261c5bb
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758470"
---
# <a name="sensitivity-labels-not-appearing"></a>Følsomhetsetiketter vises ikke

Sensitivitetsetiketter lar deg klassifisere og bidra til å beskytte sensitivt innhold. De kan opprettes i Microsoft 365 compliance center, Microsoft 365 security center eller Microsoft 365 security & Compliance Center under Klassifisering > Sensitivity etiketter. Hvis du vil vite mer om denne funksjonen, kan du se [Oversikt over følsomhetsetiketter](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).

Hvis du konfigurerte følsomhetsetikettene, men de ikke vises i Office-appene, kontrollerer du følgende:

- Kontroller at følsomhetsetiketten er [publisert](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) for brukerne og gruppene du vil bruke.

- Kontroller at brukeren bruker en app som støtter følsomhetsetiketter - se [følsomhetsetiketter i dokumentet](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Hvis du [overfører Azure Information Protection-etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), må du være oppmerksom på vurderingene som er oppført [her.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Støtte for hindring av tap av data (DLP): For øyeblikket kan bare oppbevaringsetiketter brukes som en betingelse i DLP-policyer.  Støtte for følsomhetsetiketter i en DLP-policy er ikke tilgjengelig ennå, men vi jobber med den.

- Når kryptering er aktivert på en følsomhetsetikett, kan du velge enten å:
    - Tilordne tillatelser nå
    - La brukere tilordne tillatelser


Hvis du vil ha mer informasjon om mulige problemer, kan du se [Kjente problemer med følsomhetsetiketter](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).