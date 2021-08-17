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
ms.openlocfilehash: ebc0fb718eb0572e849c5d780977deaee480a00c2825c18a12e4d2212342f17a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084103"
---
# <a name="using-dlp-in-transport-rules"></a>Bruker DLP i transportregler

Hvis du vil integrere hindring av tap av data (DLP) i en eksisterende transport, bruker du betingelsen «**Hvis meldingen inneholder...Sensitiv informasjon**» i Transport-regelinnstillingen.

**Hvis du vil ha mer informasjon, kan du se:**

- Integrerte DLP-sensitive informasjonstyper i transportregler: [Integrere sensitive informasjonsregler](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Du kan også teste regelen med eller uten policytesting ved hjelp av testmodus på regelen.  Du bør vente 30 minutter etter at du har opprettet regelen før du tester den.

- Se [Test e-postflyt/transportregler](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Obs**: Hvis du prøver å implementere en ny DLP-policy med transportregler i EAC-en, kan du bruke [DLP-policyer i sikkerhets- og samsvarssenteret](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) i stedet.
