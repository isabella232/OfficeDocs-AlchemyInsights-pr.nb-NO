---
title: Utgående videresendingsutvalg
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 8750c9036f258d9c5edc94bb027d564140bbd9914712cc1f25ff3abc3f4b9468
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54041595"
---
# <a name="outbound-relay-pool"></a>Utgående videresendingsutvalg

Microsoft gjør noen endringer i konfigurasjonen for videresending eller videresending av e-post via Microsoft 365. Meldinger i bestemte scenarier videresendes eller videresendes gjennom Microsoft 365 ved hjelp av et spesielt videresendingsutvalg. Meldinger som sendes ved hjelp av videresendingsutvalget, kan ende opp i mottakerens søppelpostmappe. Hvis du vil ha mer informasjon, kan du [se Utgående leveringsutvalg](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Hvis du vil unngå et scenario ved hjelp av videresendingsutvalget, må du kontrollere at videresendte/videresendte meldinger oppfyller ett av følgende kriterier:

- Den utgående avsenderen er et godtatt domene for leieren.
- SpF (Sender Policy Framework) sendes når meldingen kommer til Microsoft 365.
- DomainKeys Identified Mail (DKIM) på P2-avsenderdomenet sendes når meldingen kommer til Microsoft 365.
 
Meldinger som oppfyller vilkårene ovenfor, videresendes ikke gjennom videresendingsutvalget.

Hvis MX-posten for domenet peker til en tredjeparts eller lokal server, kan du bruke forbedret filtrering for å sikre at SPF-valideringen er riktig for inngående e-post og for å unngå å sende e-post gjennom videresendingsutvalget.

**Hvordan kan vi se om vi påvirkes av videresendingsutvalget?**

Hvis videresendte eller videresendte e-postmeldinger bruker et av vilkårene ovenfor, sendes ikke meldinger gjennom videresendingsutvalget. Hvis en melding sendes via et videresendingsutvalg, er imidlertid den utgående server-IP-adressen i området 40.95.0.0/16, og det utgående servernavnet inneholder **rly** i navnet.

