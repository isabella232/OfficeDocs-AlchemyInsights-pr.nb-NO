---
title: Følsomhet etiketter vises ikke
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 4bf8e02246c966f22648467386a7862f0521fecf
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207234"
---
# <a name="sensitivity-labels-not-appearing"></a>Følsomhet etiketter vises ikke

Med følsomme etiketter kan du klassifisere og bidra til å beskytte det sensitive innholdet ditt. De kan opprettes i Microsoft 365 samsvarssenter, Microsoft 365 Sikkerhetssenter eller Office 365 sikkerhet & Compliance Center under klassifisering > følsomhet etiketter. Hvis du vil vite mer om denne funksjonen, kan du se [Oversikt over følsomhet etiketter](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).

Hvis du konfigurerte følsomhet etikettene dine, men de vises ikke i Office-appene, kontrollerer du følgende:

- Kontroller at følsomheten etiketten er [publisert](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) til brukerne og gruppene du ønsker.

- Bekreft at brukeren bruker en app som støtter følsomhet etiketter-se [følsomhet etiketter i dokumentet](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).

- Hvis du [overfører etiketter for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), må du være klar over hvilke betraktninger som er oppført [her](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Støtte for hindring av datatap (DLP): for øyeblikket kan bare oppbevarings etiketter brukes som en betingelse i DLP-policyer.  Støtte for følsomhet etiketter i en DLP-policy er ikke tilgjengelig ennå, men vi jobber med det.

- Når kryptering er aktivert på en følsomhet etikett, kan du velge enten å:
    - Tilordne tillatelser nå
    - La brukere tilordne tillatelser


Hvis du vil ha mer informasjon om mulige problemer, kan du se [kjente problemer med følsomhet etiketter](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).