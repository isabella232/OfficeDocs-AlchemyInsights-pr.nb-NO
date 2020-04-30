---
title: Bruker DLP i transportregler
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915188"
---
# <a name="using-dlp-in-transport-rules"></a>Bruker DLP i transportregler

Hvis du vil integrere hindring av tap av data (DLP) i en eksisterende transport, bruker du betingelsen «**Hvis meldingen inneholder...Sensitiv informasjon**» i Transport-regelinnstillingen.

**Hvis du vil ha mer informasjon, kan du se:**

- Integrerte DLP-sensitive informasjonstyper i transportregler: [Integrere sensitive informasjonsregler](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Du kan også teste regelen med eller uten policytesting ved hjelp av testmodus på regelen.  Du bør vente 30 minutter etter at du har opprettet regelen før du tester den.

- Se [Test e-postflyt/transportregler](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Obs**: Hvis du prøver å implementere en ny DLP-policy med transportregler i EAC-en, kan du bruke [DLP-policyer i sikkerhets- og samsvarssenteret](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) i stedet.
