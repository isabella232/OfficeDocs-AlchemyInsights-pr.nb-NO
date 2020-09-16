---
title: Følsomhet-etiketter vises ikke
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801193"
---
# <a name="sensitivity-labels-not-appearing"></a>Følsomhet-etiketter vises ikke

Med følsomhet-etiketter kan du klassifisere og bidra til å beskytte sensitivt innhold. De kan opprettes i samsvars senteret for Microsoft 365, Microsoft 365 Security Center eller Microsoft 365-sikkerhets & Samsvars senteret under klassifisering > følsomhet-etiketter. Hvis du vil lære mer om denne funksjonen, kan du se [Oversikt over følsomhet-etiketter](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Hvis du har konfigurert følsomhet-etikettene, men de ikke vises i Microsoft 365-appene, kan du kontrollere følgende:

- Kontroller at følsomhet-etiketten er [publisert](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) til brukerne og gruppene du vil bruke.

- Kontroller at brukeren bruker en app som støtter følsomhet-etiketter – se [følsomhet-etiketter i dokumentet](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Hvis du [overfører Azure Information Protection-etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), må du være oppmerksom på hvilke vurderinger som er oppført [her](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Støtte for hindring av tap av data (DLP): nå kan bare oppbevarings etiketter brukes som en betingelse i policyer for DLP.  Støtte for følsomme etiketter i en DLP-policy er ikke tilgjengelig ennå, men vi jobber med den.

- Når kryptering er aktivert på en følsomhet-etikett, kan du velge begge til:
    - Tilordne tillatelser nå
    - La brukere tilordne tillatelser


Hvis du vil ha mer informasjon om mulige problemer, kan du se [kjente problemer med følsomhet-etiketter](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).