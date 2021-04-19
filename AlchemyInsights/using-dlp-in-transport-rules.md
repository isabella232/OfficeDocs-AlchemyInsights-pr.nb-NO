---
title: Bruker DLP i transportregler
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827225"
---
# <a name="using-dlp-in-transport-rules"></a>Bruker DLP i transportregler

Hvis du vil integrere hindring av tap av data (DLP) i en eksisterende transport, bruker du betingelsen «**Hvis meldingen inneholder...Sensitiv informasjon**» i Transport-regelinnstillingen.

**Hvis du vil ha mer informasjon, kan du se:**

- Integrerte DLP-sensitive informasjonstyper i transportregler: [Integrere sensitive informasjonsregler](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Du kan også teste regelen med eller uten policytesting ved hjelp av testmodus på regelen.  Du bør vente 30 minutter etter at du har opprettet regelen før du tester den.

- Se [Test e-postflyt/transportregler](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Obs**: Hvis du prøver å implementere en ny DLP-policy med transportregler i EAC-en, kan du bruke [DLP-policyer i sikkerhets- og samsvarssenteret](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) i stedet.
