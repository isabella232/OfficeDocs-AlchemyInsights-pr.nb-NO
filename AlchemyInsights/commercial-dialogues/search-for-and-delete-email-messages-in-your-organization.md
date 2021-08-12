---
title: Søke etter og slette e-postmeldinger i organisasjonen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948892"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Søke etter og slette e-postmeldinger i organisasjonen

Følg disse trinnene:

1. Hvis du ikke er global administrator, må kontoen legges til **i rollegruppen for eDiscovery Manager** eller administrasjonsrollen for samsvarssøk for å søke etter **meldinger.** Hvis du vil slette meldinger, må du bli med i rollegruppen **organisasjonsbehandling** eller rollen søk og **tøm behandling.** Tillatelser til disse rollene tilordnes i [sikkerhetssenteret & samsvarssenteret.](https://protection.office.com)
2. [Opprett et innholdssøk for](https://docs.microsoft.com/office365/securitycompliance/content-search) å finne meldingen du vil slette.
3. [Koble til sikkerhets- & Samsvarssenter PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Hvis du bruker MFA, kan du se disse instruksjonene: Koble til [Sikkerhets-& Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell) ved hjelp av godkjenning med flere faktorer
4. Slett meldingen: Kjør `New-ComplianceSearchAction` cmdleten for å slette meldingen. Slettede meldinger flyttes til en brukers gjenopprettelige elementer-mappe. Hvis du vil ha en eksempelkommando, [kan du se Trinn 3: Slette meldingen.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
