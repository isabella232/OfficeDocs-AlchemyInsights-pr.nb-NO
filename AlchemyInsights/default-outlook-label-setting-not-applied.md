---
title: Standard Outlook ikke er i bruk
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/17/2021
ms.locfileid: "58455092"
---
# <a name="default-outlook-label-setting-not-applied"></a>Standard Outlook ikke er i bruk

Hvis Outlook standard etikettinnstillinger ikke brukes riktig og en annen etikett eller ingen etikett brukes, kan det være et kjent problem (MC277818) og bør gjøre ett av disse to alternativene for å løse problemet:

**Alternativ 1:**

1. Gå til Microsoft 365 compliance center > **Solutions**  >  **Information Protection**.
1. Velg **Etikettpolicyer**, og velg etikettpolicyen du vil redigere (**OutlookDefaultlabel-innstillingen** er ikke riktig angitt på den aktuelle etikettpolicyen. Kjør **Get-labelpolicy for** å vise denne innstillingen), og velg deretter **Rediger policy**.
1. Velg **Neste** til du ser innstillingen Bruk denne standardetiketten på e-postmeldinger **,** som er tilgjengelig hvis  du velger Krev at brukere bruker en etikett på arving **av** e-postmeldinger og dokumenter i dialogboksen Policyinnstillinger.
1. Velg **Ingen** fra rullegardinlisten i dialogboksen  Bruk en standardetikett på dokumenter.
1. Velg **Neste** og **Send for** å lagre etikettinnstillingene.

**Alternativ 2:**

I [Sikkerhets- og samsvarssenteret Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)bruker du Set-LabelPolicy-kommandoleten til å endre **OutlookDefaultlabel** til **Ingen** på {OutlookDefaultLabel="None"}.

Kjør: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Hvis du vil ha mer informasjon om standardetiketter for Outlook, kan du se Angi en annen [standardetikett for Outlook](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook).